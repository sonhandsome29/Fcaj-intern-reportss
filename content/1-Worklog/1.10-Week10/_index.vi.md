---
title: "Tuần 10 - Tự động hóa, public deploy và tổng kết"
date: 2026-07-10
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Trọng tâm trong tuần
Tuần cuối cùng là giai đoạn hoàn thiện hệ thống theo hướng production hơn: tự động hóa một số luồng, khóa chặt phần bảo mật API, public frontend và rà soát lại toàn bộ project trước khi viết báo cáo.

### Công việc đã thực hiện
1. Tạo Lambda trigger để xử lý sau khi người dùng xác thực thành công, giúp đồng bộ thông tin cần thiết vào hệ thống backend.
2. Gắn Cognito authorizer cho API Gateway và cập nhật frontend để gửi JWT trong các request cần bảo vệ.
3. Deploy frontend lên Amplify, cấu hình branch, biến môi trường và kiểm tra lại luồng gọi API từ môi trường public.
4. Chạy test end-to-end, rà lỗi giao diện, bổ sung tài liệu workshop và tổng hợp phần báo cáo cuối kỳ.

### Kết quả đạt được
- Luồng đăng ký, xác thực và truy cập tài nguyên của hệ thống rõ ràng và chặt chẽ hơn.
- Frontend đã được public lên internet thay vì chỉ chạy local.
- Tôi kết thúc kỳ thực tập với một project hoàn chỉnh hơn cả về kỹ thuật lẫn tài liệu trình bày.

### Workshop tham khảo
- [Serverless Automation with AWS Lambda](https://000022.awsstudygroup.com/)
- [Single Page Application Authentication](https://000055.awsstudygroup.com/)
- [Frontend Integration with API Gateway](https://000135.awsstudygroup.com/)
- [CI/CD for Serverless Applications](https://000084.awsstudygroup.com/)
- [Serverless Storage and Auth with AWS Amplify](https://000134.awsstudygroup.com/)
