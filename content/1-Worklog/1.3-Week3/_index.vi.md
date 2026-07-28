---
title: "Worklog Tuần 3"
date: 2024-01-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Chốt chính thức đề tài, hoàn thiện sơ đồ kiến trúc tổng thể và phân công công việc chi tiết cho các thành viên trong nhóm.
* Nghiên cứu cơ chế tự động mở rộng quy mô (Auto Scaling) và cân bằng tải (Load Balancing) cho máy chủ ảo EC2.
* Tìm hiểu dịch vụ lưu trữ đối tượng Amazon S3 và hệ quản trị cơ sở dữ liệu NoSQL Amazon DynamoDB.
* Thực hành tích hợp S3 và DynamoDB với các dịch vụ tính toán (EC2 / AWS Lambda).

### Các công việc cần triển khai trong tuần này:
### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 22/06/2026 | **Họp nhóm - Chọn & Thống nhất đề tài:**<br>&emsp;+ Thảo luận các ý tưởng dự án, phân tích tính khả thi và thống nhất đề tài chính thức.<br>&emsp;+ Phác thảo sơ đồ kiến trúc hệ thống tổng thể trên draw.io. | <https://cloudjourney.awsstudygroup.com/> |
| 3 | 23/06/2026 | **Mở rộng quy mô với AWS EC2:**<br>&emsp;+ Tìm hiểu cơ chế Auto Scaling Group (ASG) và Elastic Load Balancing (ALB/NLB).<br>&emsp;+ Khái niệm AMI (Amazon Machine Image) và Launch Template.<br>&emsp;+ **Thực hành:** Tạo Launch Template, thiết lập Auto Scaling Group kết hợp ALB để tự động điều chỉnh số lượng EC2 instance theo tải. | <https://docs.aws.amazon.com/autoscaling/ec2/userguide/> |
| 4 | 24/06/2026 | **Dịch vụ lưu trữ Amazon S3:**<br>&emsp;+ Tìm hiểu khái niệm Bucket, Object, các lớp lưu trữ (Storage Classes) và Lifecycle Policies.<br>&emsp;+ Bảo mật S3: S3 Bucket Policy, Block Public Access và Access Control List (ACL).<br>&emsp;+ **Thực hành:** Tạo S3 Bucket, cấu hình phân quyền và lưu trữ tệp tĩnh (Static Website Hosting / Media Assets). | <https://docs.aws.amazon.com/AmazonS3/latest/userguide/> |
| 5 | 25/06/2026 | **Cơ sở dữ liệu NoSQL Amazon DynamoDB:**<br>&emsp;+ Khái niệm Table, Partition Key, Sort Key và Secondary Indexes (GSI/LSI).<br>&emsp;+ **Thực hành:** Khởi tạo bảng DynamoDB, thao tác dữ liệu (CRUD) thông qua AWS Management Console và AWS CLI/SDK. | <https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/> |
| 6 | 26/06/2026 | **Tích hợp & Tổng kết tuần:**<br>&emsp;+ **Thực hành tích hợp:** Viết ứng dụng trên EC2 / Lambda Function để đọc/ghi dữ liệu từ DynamoDB và lưu trữ file vào S3.<br>&emsp;+ Kiểm thử các dịch vụ đã triển khai và tổng hợp báo cáo tuần 3. | <https://cloudjourney.awsstudygroup.com/> |
### Kết quả đạt được tuần 3:

* **Đề tài nhóm:**
  * Thống nhất đề tài thực tập của nhóm.
  * Phác thảo và hoàn thiện sơ đồ kiến trúc hệ thống tổng thể trên *draw.io* để chuẩn bị cho bước phân công nhiệm vụ ở tuần tiếp theo.

* **Mở rộng Quy mô & Cân bằng tải (EC2 Scaling):**
  * Nắm vững nguyên lý hoạt động của Elastic Load Balancer (ALB) và Auto Scaling Group (ASG).
  * Khởi tạo thành công Launch Template và triển khai hệ thống EC2 có khả năng tự động tăng/giảm số lượng instance theo tải thực tế.

* **Lưu trữ Đối tượng (Amazon S3):**
  * Hiểu rõ cách tổ chức dữ liệu, cấu hình bảo mật (Bucket Policy) và quản lý vòng đời dữ liệu trên S3.
  * Triển khai thành công S3 Bucket phục vụ lưu trữ tài nguyên tĩnh và phân quyền truy cập an toàn.

* **Cơ sở dữ liệu NoSQL (Amazon DynamoDB):**
  * Hiểu tư duy thiết kế cơ sở dữ liệu NoSQL, cách chọn Partition Key và Sort Key tối ưu cho hiệu năng truy xuất.
  * Thao tác thành công các lệnh CRUD trên DynamoDB và kết nối thành công ứng dụng (EC2/Lambda) tới DynamoDB & S3 thông qua AWS SDK.