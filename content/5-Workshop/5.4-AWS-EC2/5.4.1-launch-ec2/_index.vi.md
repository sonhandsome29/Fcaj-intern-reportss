---
title : "Launch EC2"
date : 2024-01-01 
weight : 1
chapter : false
pre : " <b> 5.4.1. </b> "
---

### Khởi tạo máy chủ ảo

Bước này hướng dẫn cách tạo một máy chủ EC2, gắn nó vào mạng VPC đã tạo ở bước 5.3 và cấu hình tường lửa (Security Group) đảm bảo nguyên tắc bảo mật.

**Step 1: Truy cập EC2 Dashboard**
1. Đăng nhập vào AWS Management Console.
2. Tìm kiếm **EC2** trên thanh tìm kiếm và chọn dịch vụ EC2.
3. Nhấp vào nút **Launch instance**.

![Access EC2](/images/5-Workshop/5.4-AWS-EC2/access-ec2.png)

**Step 2: Cấu hình cơ bản**
1. **Name:** Nhập tên cho máy chủ, ví dụ: `pm_ec2-backend`.
2. **Application and OS Images (Amazon Machine Image):** Chọn **Amazon Linux**, version *Amazon Linux 2023 AMI* (hoặc Amazon Linux 2).
3. **Instance type:** Chọn **t2.micro**.

![Config EC2 OS](/images/5-Workshop/5.4-AWS-EC2/config-os.png)

**Step 3: Cấu hình Key pair**
1. Ở mục **Key pair (login)**, chọn **Create new key pair**.
2. Nhập tên Key pair name (ví dụ: `fcj-workshop-key`).
3. Key pair type: **RSA**. Private key file format: **.pem** (nếu dùng Mac/Linux) hoặc **.ppk** (nếu dùng Windows/PuTTY).
4. Nhấp **Create key pair** và lưu file này ở nơi an toàn trên máy tính của bạn.

![Create Key Pair](/images/5-Workshop/5.4-AWS-EC2/create-key-pair.png)

**Step 4: Cấu hình Mạng & Bảo mật**
1. Ở mục **Network settings**, nhấp vào **Edit**.
2. **VPC:** Chọn VPC mà bạn đã tạo ở phần 5.3.
3. **Subnet:** Chọn một **Public Subnet** để máy chủ có thể truy cập được từ Internet (Cần thiết cho quá trình cài đặt).
4. **Auto-assign public IP:** Đổi thành **Enable**.
5. **Firewall (security groups):** Chọn **Create security group**.
    * **Security group name:** `pm_ec2-sg`

![Config Security Group](/images/5-Workshop/5.4-AWS-EC2/config-sg.png)


**Step 5: Khởi chạy**
1. Phần **Configure storage** giữ nguyên mặc định là 8GB gp3.
2. Kiểm tra lại thông tin ở khung **Summary** bên phải.
3. Nhấp **Launch instance**. Chờ vài phút để trạng thái của máy chủ chuyển sang **Running**.

![Launch Summary](/images/5-Workshop/5.4-AWS-EC2/launch-summary.png)
