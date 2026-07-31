---
title: "Worklog Tuần 7"
date: 2024-02-12
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tiến hành kiểm thử tích hợp toàn bộ ứng dụng và hạ tầng của đề tài nhóm.
* Soạn thảo và hoàn thiện tài liệu hướng dẫn bài lab thực hành (Workshop Documentation).
* Tìm hiểu lý thuyết và thực hành cấu hình dịch vụ AWS WAF (Web Application Firewall) độc lập.

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 20/07/2026 | **Kiểm thử Tích hợp Project:**<br>&emsp;+ Kiểm thử luồng hoạt động end-to-end giữa Frontend, Backend, DynamoDB và S3.<br>&emsp;+ Rà soát và gỡ lỗi (debug) các kết nối API / Database của dự án. |  |
| 3 | 21/07/2026 | **Tìm hiểu lý thuyết AWS WAF:**<br>&emsp;+ Khái niệm Web ACL, Rules, Rule Groups.<br>&emsp;+ Các cơ chế phòng chống tấn công phổ biến trên ứng dụng web: SQL Injection (SQLi), Cross-Site Scripting (XSS), Rate-based (DDoS). | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| 4 | 22/07/2026 | **Thực hành AWS WAF:**<br>&emsp;+ Tạo Web ACL thử nghiệm và thêm các AWS Managed Rule Groups.<br>&emsp;+ **Thực hành:** Tạo môi trường kiểm thử riêng để gắn Web ACL và thử nghiệm khả năng chặn/mở lưu lượng truy cập. | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| 5 | 23/07/2026 | **Xây dựng Tài liệu Workshop:**<br>&emsp;+ Soạn thảo kịch bản từng bước (Step-by-step Lab Guide) cho bài Workshop thực hành của đề tài.<br>&emsp;+ Chụp hình minh họa và ghi chú các lưu ý kỹ thuật quan trọng. |  |
| 6 | 24/07/2026 | Kiểm tra tiến độ hoàn thiện tài liệu Workshop và tổng hợp báo cáo tuần 7. |  |

### Kết quả đạt được tuần 7:

* **Kiểm thử tích hợp hệ thống:**
  * Chạy thử toàn bộ luồng end-to-end giữa Frontend, Backend, DynamoDB và S3.
  * Rà soát và gỡ lỗi các kết nối API, cơ chế xác thực và luồng dữ liệu.

* **Tìm hiểu & Thực hành AWS WAF:**
  * Hiểu rõ Web ACL, Rule Group và cách thức lọc traffic Layer 7 của AWS WAF.
  * Thực hành tạo Web ACL và thêm AWS Managed Rule Groups chống SQLi, XSS, rate-based.
  * Kiểm thử khả năng chặn/mở request và đánh giá hiệu quả bảo vệ ứng dụng.

* **Xây dựng Tài liệu Workshop:**
  * Soạn thảo tài liệu thực hành chi tiết, bước-by-step, kèm hình ảnh minh họa và chú ý kỹ thuật.
  * Hoàn thiện bản thảo tài liệu Workshop để người khác có thể triển khai lại dự án từ đầu.
