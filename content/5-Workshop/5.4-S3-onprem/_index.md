---
title : "Testing and Validation"
date : 2024-01-01
weight : 4
chapter : false
pre : " <b> 5.4. </b> "
---

After successful deployment, perform system testing with the following steps to confirm the entire workflow works as designed.

## 1. Send request

Send a real request to the API to check the end-to-end workflow.

### 1.1 Create presigned URL

```bash
curl -X POST "<ApiUrl>api/presigned-url" ^
  -H "Content-Type: application/json" ^
  -d "{\"fileName\":\"sample.mp4\",\"targetFormat\":\"webm\"}"
```

Expected response contains `jobId`, `uploadUrl`, `key`.
![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image.png)

### 1.2 Upload file to S3 via presigned URL

```bash
curl -X PUT "<uploadUrl>" ^
  -H "Content-Type: video/mp4" ^
  --data-binary "@sample.mp4"
```

Expected: HTTP `200` or `204`.
![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-1.png)

### 1.3 Check job status

```bash
curl "<ApiUrl>api/job-status/<jobId>"
```

Repeat the request until `status` changes to `COMPLETED`.

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-2.png)

## 2. View logs

Check CloudWatch Logs to confirm each Lambda function was invoked correctly and there are no runtime errors.

1. Go to **CloudWatch Console → Log groups**.
2. Select the log group for each function:
   - `/aws/lambda/CloudMediaConverterServer-GetPresignedUrlFunction...`
   - `/aws/lambda/CloudMediaConverterServer-GetJobStatusFunction...`
   - `/aws/lambda/CloudMediaConverterServer-ProcessUploadFunction...`
3. Open the latest **Log stream**, verify:
   - There are `START RequestId...` and `END RequestId...` lines for each invocation.
   - No `ERROR` or exception trace exists in the `ProcessUploadFunction` logs (where ffmpeg conversion runs).
   - Duration and Billed Duration are reasonable and not timed out.

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-3.png)

<div align = "center">Valid logs, no timeout or error</div>

## 3. Check metrics

Check CloudWatch Metrics to evaluate performance and error rates at the system level.

1. Go to **CloudWatch → Metrics → Lambda**.
2. For each function, check key metrics:
   - **Invocations**: number of calls, matching the number of test requests sent.
   - **Errors**: must be `0` after successful testing.
   - **Duration**: processing time, especially note `ProcessUploadFunction` because media conversion can take time.
   - **Throttles**: must be `0`; if not, it means the concurrency limit was exceeded.
3. For API Gateway, also check:
   - **4XXError** / **5XXError**: must be `0` for valid requests.
   - **Latency**: average API response time.

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-4.png)
<div align = "center">Metrics indicate the functions are valid</div>

## 4. Error testing

Actively test error cases to confirm the system handles and reports errors correctly, not just the happy path.

|No.| Case | How to test | Expected result |
|---|---|---|---|
| 1 | File not found when polling status | Call `GET /api/job-status/<nonexistent jobId>` | API returns `404` or a clear response indicating the job was not found |
| 2 | Input file is invalid/corrupt | Upload an empty file or a non-media file | `ProcessUploadFunction` sets job status to `FAILED`, with a specific `errorMessage` in DynamoDB |
| 3 | Call API with wrong method | e.g. call `GET /api/presigned-url` instead of `POST` | API Gateway returns `403`/`404` according to route configuration |

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-5.png)
<div align = "center">Result of testcase 1</div>

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-6.png)
<div align = "center">Result of testcase 2</div>

![alt text](/fcj-workshop/images/5-Workshop/5.4-S3-onprem/image-7.png)
<div align = "center">Result of testcase 3</div>

## 5. Expected results

After completing the above test and validation steps, the system should meet these criteria:

- The **happy path** (upload → convert → download) runs successfully through both UI and CLI.
- All Lambda function logs show **no runtime errors** when processing valid requests.
- Metrics show **Errors = 0**, **Throttles = 0** during testing.
- Error cases are handled correctly: return appropriate status codes, job status changes to `FAILED` with a clear `errorMessage` rather than crashing or hanging.
- Data in S3 (raw/processed) and DynamoDB (Jobs table) matches the actual outcome of each test run.

