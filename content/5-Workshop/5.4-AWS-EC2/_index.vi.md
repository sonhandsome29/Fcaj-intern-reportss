---
title : "Triển khai Backend (AWS EC2)"
date : 2024-01-01 
weight : 4
chapter : false
pre : " <b> 5.4. </b> "
---

### Triển khai Backend trên AWS EC2

Trong dự án này, hệ thống Backend (Node.js/Express) đóng vai trò xử lý logic nghiệp vụ và giao tiếp với cơ sở dữ liệu. Chúng ta sẽ sử dụng **Amazon Elastic Compute Cloud (Amazon EC2)** để làm máy chủ chạy ứng dụng này.

![EC2 Architecture](/images/5-Workshop/5.4-AWS-EC2/ec2-architecture.png)

#### Lý do lựa chọn dịch vụ
*   **Tính linh hoạt:** EC2 cung cấp quyền kiểm soát hoàn toàn (root access) đối với môi trường máy chủ, cho phép dễ dàng cài đặt Node.js, các thư viện cần thiết và cấu hình hệ thống theo đúng yêu cầu của framework.
*   **Chi phí tối ưu:** Bằng cách sử dụng instance type `t2.micro` hoặc `t3.micro`, chúng ta có thể tận dụng AWS Free Tier, giúp tiết kiệm chi phí tối đa trong quá trình phát triển và làm workshop.
*   **Khả năng tích hợp:** Dễ dàng nằm gọn trong kiến trúc VPC đã tạo, giao tiếp nội bộ an toàn với RDS và có thể đặt sau API Gateway.

#### Bố cục phần này
1. **Launch EC2 Instance:** Khởi tạo máy chủ ảo với các cấu hình mạng và bảo mật (Security Group) phù hợp.
2. **Install Environment:** Truy cập vào máy chủ, cài đặt môi trường Node.js và tải mã nguồn Backend.

*(Lưu ý: Theo phương pháp triển khai tăng dần (Iterative), sau khi tải mã nguồn, Backend sẽ chưa thể chạy ngay lập tức vì chúng ta cần khởi tạo Cơ sở dữ liệu RDS ở bước tiếp theo).*