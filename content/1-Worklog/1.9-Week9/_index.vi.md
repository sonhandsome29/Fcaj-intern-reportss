---
title: "Tuần 9 - Ảnh, đăng nhập và trải nghiệm người dùng"
date: 2026-07-03
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Trọng tâm trong tuần
Tuần này tôi tập trung vào hai phần ảnh hưởng trực tiếp đến trải nghiệm người dùng: lưu trữ hình ảnh đúng cách và thêm cơ chế đăng ký, đăng nhập thay vì chỉ dùng dữ liệu cứng.

### Công việc đã thực hiện
1. Tạo S3 bucket để chứa ảnh và tài nguyên tĩnh, sau đó cập nhật lại đường dẫn trong frontend.
2. Khởi tạo Cognito User Pool, app client và các cấu hình xác thực cơ bản cho người dùng cuối.
3. Tích hợp Amplify UI để dựng nhanh giao diện sign up / sign in và giảm thời gian tự code form xác thực.
4. Kiểm thử luồng email verification và kiểm tra cách frontend lấy thông tin session sau khi đăng nhập thành công.

### Kết quả đạt được
- Giao diện không còn phụ thuộc vào ảnh local, giúp dễ deploy và dễ quản lý hơn.
- Hệ thống có lớp xác thực người dùng rõ ràng hơn, phù hợp với project management app.
- Đây là tuần làm cho sản phẩm “giống ứng dụng thật” hơn rất nhiều so với các tuần trước.

### Workshop tham khảo
- [Static Website Hosting with Amazon S3](https://000057.awsstudygroup.com/)
- [Serverless Storage and Auth with AWS Amplify](https://000134.awsstudygroup.com/)
- [User Authentication with Amazon Cognito](https://000081.awsstudygroup.com/)
- [Cross-Domain Authentication with Amazon Cognito](https://000141.awsstudygroup.com/)
- [Single Page Application Authentication](https://000055.awsstudygroup.com/)
