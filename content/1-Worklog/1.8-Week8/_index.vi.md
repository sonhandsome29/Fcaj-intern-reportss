---
title: "Tuần 8 - Đưa backend lên EC2"
date: 2026-06-26
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Trọng tâm công việc
Tuần thứ tám tập trung vào việc chuyển backend từ môi trường local lên hạ tầng cloud thực tế. Bên cạnh việc đưa server chạy ổn định, tuần này còn xử lý luôn bài toán môi trường, tiến trình và đường đi HTTPS cho frontend.

### Công việc thực hiện
1. Tạo EC2 instance, cấu hình security group, SSH vào máy chủ và chuẩn bị môi trường chạy Node.js.
2. Clone source backend lên EC2, cài PM2 để giữ tiến trình chạy ổn định ngay cả khi thoát phiên SSH.
3. Đồng bộ biến môi trường, kết nối backend trên EC2 với RDS và kiểm tra lại luồng Prisma.
4. Tạo API Gateway để bọc phía ngoài backend EC2, xử lý vấn đề mixed content khi frontend public gọi API.

### Kết quả đạt được
- Backend đã được triển khai thành công lên EC2 và vận hành ổn định hơn so với môi trường local.
- Hiểu rõ hơn sự khác biệt giữa việc chạy được mã nguồn và vận hành được một dịch vụ thực tế.
- API Gateway được thiết lập thành công để hỗ trợ frontend kết nối an toàn tới backend.

### Tài liệu tham khảo
- [Compute Essentials with Amazon Elastic Compute Cloud (EC2)](https://000004.awsstudygroup.com/)
- [Command Line Operations with AWS CLI](https://000011.awsstudygroup.com/)
- [Deploying Node.js Applications](https://000112.awsstudygroup.com/)
- [Frontend Integration with API Gateway](https://000135.awsstudygroup.com/)
