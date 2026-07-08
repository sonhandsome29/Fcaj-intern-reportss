---
title : "Dọn dẹp tài nguyên"
date : 2026-07-10
weight : 9
chapter : false
pre : " <b> 5.9. </b> "
---

#### Dọn dẹp tài nguyên

Sau khi hoàn thành workshop triển khai hệ thống Project Management trên AWS, bạn nên dọn dẹp toàn bộ tài nguyên để tránh phát sinh chi phí không cần thiết. Thứ tự xóa dưới đây được sắp xếp theo hướng an toàn, hạn chế lỗi phụ thuộc giữa các dịch vụ.

#### Thứ tự khuyến nghị

1. **Gỡ frontend trên AWS Amplify**

   Mở **AWS Amplify** và chọn app đã deploy. Nếu không cần giữ môi trường demo nữa, hãy xóa branch đang dùng hoặc xóa toàn bộ app hosting.

2. **Xóa cấu hình xác thực trên Amazon Cognito**

   Vào **Amazon Cognito** và kiểm tra:

   - User Pool đã tạo cho project
   - App Client đi kèm
   - Các user test không còn cần dùng

   Nếu không cần tái sử dụng, hãy xóa toàn bộ User Pool để tránh giữ cấu hình xác thực dư thừa.

3. **Xóa API trên Amazon API Gateway**

   Vào **API Gateway** và xóa:

   - HTTP API hoặc REST API đã tạo
   - Stage deploy liên quan
   - Authorizer nếu được tạo riêng cho bài lab

4. **Xóa Lambda Trigger**

   Nếu bạn đã tạo Lambda để xử lý post-confirmation hoặc trigger khác từ Cognito, hãy:

   - Gỡ trigger ra khỏi User Pool
   - Xóa function Lambda nếu không dùng nữa

5. **Dừng và xóa EC2 backend**

   Vào **EC2 Console** và thực hiện:

   - Stop instance để kiểm tra lần cuối
   - Terminate instance backend nếu không cần giữ
   - Xóa Elastic IP nếu có gán riêng
   - Xóa key pair trên AWS nếu không còn sử dụng

6. **Xóa cơ sở dữ liệu Amazon RDS**

   Vào **RDS Console**, chọn database của project và quyết định:

   - **Giữ final snapshot** nếu muốn sao lưu dữ liệu trước khi kết thúc
   - **Không giữ snapshot** nếu đây chỉ là môi trường lab và không còn nhu cầu phục hồi

   Sau đó xóa database instance.

7. **Xóa S3 bucket lưu hình ảnh**

   Vào **Amazon S3**:

   - Xóa toàn bộ object trong bucket
   - Xác nhận bucket rỗng
   - Xóa bucket chứa ảnh hoặc static assets của project

8. **Xóa Security Group và tài nguyên mạng phụ trợ**

   Sau khi EC2 và RDS đã bị xóa, bạn có thể xóa tiếp:

   - Security Group dùng riêng cho EC2
   - Security Group dùng riêng cho RDS
   - DB subnet group nếu tạo riêng

9. **Xóa subnet, route table, internet gateway và VPC**

   Nếu VPC này chỉ phục vụ cho workshop, hãy xóa theo thứ tự:

   - Subnet
   - Route table tùy chỉnh
   - Internet Gateway (detach trước, rồi delete)
   - VPC

#### Ghi chú cuối

Trước khi xóa hoàn toàn tài nguyên, hãy chắc chắn rằng bạn đã lưu lại:

- Source code cuối cùng
- Ảnh chụp màn hình để viết báo cáo
- Link demo hoặc thông tin cấu hình quan trọng nếu cần đối chiếu sau này
