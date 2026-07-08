---
title: "Tuần 3 - VPC và cơ sở dữ liệu được quản lý"
date: 2026-05-22
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Trọng tâm trong tuần
Đây là tuần tôi bắt đầu nhìn hệ thống theo góc độ kiến trúc hạ tầng, không chỉ chạy được mà còn phải tách lớp mạng, kiểm soát truy cập và đặt database vào vị trí an toàn.

### Công việc đã thực hiện
1. Thiết kế VPC với public subnet cho EC2 và private subnet cho RDS để đảm bảo tách biệt frontend/backbone hạ tầng.
2. Làm quen với internet gateway, route table và cách route hoạt động giữa các subnet trong cùng một VPC.
3. Khởi tạo PostgreSQL trên Amazon RDS, cấu hình subnet group và security group phù hợp.
4. Tìm hiểu thêm về Route 53 theo hướng hybrid DNS để hiểu tư duy phân giải tên trong các môi trường thực tế.

### Kết quả đạt được
- Tôi hiểu rõ hơn vì sao database nên được đặt trong private subnet thay vì public.
- Tôi đã có nền tảng để kết nối EC2 với RDS một cách an toàn.
- Việc học Route 53 giúp tôi mở rộng góc nhìn từ một bài lab đơn lẻ sang bức tranh kiến trúc hoàn chỉnh hơn.

### Workshop tham khảo
- [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsstudygroup.com/)
- [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsstudygroup.com/)
- [Hybrid DNS Management with Amazon Route 53](https://000010.awsstudygroup.com/)
