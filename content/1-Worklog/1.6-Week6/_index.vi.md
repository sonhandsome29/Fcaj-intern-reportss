---
title: "Tuần 6 - Xây API và dựng hạ tầng backend"
date: 2026-06-12
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Trọng tâm trong tuần
Tôi bắt đầu bước vào phần kỹ thuật cốt lõi của project: vừa code backend, vừa dựng hạ tầng mạng và database trên AWS để chuẩn bị cho giai đoạn deploy thật.

### Công việc đã thực hiện
1. Khởi tạo backend với Express, cấu hình các middleware cần thiết như CORS, logging và xử lý lỗi cơ bản.
2. Viết các API đầu tiên cho project và task để có thể kiểm tra luồng dữ liệu trước khi tích hợp frontend.
3. Tạo VPC, public subnet cho EC2 và private subnet cho RDS theo đúng sơ đồ đã chốt ở tuần trước.
4. Khởi tạo PostgreSQL trên Amazon RDS, thiết lập security group và kiểm tra logic kết nối từ phía ứng dụng.

### Kết quả đạt được
- Backend không còn dừng ở mức skeleton mà đã có các endpoint dùng được.
- Hạ tầng cloud bắt đầu bám sát với nhu cầu thực tế của project thay vì chỉ là bài lab rời rạc.
- Tôi quen hơn với việc vừa phát triển chức năng, vừa kiểm tra tác động của cấu hình hạ tầng.

### Workshop tham khảo
- [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsstudygroup.com/)
- [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsstudygroup.com/)
- [Building Microservices](https://000052.awsstudygroup.com/)
- [Data and Workflow Restructuring](https://000053.awsstudygroup.com/)
