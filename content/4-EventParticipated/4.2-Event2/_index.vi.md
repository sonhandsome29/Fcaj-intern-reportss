---
title: "Event 2"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Bài thu hoạch “FCAJ Community Day (23-05-2026)”

### Mục đích của sự kiện

Buổi Community Day lần này tập trung mạnh hơn vào câu chuyện nghề nghiệp trong kỷ nguyên AI, cách làm việc với LLM có kiểm soát, cũng như cách xây hệ thống AI ở mức doanh nghiệp. Ngoài ra, sự kiện còn mở rộng sang bài toán dữ liệu, chi phí hạ tầng và tư duy phát triển sản phẩm.

Các mục tiêu chính gồm:

- Cập nhật góc nhìn nghề nghiệp trong bối cảnh AI phát triển rất nhanh
- Làm rõ vai trò của context khi sử dụng công cụ AI
- Tìm hiểu khả năng phân tích dữ liệu với Amazon Q Business
- Hiểu thêm về tối ưu chi phí và bảo vệ hạ tầng bằng AWS CloudFront
- Tiếp cận mô hình Multi-Agent ở cấp độ enterprise

### Diễn giả tham gia

- **Anh Nguyễn Gia Hưng** - Solution Architect AWS Việt Nam, Founder FCAJ
- **Anh Tịnh Trương** - Platform Engineer tại Got It
- **Anh Hải Anh** - Kỹ sư tại Pacific Việt Nam
- **Anh Nguyễn Hữu Thịnh** - DevOps Engineer
- **Team UTM Morpo (Uyển, Thảo, Mạch)** - Nhóm thắng giải Hackathon

### Nội dung nổi bật

#### 1. Định hướng nghề nghiệp trong thời đại AI

Một trong những ý chính của sự kiện là khi AI làm giảm chi phí tạo phần mềm, số lượng sản phẩm được xây dựng sẽ tăng nhanh. Điều đó không có nghĩa nhu cầu kỹ sư giảm đi, mà ngược lại, các vai trò như platform engineering, vận hành, bảo trì và tối ưu hệ thống sẽ càng quan trọng hơn.

Từ góc nhìn đó, diễn giả nhấn mạnh:

- Bằng cấp và kiến thức nền vẫn rất quan trọng
- Chỉ biết kỹ thuật là chưa đủ, cần hiểu thêm business context
- Sinh viên nên cố gắng tạo ra sản phẩm thực tế thay vì chỉ dừng ở demo

#### 2. Context và giới hạn của LLM

Phần này giúp tôi nhận ra rằng AI chỉ cho kết quả tốt khi nó được đặt vào đúng ngữ cảnh. Nếu không có context về domain, coding style hay yêu cầu nghiệp vụ, AI rất dễ sinh ra code vô ích hoặc khiến hệ thống phình to theo hướng khó kiểm soát.

Một khái niệm đáng chú ý là “Internet Puller”, tức thói quen sao chép công cụ, thư viện hoặc đoạn code từ nhiều nguồn mà không hiểu bản chất. Đây là điều rất nguy hiểm khi dự án phát triển lớn hơn.

Ngoài ra, diễn giả cũng nhắc đến tính không hoàn toàn ổn định của LLM: ngay cả khi để temperature thấp, output vẫn có thể khác nhau. Vì vậy, hệ thống dùng AI phải luôn chuẩn bị sẵn cho tình huống output sai format hoặc lệch mong đợi.

#### 3. Dữ liệu kinh doanh và hạ tầng cloud

Tôi thấy phần trình bày về **Amazon Q Business** khá thú vị vì nó cho thấy AI không chỉ dành cho code. Khi được kết nối với nguồn dữ liệu như Excel hoặc kho tài liệu doanh nghiệp, agent có thể hỗ trợ phân tích và dựng dashboard phục vụ quản trị mà không cần viết quá nhiều logic thủ công.

Với **AWS CloudFront**, nội dung chia sẻ tập trung vào góc nhìn thực tế của doanh nghiệp:

- Tối ưu chi phí tốt hơn với mô hình phù hợp
- Hạn chế rủi ro bill spike
- Tăng hiệu quả phân phối nội dung
- Hỗ trợ bảo mật tốt hơn cho origin

#### 4. Thiết kế hệ thống Multi-Agent cấp doanh nghiệp

Phần Multi-Agent là nội dung tôi thấy có chiều sâu nhất. Diễn giả nhấn mạnh rằng với những bài toán phức tạp, không nên nhồi toàn bộ xử lý vào một agent duy nhất. Thay vào đó, nên chia nhỏ theo chuyên môn: một agent phụ trách tài chính, một agent lo nghiên cứu thị trường, một agent điều phối tổng, v.v.

