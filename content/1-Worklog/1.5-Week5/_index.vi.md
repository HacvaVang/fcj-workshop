---
title: "Worklog Tuần 5"
date: 2024-01-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Tự động hóa việc khởi tạo và quản lý hạ tầng đề tài bằng AWS CloudFormation.
* Viết và chuẩn hóa mẫu template CloudFormation cho toàn bộ tài nguyên hệ thống.
* Kiểm thử triển khai và cập nhật hạ tầng thông qua CloudFormation Stack.

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 06/07/2026 | **Xây dựng Mạng & Hạ tầng cơ sở (IaC):**<br>&emsp;+ Viết CloudFormation template tạo VPC, Public/Private Subnets, Internet Gateway, Route Tables.<br>&emsp;+ Thực hành triển khai và kiểm thử Stack mạng cơ bản. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| 3 | 07/07/2026 | **Xây dựng Lớp Tính toán & Mở rộng (Compute & Scaling):**<br>&emsp;+ Viết template khởi tạo Security Groups, Launch Template, Auto Scaling Group và Application Load Balancer (ALB).<br>&emsp;+ Tích hợp tham số (Parameters) và tham chiếu (Ref/GetAtt) trong CloudFormation. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| 4 | 08/07/2026 | **Xây dựng Lớp Lưu trữ & Cơ sở dữ liệu (Storage & Database):**<br>&emsp;+ Viết template khởi tạo S3 Bucket, DynamoDB Table và tích hợp khóa KMS đã tạo ở tuần trước.<br>&emsp;+ Đóng gói thành các Nested Stacks hoặc Modular Templates. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| 5 | 09/07/2026 | **Triển khai & Debug Stack tổng hợp:**<br>&emsp;+ Triển khai toàn bộ hạ tầng dự án qua CloudFormation Stack tổng hợp.<br>&emsp;+ Xử lý các lỗi phát sinh trong quá trình khởi tạo (Rollback, Dependency errors). | <https://cloudjourney.awsstudygroup.com/> |
| 6 | 10/07/2026 | **Tự động hóa Cập nhật & Tổng kết tuần:**<br>&emsp;+ Thực hành sử dụng Change Sets để cập nhật hạ tầng an toàn.<br>&emsp;+ Kiểm tra tính sẵn sàng của hệ thống sau triển khai và cập nhật báo cáo tuần 5. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 5:

* **Tự động hóa Hạ tầng (AWS CloudFormation):**
  * Số hóa toàn bộ hạ tầng dự án thành mã nguồn (Code) dạng YAML/JSON theo đúng chuẩn IaC.
  * Viết thành công bộ CloudFormation template hoàn chỉnh bao gồm VPC, Subnet, ALB, ASG, EC2, S3, DynamoDB và KMS.
  * Cấu trúc template hợp lý, dễ tái sử dụng và mở rộng cho các giai đoạn tiếp theo.

* **Quản lý Triển khai (Stack Management):**
  * Triển khai thành công toàn bộ hệ thống chỉ qua một thao tác khởi tạo CloudFormation Stack.
  * Thực hành debug lỗi triển khai Stack, xử lý rollback và dependency errors.
  * Sử dụng Change Sets để cập nhật hạ tầng an toàn, giảm thiểu gián đoạn dịch vụ.