---
title: "Worklog Tuần 4"
date: 2024-01-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Hoàn thiện sơ đồ kiến trúc hệ thống tổng thể và phân công nhiệm vụ chi tiết cho từng thành viên trong nhóm.
* Tìm hiểu dịch vụ quản lý khóa mã hóa AWS Key Management Service (KMS).
* Thực hành tạo khóa mã hóa và áp dụng bảo mật dữ liệu cho các dịch vụ AWS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 29/06/2026 | **Thiết kế Kiến trúc Hệ thống:**<br>&emsp;+ Hoàn thiện sơ đồ kiến trúc tổng thể chi tiết trên draw.io.<br>&emsp;+ Thảo luận và chốt luồng dữ liệu (Data flow) giữa các thành phần. | <https://cloudjourney.awsstudygroup.com/> |
| 3 | 30/06/2026 | **Phân công Nhiệm vụ Nhóm:**<br>&emsp;+ Họp nhóm phân chia module công việc chi tiết cho từng thành viên (Frontend, Backend, Infra/AWS).<br>&emsp;+ Thiết lập môi trường phát triển chung (Git repository, AWS IAM Accounts). | <https://cloudjourney.awsstudygroup.com/> |
| 4 | 01/07/2026 | **Tìm hiểu AWS KMS (Key Management Service):**<br>&emsp;+ Khái niệm KMS, AWS Managed Keys và Customer Managed Keys (CMK).<br>&emsp;+ Cơ chế mã hóa dữ liệu At-Rest (lưu trữ) và In-Transit (truyền tải).<br>&emsp;+ Quản lý chính sách truy cập khóa (Key Policies). | <https://docs.aws.amazon.com/kms/latest/developerguide/> |
| 5 | 02/07/2026 | **Thực hành mã hóa dữ liệu với KMS:**<br>&emsp;+ Tạo Customer Managed Key (CMK) trong AWS KMS Console.<br>&emsp;+ **Thực hành:** Tích hợp khóa KMS để mã hóa dữ liệu trên S3 Bucket, EBS Volume và DynamoDB Table. | <https://docs.aws.amazon.com/kms/latest/developerguide/> |
| 6 | 03/07/2026 | **Tổng kết & Đánh giá tuần:**<br>&emsp;+ Kiểm thử khả năng truy xuất dữ liệu đã mã hóa từ ứng dụng.<br>&emsp;+ Rà soát lại sơ đồ kiến trúc và phân công công việc, cập nhật báo cáo tuần 4. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:

* **Thiết kế & Phân công công việc:**
  * Hoàn thiện sơ đồ kiến trúc hệ thống chuẩn trên draw.io, thể hiện rõ tương tác giữa EC2, S3, DynamoDB và các lớp bảo mật.
  * Phân công công việc chi tiết cho từng thành viên, thiết lập xong môi trường làm việc chung (Git, AWS IAM Roles/Users).

* **Quản lý Khóa Mã hóa (AWS KMS):**
  * Nắm vững khái niệm về mã hóa dữ liệu trên Cloud và cách quản lý vòng đời của khóa mã hóa.
  * Khởi tạo thành công Customer Managed Key (CMK) và thiết lập Key Policy an toàn.
  * Áp dụng mã hóa KMS cho S3 Bucket, EBS Volume và DynamoDB Table, đảm bảo an toàn dữ liệu ở trạng thái lưu trữ (At-Rest).