---
title: "Worklog Week 4"
date: 2024-01-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Goals for Week 4:

* Complete overall system architecture diagram and detailed task breakdown for each team member.
* Research AWS Key Management Service (KMS) encryption key management service.
* Practice creating encryption keys and applying data security to AWS services.

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 29/06/2026 | **System Architecture Design:**<br>&emsp;+ Finalize detailed overall architecture diagram on draw.io.<br>&emsp;+ Discuss and finalize data flow between components. | <https://cloudjourney.awsstudygroup.com/> |
| Tue | 30/06/2026 | **Team Task Assignment:**<br>&emsp;+ Hold team meeting to assign detailed module tasks to each member (Frontend, Backend, Infra/AWS).<br>&emsp;+ Set up shared development environment (Git repository, AWS IAM Accounts). | <https://cloudjourney.awsstudygroup.com/> |
| Wed | 01/07/2026 | **Learn AWS KMS (Key Management Service):**<br>&emsp;+ Concepts of KMS, AWS Managed Keys, and Customer Managed Keys (CMK).<br>&emsp;+ Data encryption mechanisms At-Rest (storage) and In-Transit (transmission).<br>&emsp;+ Key access policies (Key Policies) management. | <https://docs.aws.amazon.com/kms/latest/developerguide/> |
| Thu | 02/07/2026 | **Hands-on Data Encryption with KMS:**<br>&emsp;+ Create Customer Managed Key (CMK) in AWS KMS Console.<br>&emsp;+ **Hands-on practice:** Integrate KMS key to encrypt data on S3 Bucket, EBS Volume, and DynamoDB Table. | <https://docs.aws.amazon.com/kms/latest/developerguide/> |
| Fri | 03/07/2026 | **Review & Weekly Assessment:**<br>&emsp;+ Test ability to retrieve encrypted data from application.<br>&emsp;+ Review architecture diagram and task assignments, update Week 4 report. | <https://cloudjourney.awsstudygroup.com/> |

### Results achieved in Week 4:

* **Design & Task Assignment:**
  * Completed system architecture diagram on draw.io, clearly illustrating interactions between EC2, S3, DynamoDB, and security layers.
  * Detailed task assignments for each member and established shared workspace environment (Git, AWS IAM Roles/Users).

* **Encryption Key Management (AWS KMS):**
  * Mastered concepts of Cloud data encryption, Customer Managed Keys, and Key Policies.
  * Initialized Customer Managed Key (CMK) and established secure key access policies.
  * Applied KMS encryption to S3 Bucket, EBS Volume, and DynamoDB Table, ensuring data at rest is protected.
