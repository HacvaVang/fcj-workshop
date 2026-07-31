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
| 2 | 13/07/2026 | **Thực tập tại công ty**<br>**Báo cáo Tiến độ Nhóm:**<br>&emsp;+ Báo cáo tiến độ triển khai hạ tầng và ứng dụng với Mentor/Đơn vị thực tập.<br>&emsp;+ Ghi nhận các góp ý về kiến trúc và yêu cầu tối ưu bổ sung. | <https://cloudjourney.awsstudygroup.com/> |
| 3 | 14/07/2026 | **Chỉnh sửa & Refactor Hạ tầng:**<br>&emsp;+ Cập nhật CloudFormation template theo phản hồi (tối ưu Security Group, tinh chỉnh tham số Auto Scaling).<br>&emsp;+ Cập nhật Change Set và kiểm thử lại hạ tầng. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| 4 | 15/07/2026 | **Tìm hiểu Amazon CloudFront (CDN):**<br>&emsp;+ Khái niệm CDN, Edge Locations, Origin, Caching Policy.<br>&emsp;+ Cơ chế bảo mật Origin Access Control (OAC) khi kết hợp CloudFront với S3. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 5 | 16/07/2026 | **Thực hành cấu hình Amazon CloudFront:**<br>&emsp;+ Tạo CloudFront Distribution kết hợp với S3 Bucket (cho tệp tĩnh) và ALB (cho động).<br>&emsp;+ Cấu hình Origin Access Control (OAC) để chặn truy cập trực tiếp vào S3 Bucket. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 6 | 17/07/2026 | **Kiểm thử Hiệu năng & Tổng kết:**<br>&emsp;+ Kiểm thử tốc độ tải trang trước và sau khi qua CloudFront (Latency / Bandwidth optimization).<br>&emsp;+ Bổ sung tài nguyên CloudFront vào CloudFormation template và hoàn thiện báo cáo tuần 6. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:

* **Tối ưu hóa Hạ tầng Dự án:**
  * Refactor thành công CloudFormation template, giảm bớt cấu hình thừa, chuẩn hóa tham số và nâng cao khả năng mở rộng.
  * Cập nhật Security Group để chỉ mở các cổng cần thiết, tinh chỉnh chính sách truy cập giữa ALB và EC2, giúp giảm bề mặt tấn công và tăng tính bảo mật.
  * Điều chỉnh tham số Auto Scaling Group (số lượng tối thiểu/tối đa, chính sách scaling) để cân bằng chi phí và hiệu năng trong môi trường thực tập.
  * Bổ sung CloudFront vào template và tạo Change Set kiểm thử cập nhật hạ tầng một cách an toàn.

* **Phân phối Nội dung (Amazon CloudFront):**
  * Hiểu rõ nguyên lý CDN, caching, chế độ Origin, Edge Locations và hệ thống phân phối nội dung của AWS.
  * Triển khai thành công CloudFront Distribution cho cả tệp tĩnh trên S3 và dịch vụ động qua ALB.
  * Cấu hình Origin Access Control (OAC) kết hợp S3 Origin, đảm bảo truy cập S3 chỉ qua CloudFront, tăng cường bảo mật dữ liệu tĩnh.
  * Định nghĩa chính sách cache phù hợp cho nội dung tĩnh, giúp giảm tải trực tiếp lên S3 và cải thiện tốc độ tải trang cho người dùng toàn cầu.
  * Kiểm thử hiệu năng trước và sau khi sử dụng CloudFront, xác định giảm độ trễ, tăng tốc độ duyệt trang và tối ưu băng thông cho nội dung tĩnh.
