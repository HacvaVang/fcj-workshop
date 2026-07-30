---
title: "Event 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Bài thu hoạch "FCAJ x Agentic AI Build Week"

### Mục Đích Của Sự Kiện
- Chia sẻ best practices trong thiết kế ứng dụng hiện đại và tích hợp Agentic AI vào quy trình vận hành.
- Chia sẻ văn hóa công ty, tư duy đổi mới sáng tạo và trải nghiệm thực tế từ các doanh nghiệp/chuyên gia lớn (như AWS).
- Tạo sân chơi thực hành kỹ thuật, thúc đẩy đổi mới sáng tạo và giải quyết các bài toán thực tế của doanh nghiệp bằng công nghệ AI.

---

### Danh Sách Diễn Giả
- **Mr. Nguyễn Gia Hưng**: Head of Solution Architect, AWS Vietnam.
- **Mr. Joseph Marazota**: Head of Technology, AWS ASEAN.
- **One Team**: Đội thắng cuộc AABW Hackathon.
- **Signal Scout**: Đội Á quân AABW Hackathon.
- **Plan V**: Đội tham gia cuộc thi AABW Hackathon.
- **3KA**: Đội tham gia cuộc thi AABW Hackathon.
- **Six Pillar Team**: Đội tham gia cuộc thi AABW Hackathon.

---

### Nội Dung Nổi Bật

#### AI-Powered Conversation Ordering
- **Bài toán**: Các giải pháp đặt đồ ăn bằng AI hiện tại dễ phát sinh lỗi khi xử lý ngôn ngữ tự nhiên, làm khách hàng thất vọng. Đồng thời, việc chuyển đổi kênh từ chat sang tải app tạo ra ma sát (friction) và mất tương tác.
- **Giải pháp**: Xây dựng Agent AI hội thoại đa kênh trên Zalo/WhatsApp, tương tác tự nhiên, xác nhận đơn hàng rõ ràng để tránh nhầm lẫn.
- **Kiến trúc & Công nghệ**: Sử dụng AI web scraping (Tiny Fish, Abify) thu thập menu/khuyến mãi từ KFC; kiến trúc modular dễ thay đổi logic kinh doanh; AI Agent có bộ nhớ phiên (session memory).
- **Chi phí & Hiệu năng**: Độ trễ 0.3 - 0.4s, chi phí hạ tầng ~$88/tháng (~$0.006/đơn hàng), tiết kiệm 60% chi phí hạ tầng nhờ tối ưu thiết kế.

#### Solutional Architect Profressional Native App
- **Bài toán**: Giải quyết áp lực cho các Cloud Solution Architects (SA) khi phải thiết kế, báo giá và triển khai hạ tầng nhanh chóng trong vòng vài giờ.
- **Giải pháp**: Ứng dụng AI-native tự động hóa vẽ kiến trúc, tính giá và sinh mã Infrastructure as Code (Terraform, CloudFormation) qua tương tác ngôn ngữ tự nhiên hoặc tài liệu kinh doanh.
- **Điểm nổi bật**: Hỗ trợ Blacklist validation lọc dịch vụ không cho phép, có khả năng giải thích lý do thiết kế (stepwise reasoning) và tái sử dụng các module IaC.

#### Build a production-ready AI application using AWS AI/ML
- **Tích hợp dịch vụ AWS**: Sử dụng các giải pháp như AWS Amplify, Cognito, Lambda, Fargate, S3, DynamoDB để đảm bảo tính sẵn sàng sản xuất (production-ready).
- **Ứng dụng Multi-Agent System**: Kết hợp các agent crawler, agent lọc nhiễu, agent phân tích/chấm điểm và nhân sự kiểm duyệt (Human-in-the-loop).
- **Phân tích chiến lược doanh nghiệp**: Nhanh chóng cào và phân tích dữ liệu đối thủ cạnh tranh từ báo cáo tài chính và website, dự báo tác động chiến lược với chi phí $35 - $130/tháng.

#### Smart Human-flow Evaluation, Prediction, Hazard Detection, Response and Dispatch (S.H.E.P.H.R.D)
- **Bài toán**: Quản lý ùn tắc đám đông tại sân bay, sự kiện, cửa hàng bán lẻ đòi hỏi sự chủ động thay vì giám sát thủ công.
- **Giải pháp**: Hệ thống phân tích video thời gian thực kết hợp Edge Computing và AWS Cloud.
- **Mô hình & Kiến trúc**: Sử dụng mô hình YOLO v2.6 Small để phát hiện và theo dõi người theo từng khu vực (zonal tracking); luồng dữ liệu truyền vào AWS Fargate, lưu trữ tại DynamoDB/S3.
- **Chức năng**: Tính toán thời gian chờ, gợi ý biện pháp điều tiết, phát cảnh báo tự động và hỗ trợ người vận hành can thiệp (Operator Cockpit).

