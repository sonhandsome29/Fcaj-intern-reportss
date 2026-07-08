---
title: "Tuần 7 - Hoàn thiện giao diện và kết nối local"
date: 2026-06-19
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Trọng tâm trong tuần
Sau khi backend đã có dữ liệu cơ bản, tôi chuyển trọng tâm sang phần giao diện để biến project thành một sản phẩm có thể nhìn thấy, thao tác được và bắt đầu test luồng end-to-end ở local.

### Công việc đã thực hiện
1. Dựng khung frontend với Next.js, Tailwind CSS và các thành phần UI cần thiết cho dashboard.
2. Tích hợp RTK Query để chuẩn hóa cách gọi API thay vì fetch thủ công cho từng màn hình.
3. Xây dựng các trang chính như dashboard, board view, table view và timeline để mô phỏng bài toán quản lý dự án.
4. Ghép nối frontend với backend local, xử lý lỗi hydration, trạng thái loading và đồng bộ dữ liệu giữa các màn hình.

### Kết quả đạt được
- Project bắt đầu có cảm giác là một sản phẩm hoàn chỉnh hơn chứ không chỉ là backend chạy được.
- Tôi tiến bộ rõ ở phần tổ chức state, chia component và xử lý dữ liệu bất đồng bộ.
- Việc nối local API giúp tôi phát hiện bug sớm trước khi deploy lên AWS.

### Workshop tham khảo
- [Modernize the application Overview](https://cloudjourney.awsstudygroup.com/4-modernize/)
- [Single Page Application Authentication](https://000055.awsstudygroup.com/)
- [Frontend Development for Serverless APIs](https://000079.awsstudygroup.com/)
