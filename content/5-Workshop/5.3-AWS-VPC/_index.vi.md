---
title : "Thiết lập Mạng lưới ảo (AWS VPC)"
date : 2024-01-01 
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

### Cô lập tài nguyên mạng bằng VPC
*Isolating Network Resources with VPC*

Trong phần này, chúng ta sẽ tự tay khởi tạo một **Mạng riêng ảo (VPC)** từ đầu để cung cấp môi trường mạng an toàn cho toàn bộ dự án. Thay vì sử dụng Default VPC (VPC mặc định của AWS), chúng ta sẽ thiết kế một kiến trúc mạng phân tầng bao gồm: **Public Subnet** (mạng công cộng) dành cho máy chủ Backend (EC2) để có thể giao tiếp với mạng Internet thông qua **Internet Gateway**, và các **Private Subnets** (mạng nội bộ) dành riêng cho cơ sở dữ liệu (RDS) nhằm bảo vệ dữ liệu nghiệp vụ của hệ thống khỏi các truy cập trái phép từ bên ngoài.
*In this section, we will provision a custom **Virtual Private Cloud (VPC)** from scratch to provide a secure network environment for the entire project. Instead of using the AWS Default VPC, we will design a tiered network architecture comprising: a **Public Subnet** for the Backend server (EC2) to communicate with the Internet via an **Internet Gateway**, and **Private Subnets** dedicated to the database (RDS) to strictly protect business data from unauthorized external access.*

![VPC Architecture](/images/5-Workshop/5.3/vpc-architecture.png)
*(Lưu ý: Chèn sơ đồ VPC vào đây. Bạn có thể sử dụng công cụ draw.io hoặc dùng chính ảnh sơ đồ kiến trúc tổng quan ở file Proposal nhưng crop nhỏ lại, chỉ lấy phần khung viền màu xanh lá cây chứa VPC)*

#### Nội dung (Content)

- [Khởi tạo VPC & Subnets](5.3.1-create-vpc-subnets/)
- [Cấu hình Internet Gateway & Route Tables](5.3.2-igw-route-tables/)