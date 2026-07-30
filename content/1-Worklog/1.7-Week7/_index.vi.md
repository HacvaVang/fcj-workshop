---
title: "Worklog Tuần 7"
date: 2024-02-12
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tiến hành kiểm thử tích hợp toàn bộ ứng dụng và hạ tầng của đề tài.
* Tìm hiểu và nâng cao bảo mật ứng dụng web với AWS WAF (Web Application Firewall).
* Soạn thảo và hoàn thiện tài liệu hướng dẫn bài lab thực hành (Workshop Documentation).

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 20/07/2026 | **Kiểm thử Tích hợp (Integration Testing):**<br>&emsp;+ Kiểm thử luồng hoạt động end-to-end giữa Frontend, Backend, DynamoDB và S3.<br>&emsp;+ Rà soát và gỡ lỗi (debug) các kết nối API / Database. | <https://cloudjourney.awsstudygroup.com/> |
| 3 | 21/07/2026 | **Tìm hiểu về AWS WAF:**<br>&emsp;+ Khái niệm Web ACL, Rules, Rule Groups.<br>&emsp;+ Các cơ chế phòng chống tấn công phổ biến: SQL Injection, Cross-Site Scripting (XSS), Rate-based (DDoS). | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| 4 | 22/07/2026 | **Thực hành cấu hình AWS WAF:**<br>&emsp;+ Tạo Web ACL và thêm các AWS Managed Rule Groups.<br>&emsp;+ **Thực hành:** Đính kèm Web ACL vào CloudFront Distribution và Application Load Balancer (ALB). | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| 5 | 23/07/2026 | **Xây dựng Tài liệu Workshop:**<br>&emsp;+ Soạn thảo kịch bản từng bước (Step-by-step Lab Guide) cho bài Workshop thực hành của đề tài.<br>&emsp;+ Chụp hình minh họa và ghi chú các lưu ý kỹ thuật quan trọng. | <https://cloudjourney.awsstudygroup.com/> |
| 6 | 24/07/2026 | **Kiểm thử Bảo mật & Tổng kết tuần:**<br>&emsp;+ Giả lập các cuộc tấn công đơn giản (IP Rate Limit, Bad Bot) để kiểm thử phản ứng của AWS WAF.<br>&emsp;+ Đánh giá mức độ hoàn thiện tài liệu Workshop và tổng hợp báo cáo tuần 7. | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 7:

* **Kiểm thử Hệ thống:**
  * Toàn bộ luồng hoạt động của dự án đã chạy ổn định trên hạ tầng AWS, các dịch vụ kết nối với nhau mượt mà và an toàn.

* **Bảo mật Ứng dụng Web (AWS WAF):**
  * Hiểu rõ cơ chế lọc traffic và bảo mật lớp ứng dụng (Layer 7).
  * Triển khai thành công AWS WAF gắn liền với CloudFront/ALB, kích hoạt các bộ quy tắc bảo mật chống SQLi, XSS và giới hạn tần suất truy cập (Rate Limiting).

* **Xây dựng Tài liệu Workshop:**
  * Hoàn thiện bộ tài liệu hướng dẫn thực hành Workshop chi tiết, rõ ràng, giúp người đọc có thể tự triển khai lại toàn bộ dự án từ đầu.