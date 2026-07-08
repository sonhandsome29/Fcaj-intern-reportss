---
title: "Tuần 9 - Ảnh, đăng nhập và trải nghiệm người dùng"
date: 2026-07-03
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Trọng tâm công việc
Tuần thứ chín tập trung vào hai thành phần có ảnh hưởng trực tiếp tới trải nghiệm người dùng: cơ chế lưu trữ hình ảnh và hệ thống xác thực tài khoản.

### Công việc thực hiện
1. Tạo S3 bucket để chứa ảnh và tài nguyên tĩnh, sau đó cập nhật lại đường dẫn trong frontend.
2. Khởi tạo Cognito User Pool, app client và các cấu hình xác thực cơ bản cho người dùng cuối.
3. Tích hợp Amplify UI để dựng nhanh giao diện sign up / sign in và giảm thời gian tự code form xác thực.
4. Kiểm thử luồng email verification và kiểm tra cách frontend lấy thông tin session sau khi đăng nhập thành công.

### Kết quả đạt được
- Hoàn tất việc chuyển tài nguyên hình ảnh sang S3 để thuận tiện cho quản lý và triển khai.
- Thiết lập được lớp xác thực người dùng phù hợp hơn với mô hình ứng dụng quản lý dự án.
- Giao diện và trải nghiệm sử dụng của hệ thống tiến gần hơn tới một ứng dụng hoàn chỉnh.

### Tài liệu tham khảo
- [Static Website Hosting with Amazon S3](https://000057.awsstudygroup.com/)
- [Serverless Storage and Auth with AWS Amplify](https://000134.awsstudygroup.com/)
- [User Authentication with Amazon Cognito](https://000081.awsstudygroup.com/)
- [Cross-Domain Authentication with Amazon Cognito](https://000141.awsstudygroup.com/)
- [Single Page Application Authentication](https://000055.awsstudygroup.com/)