#### Adaptive AML Workflow Engine
- **Bài toán**: Lĩnh vực tài chính gặp lượng lớn cảnh báo giao dịch đáng ngờ nhưng có tới 90-95% là dương tính giả (false positives). Quy trình thủ công tốn thời gian và chi phí.
- **Giải pháp**: Động cơ AI tối ưu hóa quy trình điều tra cảnh báo chống rửa tiền (AML), tự động thu thập và tổng hợp dữ liệu từ nhiều nguồn (lich sử giao dịch, KYC, screening).
- **Hiệu quả**: Giảm thời gian xử lý từ vài ngày/giờ xuống còn vài phút, cung cấp nhật ký bằng chứng có thể truy xuất nguồn gốc (auditability & explainability) mà không thay đổi vai trò quyết định của con người.

#### Trải nghiệm khi tham gia Hackathon
- **Làm việc dưới áp lực thời gian**: Thử thách kéo dài đến 3-4 giờ sáng, yêu cầu tinh thần giải quyết vấn đề nhanh chóng.
- **Xây dựng MVP & Demo**: Nhấn mạnh việc tập trung vào bài toán cốt lõi, phạm vi thực tế (scope control) và chuẩn bị demo chạy trực tiếp thay vì chỉ trình bày lý thuyết.
- **Quản lý xung đột & Giao tiếp**: Đội ngũ đa dạng ngôn ngữ, kỹ năng cần lắng nghe, phân công vai trò rõ ràng và thống nhất mục tiêu chung để vượt qua bất đồng.

---

### Những Gì Học Được
- **Tư duy thiết kế sản phẩm AI**: Cần tập trung 70%+ vào việc giải quyết bài toán kinh doanh thực tế (business use case) hơn là chỉ phô diễn công nghệ thuần túy.
- **Ứng dụng Multi-Agent & Human-in-the-loop**: Kết hợp linh hoạt nhiều Agent chuyên biệt và giữ yếu tố con người can thiệp ở các trường hợp độ tin cậy thấp (low confidence).
- **Tối ưu hóa chi phí & Hiệu năng**: Kỹ thuật thiết kế hệ thống giúp giảm tới 60% chi phí vận hành AI, tận dụng kiến trúc serverless (Lambda, Fargate).
- **Kỹ năng mềm**: Bài học về làm việc nhóm dưới áp lực cao, quản lý scope dự án, và kỹ năng thuyết trình/trả lời Q&A trước ban giám khảo.

---

### Ứng Dụng Vào Công Việc
- **Tự động hóa quy trình nghiệp vụ**: Áp dụng mô hình AI Agent vào việc tự động tổng hợp dữ liệu, trích xuất thông tin tài liệu và tạo báo cáo tự động.
- **Tối ưu hóa thiết kế hệ thống**: Sử dụng các nguyên tắc kiến trúc Cloud/AI từ AWS để xây dựng giải pháp có khả năng mở rộng tốt và tiết kiệm chi phí.
- **Cải thiện trải nghiệm khách hàng**: Nghiên cứu tích hợp AI hội thoại có bộ nhớ (session memory) vào các kênh tương tác trực tiếp với người dùng mà không bắt họ chuyển đổi ứng dụng.

---

### Trải nghiệm trong event

#### Học hỏi từ các diễn giả có chuyên môn cao
- Nhận được những chia sẻ tầm nhìn chiến lược từ Mr. Joseph Marazota và Mr. Nguyễn Gia Hưng về xu hướng dịch chuyển từ chu kỳ phát hành theo quý sang phát hành liên tục theo phút, cùng vai trò của AI trong tái hình thành các ngành công nghiệp.

#### Trải nghiệm kỹ thuật thực tế
- Tiếp cận trực tiếp với các giải pháp kỹ thuật tiên tiến: YOLO v2.6 cho xử lý video thời gian thực, Multi-Agent workflow, AI scraping (Tiny Fish), tự động sinh IaC (Terraform/CloudFormation).

#### Ứng dụng công cụ hiện đại
- Trải nghiệm việc tích hợp các dịch vụ hàng đầu của AWS (Amplify, Cognito, Lambda, Fargate, DynamoDB, S3) cùng các mô hình AI/ML hiện đại để xây dựng sản phẩm production-ready.

#### Kết nối và trao đổi
- Mở rộng mạng lưới kết nối (networking) với các chuyên gia, diễn giả hàng đầu từ AWS cùng các bạn trẻ đam mê công nghệ năng động trong cộng đồng AI tại TP.HCM.

#### Bài học rút ra
- Luôn giữ tinh thần học hỏi liên tục (continuous learning), chấp nhận rủi ro, không ngại thử thách tại các cuộc thi hackathon. Dù ý tưởng tốt đến đâu, việc tập trung vào một MVP thực thi được và giải quyết đúng nhu cầu người dùng mới là yếu tố quyết định thành công.

#### Một số hình ảnh khi tham gia sự kiện
![Event picture 1](/fcj-workshop/images/4-Events/event-3.1.jpg)
![Event picture 2](/fcj-workshop/images/4-Events/event-3.2.jpg)