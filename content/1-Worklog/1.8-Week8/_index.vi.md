---
title: "Worklog Tuần 8"
date: 2024-02-19
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Kiểm thử tổng thể (End-to-End Testing) và triển khai bản chính thức của dự án.
* Chạy thử nghiệm và rà soát tài liệu Workshop (Dry Run) đảm bảo chất lượng.
* Đóng gói toàn bộ tài nguyên dự án (mã nguồn, hạ tầng CloudFormation) và hoàn thiện bài hướng dẫn Workshop song ngữ (Tiếng Việt & Tiếng Anh) để nộp lên hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Ngày | Công việc | Nguồn tài liệu |
| --- | ---- | --------- | -------------- |
| 2 | 27/07/2026 | **Kiểm thử Tổng thể & Tải (End-to-End & Load Testing):**<br>&emsp;+ Kiểm thử toàn bộ hệ thống dưới tải giả lập (Load test Auto Scaling và Load Balancer).<br>&emsp;+ Rà soát lại log trên Amazon CloudWatch để phát hiện bất thường. |  |
| 3 | 28/07/2026 | **Triển khai Chính thức & Tối ưu Chi phí:**<br>&emsp;+ Khởi tạo bản hạ tầng chính thức (Production Deployment) qua CloudFormation.<br>&emsp;+ Dọn dẹp tài nguyên thừa, kiểm tra lại ngân sách trên AWS Budgets. |  |
| 4 | 29/07/2026 | **Thực tập tại công ty**<br>**Chạy thử nghiệm Workshop (Dry Run):**<br>&emsp;+ Các thành viên trong nhóm thực hiện lại bài lab Workshop theo kịch bản đã viết để phát hiện lỗi sót.<br>&emsp;+ Chỉnh sửa, hoàn thiện file hướng dẫn và mã nguồn dự án trên GitHub repository. |  |
| 5 | 30/07/2026 | **Đóng gói Tài nguyên & Biên dịch Song ngữ:**<br>&emsp;+ Đóng gói toàn bộ sản phẩm: Sơ đồ kiến trúc, Mẫu CloudFormation, Mã nguồn ứng dụng.<br>&emsp;+ Tối ưu hình thức, định dạng bài viết và hoàn thiện bản dịch bài Workshop (Tiếng Việt & Tiếng Anh). |  |
| 6 | 31/07/2026 | Kiểm tra lại toàn bộ tệp đính kèm và tài liệu bài viết, chính thức nộp bài Workshop và project đề tài lên hệ thống của chương trình. | |

### Kết quả đạt được tuần 8:

* **Hoàn thiện Dự án Đề tài:**
  * Triển khai bản chính thức Production bằng CloudFormation và đảm bảo hệ thống hoạt động ổn định.
  * Kiểm thử End-to-End và tải giả lập, đánh giá khả năng Auto Scaling và cân bằng tải của ALB.
  * Rà soát CloudWatch logs để phát hiện bất thường và hoàn thiện sửa lỗi trước khi bàn giao.

* **Tối ưu Chi phí & Quản lý tài nguyên:**
  * Dọn dẹp tài nguyên thừa và kiểm tra lại ngân sách trên AWS Budgets.
  * Điều chỉnh thiết lập để cân bằng chi phí vận hành và độ sẵn sàng dịch vụ.

* **Hoàn thiện Báo cáo & Workshop:**
  * Chuẩn bị tài liệu Workshop song ngữ (Tiếng Việt/Anh) và đóng gói toàn bộ mã nguồn, template hạ tầng.
  * Nộp bài dự án và tài liệu hoàn chỉnh lên hệ thống, đảm bảo cả nội dung và hình thức đều chỉnh chu.