Đi kèm với đó là yêu cầu rất chặt về:

- Guardrails
- Phân quyền rõ ràng
- Audit log cho các quyết định AI đưa ra
- Tuân thủ bảo mật và pháp lý

### Những gì tôi học được

#### Về tư duy kỹ thuật

- Tối ưu LLM không chỉ nằm ở prompt mà còn nằm ở cách cung cấp context và kiểm soát rủi ro đầu ra
- Multi-Agent chỉ thực sự hữu ích khi có thiết kế vai trò và ranh giới trách nhiệm rõ
- Hạ tầng cloud cần được nhìn đồng thời ở ba góc: hiệu năng, bảo mật và chi phí

#### Về tư duy công việc

- Sản phẩm tốt không chỉ là sản phẩm chạy được, mà phải giải quyết đúng bài toán kinh doanh
- Viết hạ tầng bằng mã và quản lý thay đổi bài bản là tư duy rất quan trọng nếu muốn làm hệ thống nghiêm túc
- Khi thời gian và nguồn lực có hạn, cần ưu tiên core value thay vì cố nhồi quá nhiều tính năng

### Ứng dụng vào công việc

Sau sự kiện, tôi rút ra một số hướng áp dụng cụ thể:

- Dùng AI có chọn lọc hơn, tránh thói quen copy-paste thiếu kiểm chứng
- Kiểm tra kỹ đầu vào và đầu ra của LLM trước khi tích hợp vào hệ thống
- Học sâu hơn về serverless architecture và hạ tầng dạng Infrastructure as Code
- Khi đề xuất tính năng mới, luôn bắt đầu bằng business context và giá trị thực tế mang lại

### Trải nghiệm tại sự kiện

Buổi Community Day ngày 23/05/2026 cho tôi cảm giác rất khác so với các buổi chia sẻ công nghệ thông thường, vì nó không chỉ nói về “công cụ nào mới”, mà còn chỉ rõ khoảng cách giữa một bản demo và một sản phẩm đủ tiêu chuẩn doanh nghiệp. Tôi đặc biệt ấn tượng với cách các diễn giả đặt yếu tố bảo mật, compliance và business value lên trước cả sự hào nhoáng của AI.

Một bài học đáng nhớ khác là câu chuyện về feature creep từ nhóm thắng giải Hackathon. Điều đó khiến tôi nhận ra rằng đôi khi làm ít hơn nhưng đúng trọng tâm lại hiệu quả hơn nhiều so với cố gắng ôm quá nhiều thứ cùng lúc.

#### Một số hình ảnh khi tham gia sự kiện
![Event 2](/images/4-Event/event-2.jpg)

### Ảnh minh chứng tham gia Event 2

![Email xác nhận đăng ký Event 2](/images/4-Event/event2/registration-email.png)
*Email xác nhận đăng ký tham gia FCAJ Community Day ngày 23/05/2026.*

![Vé QR tham gia Event 2](/images/4-Event/event2/ticket-qr.png)
*Mã QR check-in sự kiện tại Bitexco Financial Tower.*

![Không gian sự kiện Event 2](/images/4-Event/event2/event-room.png)
*Toàn cảnh khu vực tổ chức và người tham dự trước giờ bắt đầu chương trình.*

![Ảnh người tham dự Event 2](/images/4-Event/event2/audience-photo.png)
*Không khí theo dõi phần trình bày tại sự kiện.*

![Slide Proposed Deployment Approach](/images/4-Event/event2/deployment-approach-slide.png)
*Minh họa nội dung chia sẻ về hướng triển khai hệ thống ở mức enterprise.*

![Slide Basic Deployment Flow](/images/4-Event/event2/deployment-flow-slide.png)
*Sơ đồ flow triển khai cơ bản được trình bày trong workshop.*

![Slide Workshop Exercises](/images/4-Event/event2/workshop-exercises-slide.png)
*Nội dung các bài tập thực hành đi kèm trong buổi chia sẻ.*

![Ghi chú whiteboard tại Event 2](/images/4-Event/event2/whiteboard-note.png)
*Một số từ khóa trọng tâm được nhấn mạnh trong phần thảo luận: Security, Reliability, Scalable.*

> Sau sự kiện này, tôi có góc nhìn rõ hơn về cách xây dựng hệ thống AI theo hướng thực tế và bền vững hơn, đặc biệt là khi bước vào môi trường doanh nghiệp hoặc các dự án có yêu cầu vận hành thật.
