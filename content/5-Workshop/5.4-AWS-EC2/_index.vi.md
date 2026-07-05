---
title : "Triển khai Máy chủ Backend (AWS EC2)"
date : 2024-01-01 
weight : 4
chapter : false
pre : " <b> 5.4. </b> "
---

### Lưu trữ ứng dụng với Amazon EC2

Trong phần này, chúng ta sẽ khởi chạy một máy chủ ảo **Amazon EC2 (Elastic Compute Cloud)** để làm môi trường chạy mã nguồn Backend (Node.js) cho dự án. Máy chủ này sẽ được đặt bên trong **Public Subnet** của VPC mà chúng ta vừa tạo, cho phép nó nhận các yêu cầu (requests) từ người dùng ngoài Internet thông qua cổng HTTP/HTTPS, đồng thời có thể giao tiếp an toàn với cơ sở dữ liệu ở Private Subnet.

![EC2 Architecture](/images/5-Workshop/5.4/ec2-architecture.png)
*(Lưu ý: Chèn sơ đồ kiến trúc EC2 vào đây. Bạn có thể dùng Draw.io, lấy sơ đồ VPC ở phần trước và vẽ thêm icon EC2 vào bên trong khung Public Subnet).*

#### Nội dung (Content)

- [Khởi chạy EC2 Instance & Security Group](5.4.1-launch-ec2/)
- [Cài đặt Node.js & PM2 qua SSH](5.4.2-install-env/)