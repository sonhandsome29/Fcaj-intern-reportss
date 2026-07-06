---
title : "Install Environment"
date : 2024-01-01 
weight : 2
chapter : false
pre : " <b> 5.4.2. </b> "
---

### Cài đặt môi trường và tải mã nguồn

Sau khi máy chủ đã chạy, chúng ta cần truy cập vào nó để cài đặt Node.js và lấy mã nguồn dự án từ GitHub.

**Step 1: Cài đặt Node.js, NPM và Git**
Trên Amazon Linux, chúng ta sử dụng trình quản lý gói `yum`. Chạy các lệnh sau để cập nhật hệ thống và cài đặt Node.js cùng với Git:

```bash
# Chuyển sang quyền root (giống trong video)
sudo su -

# Tải và cài đặt NVM (Node Version Manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# Kích hoạt NVM
. ~/.nvm/nvm.sh

# Cài đặt Node.js phiên bản 20 (hoặc bản bạn dùng local)
nvm install 20

# Cài đặt Git (Bắt buộc để clone code)
yum install git -y

# Kiểm tra lại phiên bản
node -v
npm -v
git --version
```

![Install Nodejs](/images/5-Workshop/5.4-AWS-EC2/install-nodejs.png)
![Install Nodejs](/images/5-Workshop/5.4-AWS-EC2/install-nodejs1.png)

**Step 2: Tải mã nguồn dự án**
Chúng ta sẽ sử dụng Git để lấy mã nguồn Backend về máy chủ.

```bash
# Clone dự án từ Github
git clone [https://github.com/Sazzazaa/project-management-aws.git](https://github.com/Sazzazaa/project-management-aws.git)

# Di chuyển vào thư mục dự án
cd project-management-aws/server

# Cài đặt các thư viện phụ thuộc
npm install
# Chạy thử để check
npm run dev
```

![Clone Repo](/images/5-Workshop/5.4-AWS-EC2/clone-repo.png)


**Step 3: Chuẩn bị file biến môi trường**
Ứng dụng Backend cần file `.env` để hoạt động. Chúng ta sẽ tạo file này dựa trên file mẫu.

```bash
# Tạo file môi trường
echo "PORT=80" > .env
```
![Config Env](/images/5-Workshop/5.4-AWS-EC2/config-env0.png)

![Config Env](/images/5-Workshop/5.4-AWS-EC2/config-env.png)


👉 **Bước tiếp theo:** Chúng ta sẽ chuyển sang phần **5.5. AWS RDS** để thiết lập Database, sau đó quay lại hoàn thiện file `.env` và khởi chạy Backend.