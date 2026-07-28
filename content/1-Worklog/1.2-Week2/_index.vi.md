---
title: "Worklog Tuần 2"
date: 2024-01-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Tìm hiểu về quản lý truy cập và bảo mật hệ thống thông qua AWS IAM.
* Tìm hiểu Infrastructure as Code (IaC) và thực hành triển khai tài nguyên tự động.
* Tìm hiểu cơ chế hoạt động của serverless với AWS Lambda và tích hợp cơ bản.
* 
### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 15/06/2026 | **Tìm hiểu về AWS IAM & Bảo mật:**<br>&emsp;+ Khái niệm IAM User, Group, Role, và Policy.<br>&emsp;+ Phân loại các loại IAM Role (Service Role, Cross-Account Role,...).<br>&emsp;+ Áp dụng nguyên tắc quyền tối thiểu (Principle of Least Privilege). | <https://cloudjourney.awsstudygroup.com/><br><https://docs.aws.amazon.com/IAM/latest/UserGuide/> |
| 3 | 16/06/2026 | **Thực tập tại công ty**<br>**Tìm hiểu Infrastructure as Code (IaC):**<br>&emsp;+ Tìm hiểu tổng quan về AWS CloudFormation và AWS CDK.<br>&emsp;+ **Thực hành:** Cấu trúc một template IaC đơn giản để khởi tạo tài nguyên cơ bản (VPC, Subnet, EC2 Instance). | <https://docs.aws.amazon.com/cloudformation/><br><https://docs.aws.amazon.com/cdk/v2/developerguide/> |
| 4 | 17/06/2026 | **Nghiên cứu dịch vụ Serverless AWS Lambda:**<br>&emsp;+ Khái niệm, kiến trúc và cách thiết lập Lambda Function.<br>&emsp;+ Tìm hiểu về Event Sources, Triggers và Execution Role.<br>&emsp;+ **Thực hành:** Tạo Lambda Function đơn giản kết nối với IAM Role và kiểm thử bằng Function URL / API Gateway. | <https://cloudjourney.awsstudygroup.com/><br><https://docs.aws.amazon.com/lambda/> |
| 5 | 18/06/2026 | **Tích hợp & Thực hành tổng hợp:**<br>&emsp;+ Kết hợp IAM Role + Lambda + CloudFormation để tự động hóa triển khai một luồng công việc nhỏ.<br>&emsp;+ Kiểm thử khả năng gán IAM Role cho máy chủ EC2 và Lambda Function. | <https://cloudjourney.awsstudygroup.com/> |
| 6 | 19/06/2026 | **Review & Tổng kết tuần:**<br>&emsp;+ Kiểm tra, tối ưu hóa các mẫu template CloudFormation đã viết.<br>&emsp;+ Gỡ lỗi (debug) các vấn đề liên quan đến phân quyền IAM Policy.<br>&emsp;+ Cập nhật tài liệu báo cáo Worklog Tuần 2. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 2:

* **Quản trị Bảo mật & Phân quyền (IAM):**
  * Hiểu rõ cơ chế hoạt động của IAM: User, Group, Role và Policy.
  * Phân biệt rõ ràng các loại Role (đặc biệt là Service Role cho EC2/Lambda) và áp dụng nguyên tắc quyền tối thiểu (Least Privilege) để cấp quyền an toàn.

* **Hạ tầng dưới dạng mã (IaC):**
  * Nắm được tự động hóa hạ tầng bằng IaC.
  * Xây dựng thành công mẫu template CloudFormation / CDK đơn giản để tự động khởi tạo VPC, Subnet và EC2 instance mà không cần thao tác thủ công trên Console.

* **Điện toán Serverless (AWS Lambda):**
  * Nắm vững cách thức hoạt động, vòng đời (lifecycle) và cơ chế kích hoạt (Triggers/Event Sources) của AWS Lambda.
  * Tạo và triển khai thành công một Lambda Function đơn giản, gán IAM Role phù hợp để giao tiếp với các dịch vụ AWS khác.