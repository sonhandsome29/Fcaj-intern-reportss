---
title: "Tuần 6 - Xây API và dựng hạ tầng backend"
date: 2026-06-12
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Trọng tâm công việc
Tuần thứ sáu tập trung vào phần kỹ thuật cốt lõi của project, gồm phát triển backend và đồng thời triển khai hạ tầng mạng, cơ sở dữ liệu trên AWS để chuẩn bị cho giai đoạn đưa hệ thống lên môi trường cloud.

### Công việc thực hiện
1. Khởi tạo backend với Express, cấu hình các middleware cần thiết như CORS, logging và xử lý lỗi cơ bản.
2. Viết các API đầu tiên cho project và task để có thể kiểm tra luồng dữ liệu trước khi tích hợp frontend.
3. Tạo VPC, public subnet cho EC2 và private subnet cho RDS theo đúng sơ đồ đã chốt ở tuần trước.
4. Khởi tạo PostgreSQL trên Amazon RDS, thiết lập security group và kiểm tra logic kết nối từ phía ứng dụng.

### Kết quả đạt được
- Backend đã vượt qua giai đoạn khởi tạo ban đầu và có các API có thể sử dụng để kiểm thử.
- Hạ tầng cloud bắt đầu được triển khai bám sát nhu cầu của project thực tế.
- Việc kết hợp giữa code và cấu hình hạ tầng giúp quá trình phát triển có tính liên kết hơn.

### Tài liệu tham khảo
- [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsstudygroup.com/)
- [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsstudygroup.com/)
- [Building Microservices](https://000052.awsstudygroup.com/)
- [Data and Workflow Restructuring](https://000053.awsstudygroup.com/)
