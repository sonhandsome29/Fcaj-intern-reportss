---
title : "Dọn dẹp tài nguyên"
date : 2026-07-08
weight : 9
chapter : false
pre : " <b> 5.9. </b> "
---

#### Dọn dẹp tài nguyên

Sau khi hoàn thành việc triển khai hệ thống **Project Management** trên AWS, bước dọn dẹp tài nguyên là việc nên làm để tránh phát sinh chi phí không cần thiết. Vì các dịch vụ trong project có liên kết với nhau, mình ưu tiên xóa theo thứ tự từ lớp bên ngoài như frontend và API, rồi mới đi dần vào backend, database và phần hạ tầng mạng. Cách làm này giúp hạn chế tình trạng một tài nguyên vẫn còn bị service khác tham chiếu nên chưa thể xóa ngay.

#### Thứ tự thực hiện khuyến nghị

1. **Gỡ frontend trên AWS Amplify**

   Trước tiên, vào **AWS Amplify** và kiểm tra ứng dụng frontend của project-management đã deploy. Nếu không còn nhu cầu giữ bản demo public nữa, có thể xóa branch đang dùng hoặc xóa toàn bộ hosting app.

2. **Xóa cấu hình xác thực trên Amazon Cognito**

   Tiếp theo, vào **Amazon Cognito** để rà soát lại phần đăng nhập của hệ thống:

   - User Pool đã tạo cho project
   - App Client đi kèm
   - Các user test đã dùng trong quá trình kiểm thử

   Nếu không có ý định dùng lại luồng xác thực này, có thể xóa toàn bộ User Pool để tránh giữ lại những cấu hình không còn giá trị sử dụng.

3. **Xóa API trên Amazon API Gateway**

   Sau đó, mở **API Gateway** và xóa phần public endpoint đã tạo cho backend:

   - HTTP API hoặc REST API đã tạo
   - Stage deploy liên quan
   - Cognito Authorizer nếu được tạo riêng cho project

4. **Xóa Lambda Trigger**

   Trong project này, Lambda được dùng để xử lý sau khi user xác thực thành công. Trước khi xóa function, nên:

   - Gỡ trigger ra khỏi User Pool
   - Kiểm tra lại permission hoặc mapping liên quan
   - Xóa Lambda function nếu không còn dùng nữa

5. **Dừng và xóa EC2 backend**

   Sau khi frontend, auth và API public đã được gỡ, vào **EC2 Console** để xử lý máy chủ backend:

   - Stop instance để kiểm tra lần cuối
   - Terminate instance backend nếu không còn nhu cầu giữ lại
   - Release Elastic IP nếu trước đó có gán riêng
   - Xóa key pair trên AWS nếu xác định không dùng lại

6. **Xóa cơ sở dữ liệu Amazon RDS**

   Tiếp theo là phần **Amazon RDS**, nơi đang chứa dữ liệu của hệ thống Project Management. Trước khi xóa database, nên cân nhắc:

   - **Giữ final snapshot** nếu vẫn muốn lưu lại dữ liệu để đối chiếu hoặc demo sau này
   - **Không giữ snapshot** nếu đây chỉ là môi trường thực hành và không còn nhu cầu khôi phục

   Khi đã xác định rõ phương án, tiến hành xóa database instance.

7. **Xóa S3 bucket lưu hình ảnh**

   Ở phần **Amazon S3**, project này có dùng bucket để lưu ảnh hoặc static assets. Với bucket như `project-management-images-aws`, nên dọn theo thứ tự:

   - Xóa toàn bộ object trong bucket
   - Xác nhận bucket rỗng
   - Xóa bucket chứa ảnh hoặc static assets của project

8. **Xóa Security Group và tài nguyên mạng phụ trợ**

   Khi EC2, RDS và các service bên ngoài đã được dọn, có thể quay lại xóa các tài nguyên mạng phụ trợ:

   - Security Group dùng riêng cho EC2
   - Security Group dùng riêng cho RDS
   - DB subnet group nếu đã tạo riêng cho workshop này

9. **Xóa subnet, route table, internet gateway và VPC**

   Cuối cùng, nếu toàn bộ VPC này chỉ phục vụ cho project-management workshop, có thể xóa theo đúng thứ tự để tránh báo lỗi phụ thuộc:

   - Subnet
   - Route table tùy chỉnh
   - Internet Gateway (detach trước, rồi delete)
   - VPC

#### Lưu ý cuối cùng

Trước khi xóa hoàn toàn tài nguyên, mình nên chắc rằng đã lưu lại đầy đủ các nội dung cần giữ cho báo cáo:

- Source code cuối cùng
- Ảnh chụp màn hình để viết báo cáo
- Link demo, thông tin cấu hình quan trọng hoặc file `.env` mẫu nếu cần đối chiếu sau này
