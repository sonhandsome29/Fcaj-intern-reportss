---
title: "Tuần 2 - EC2, CLI và bài deploy đầu tiên"
date: 2026-05-15
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Trọng tâm trong tuần
Sau khi có tài khoản và quyền truy cập ổn định, tôi chuyển sang làm quen với máy chủ EC2, AWS CLI và cách đưa một tài nguyên tĩnh đầu tiên lên S3 để hiểu luồng triển khai cơ bản.

### Công việc đã thực hiện
1. Tạo EC2 instance, thực hành kết nối SSH và làm quen với các thao tác cơ bản trên máy chủ.
2. Cài đặt và sử dụng AWS CLI để kiểm tra thông tin tài nguyên, cấu hình thông tin truy cập và chạy lệnh trực tiếp từ môi trường thực hành.
3. Tìm hiểu sự khác nhau giữa IAM User và IAM Role, sau đó gắn role cho EC2 để truy cập dịch vụ AWS an toàn hơn.
4. Tạo S3 bucket và thử publish một website tĩnh đơn giản để hiểu cách lưu trữ file public trên AWS.

### Kết quả đạt được
- Tôi đã tự tin hơn khi thao tác với EC2 và môi trường dòng lệnh.
- Tôi hiểu vì sao nên dùng IAM Role thay vì hard-code access key trong ứng dụng.
- Việc deploy website tĩnh trên S3 giúp tôi hình dung rõ hơn về khái niệm hosting trên cloud.

### Workshop tham khảo
- [Compute Essentials with Amazon Elastic Compute Cloud (EC2)](https://000004.awsstudygroup.com/)
- [Command Line Operations with AWS CLI](https://000011.awsstudygroup.com/)
- [Instance Profiling with IAM Roles for EC2](https://000048.awsstudygroup.com/)
- [Static Website Hosting with Amazon S3](https://000057.awsstudygroup.com/)
