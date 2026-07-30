---
title: "Worklog Tuần 6"
date: 2024-02-05
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Báo cáo tiến độ triển khai hạ tầng dự án với Mentor và tiếp thu ý kiến đóng góp.
* Chỉnh sửa, tối ưu hóa và bổ sung các dịch vụ cần thiết vào mẫu CloudFormation template.
* Tìm hiểu và tích hợp dịch vụ mạng phân phối nội dung Amazon CloudFront (CDN) để tối ưu hiệu năng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 13/07/2026 | **Báo cáo Tiến độ Nhóm:**<br>&emsp;+ Báo cáo tiến độ triển khai hạ tầng và ứng dụng với Mentor/Đơn vị thực tập.<br>&emsp;+ Ghi nhận các góp ý về kiến trúc và yêu cầu tối ưu bổ sung. | <https://cloudjourney.awsstudygroup.com/> |
| 3 | 14/07/2026 | **Chỉnh sửa & Refactor Hạ tầng:**<br>&emsp;+ Cập nhật CloudFormation template theo phản hồi (tối ưu Security Group, tinh chỉnh tham số Auto Scaling).<br>&emsp;+ Cập nhật Change Set và kiểm thử lại hạ tầng. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| 4 | 15/07/2026 | **Tìm hiểu Amazon CloudFront (CDN):**<br>&emsp;+ Khái niệm CDN, Edge Locations, Origin, Caching Policy.<br>&emsp;+ Cơ chế bảo mật Origin Access Control (OAC) khi kết hợp CloudFront với S3. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 5 | 16/07/2026 | **Thực hành cấu hình Amazon CloudFront:**<br>&emsp;+ Tạo CloudFront Distribution kết hợp với S3 Bucket (cho tệp tĩnh) và ALB (cho động).<br>&emsp;+ Cấu hình Origin Access Control (OAC) để chặn truy cập trực tiếp vào S3 Bucket. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 6 | 17/07/2026 | **Kiểm thử Hiệu năng & Tổng kết:**<br>&emsp;+ Kiểm thử tốc độ tải trang trước và sau khi qua CloudFront (Latency / Bandwidth optimization).<br>&emsp;+ Bổ sung tài nguyên CloudFront vào CloudFormation template và hoàn thiện báo cáo tuần 6. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:

* **Tối ưu hóa Hạ tầng Dự án:**
  * Tiếp thu ý kiến đóng góp, refactor thành công mã nguồn CloudFormation giúp hạ tầng gọn nhẹ, bảo mật và dễ bảo trì hơn.

* **Phân phối Nội dung (Amazon CloudFront):**
  * Nắm vững nguyên lý hoạt động của CDN và mạng lưới Edge Location của AWS.
  * Tích hợp thành công Amazon CloudFront làm lớp đệm trước S3 Bucket và Load Balancer, giúp giảm độ trễ (latency) và tăng tốc độ tải trang.
  * Cấu hình an toàn Origin Access Control (OAC), đảm bảo người dùng chỉ có thể truy cập tài nguyên S3 thông qua CloudFront.