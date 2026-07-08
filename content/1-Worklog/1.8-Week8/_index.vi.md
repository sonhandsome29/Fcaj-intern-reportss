---
title: "Tuần 8 - Đưa backend lên EC2"
date: 2026-06-26
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Trọng tâm trong tuần
Đây là tuần tôi chuyển backend từ local sang môi trường cloud thật. Công việc không chỉ là chạy được server, mà còn phải giải quyết luôn bài toán tiến trình, cấu hình môi trường và đường đi HTTPS cho frontend.

### Công việc đã thực hiện
1. Tạo EC2 instance, cấu hình security group, SSH vào máy chủ và chuẩn bị môi trường chạy Node.js.
2. Clone source backend lên EC2, cài PM2 để giữ tiến trình chạy ổn định ngay cả khi thoát phiên SSH.
3. Đồng bộ biến môi trường, kết nối backend trên EC2 với RDS và kiểm tra lại luồng Prisma.
4. Tạo API Gateway để bọc phía ngoài backend EC2, xử lý vấn đề mixed content khi frontend public gọi API.

### Kết quả đạt được
- Backend đã chạy được ổn định trên EC2 thay vì chỉ hoạt động ở local.
- Tôi hiểu rõ hơn sự khác nhau giữa “code chạy” và “dịch vụ chạy ổn định”.
- API Gateway trở thành mắt xích quan trọng để frontend có thể giao tiếp an toàn với backend.

### Workshop tham khảo
- [Compute Essentials with Amazon Elastic Compute Cloud (EC2)](https://000004.awsstudygroup.com/)
- [Command Line Operations with AWS CLI](https://000011.awsstudygroup.com/)
- [Deploying Node.js Applications](https://000112.awsstudygroup.com/)
- [Frontend Integration with API Gateway](https://000135.awsstudygroup.com/)
