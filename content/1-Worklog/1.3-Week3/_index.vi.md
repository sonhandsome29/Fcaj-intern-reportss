---
title: "Tuần 3 - VPC và cơ sở dữ liệu được quản lý"
date: 2026-05-22
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Trọng tâm công việc
Tuần thứ ba đánh dấu bước chuyển từ các bài thực hành rời rạc sang tư duy kiến trúc hạ tầng, trong đó trọng tâm là phân lớp mạng, kiểm soát truy cập và đặt cơ sở dữ liệu vào vùng an toàn.

### Công việc thực hiện
1. Thiết kế VPC với public subnet cho EC2 và private subnet cho RDS để đảm bảo tách biệt frontend/backbone hạ tầng.
2. Làm quen với internet gateway, route table và cách route hoạt động giữa các subnet trong cùng một VPC.
3. Khởi tạo PostgreSQL trên Amazon RDS, cấu hình subnet group và security group phù hợp.
4. Tìm hiểu thêm về Route 53 theo hướng hybrid DNS để hiểu tư duy phân giải tên trong các môi trường thực tế.

### Kết quả đạt được
- Nắm rõ hơn nguyên tắc tách lớp mạng giữa khu vực public và private trong cùng một VPC.
- Hoàn thành bước cấu hình nền tảng cho việc kết nối EC2 với RDS theo hướng an toàn.
- Có thêm góc nhìn tổng quan về DNS và cách mở rộng hệ thống theo kiến trúc thực tế.

### Tài liệu tham khảo
- [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsstudygroup.com/)
- [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsstudygroup.com/)
- [Hybrid DNS Management with Amazon Route 53](https://000010.awsstudygroup.com/)
