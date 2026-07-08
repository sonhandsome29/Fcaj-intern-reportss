---
title: "Event 3"
date: 2026-07-04
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Bài thu hoạch “AWS GameDay - 8 Đội Tranh Hùng”

### Mục Đích Của Sự Kiện

- Tạo sân chơi thi đấu kiến thức công nghệ thực tế và kịch tính trên nền tảng AWS
- Đánh giá khả năng phản xạ, xử lý tình huống và tư duy kiến trúc hệ thống của các đội
- Rèn luyện kỹ năng làm bài thi chứng chỉ AWS thông qua format trắc nghiệm tính giờ
- Kết nối cộng đồng đam mê điện toán đám mây

### Thành Phần Tham Dự

- **Ban tổ chức & Trọng tài** - Các chuyên gia AWS chịu trách nhiệm ra đề và kiểm soát trận đấu
- **8 Đội thi** - Các thí sinh xuất sắc tham gia tranh tài trực tiếp trên sân khấu
- **Khán giả** - Những người theo dõi, cổ vũ và học hỏi kiến thức từ các lượt đấu

### Nội Dung Nổi Bật

#### Thể thức thi đấu đối kháng (Knockout)

- **Cấu trúc giải đấu:** 8 đội chia thành các cặp thi đấu trực tiếp (1 vs 1) qua các vòng Tứ kết, Bán kết và Chung kết.
- **Giới hạn trận đấu:** Mỗi lượt đấu sẽ giải quyết đúng 10 câu hỏi trắc nghiệm.

#### Luật thi đấu đồng thời & Tính điểm "Sinh tử"

Quy tắc thi đấu áp đặt một áp lực thời gian và tâm lý cực lớn lên cả 2 đội:
- **Trả lời đồng thời:** Chỉ có 1 câu hỏi xuất hiện trên màn hình với thời gian đếm ngược chung. Cả 2 đội **bắt buộc** phải chốt đáp án, không đội nào được quyền bỏ qua. 
- **Kiểm tra kết quả:** Hết thời gian, hệ thống sẽ mở đáp án của cả 2 đội cùng lúc.
- **Trả lời đúng:** Đội được cộng điểm lợi thế.
- **Trả lời sai:** Đội bị trừ điểm trực tiếp vào tổng điểm hiện có.

#### Phân loại câu hỏi AWS

- **Kiến thức nền tảng:** Các câu hỏi tốc độ, yêu cầu định nghĩa nhanh chức năng của một dịch vụ cụ thể (tương đương cấp độ Cloud Practitioner).
- **Tình huống hệ thống:** Các câu hỏi dài, mô tả vấn đề của doanh nghiệp và yêu cầu chọn giải pháp kiến trúc tối ưu (tương đương cấp độ Solutions Architect).

### Những Gì Học Được

#### Chiến Thuật Làm Bài Trắc Nghiệm

- **Quản lý rủi ro:** Vì luật thi không cho phép bỏ qua câu hỏi, các đội không được phép hoảng loạn. Khi gặp câu khó, thay vì "đoán mò" (đánh lụi) dễ dẫn đến bị trừ điểm, họ buộc phải bình tĩnh phân tích để có sự lựa chọn rủi ro thấp nhất.
- **Kỹ năng Scan Keyword:** Không đọc từng chữ trong đề bài dài. Tập trung quét các từ khóa cốt lõi (ví dụ: *most cost-effective*, *decouple*, *single-digit millisecond latency*) để định hình ngay hướng giải quyết trong thời gian ngắn.
- **Nghệ thuật loại trừ:** Áp lực thời gian chung khiến việc tìm ngay câu đúng rất khó. Thay vào đó, tập trung chỉ ra điểm vô lý của các đáp án sai để loại trừ dần, từ đó chốt lại lựa chọn cuối cùng an toàn nhất trước khi hết giờ.

#### Kiến Thức Công Nghệ Thực Chiến

- **Phản xạ dịch vụ:** Nắm vững bản chất của hệ sinh thái AWS để có thể "khớp" yêu cầu với dịch vụ chỉ trong 1-2 giây.
- **Architecture Patterns:** Hiểu rõ cách phối hợp các dịch vụ (ví dụ: dùng SQS làm buffer trước Lambda để chống nghẽn, hoặc chọn Spot Instances khi cần tối ưu chi phí cho batch processing).

#### Tâm Lý Thi Đấu

- **Giữ "cái đầu lạnh":** Việc phải nhìn thấy đáp án của đối thủ sau mỗi câu hỏi rất dễ gây dao động tâm lý. Cần giữ bình tĩnh ngay cả khi bị đối thủ dẫn trước hoặc lỡ trả lời sai và bị trừ điểm.
- **Tập trung cao độ:** Chắt chiu từng cơ hội trong giới hạn 10 câu hỏi, vì một câu trả lời đúng ở phút chót có thể lật ngược hoàn toàn thế cờ.

### Ứng Dụng Vào Công Việc (Và Học Tập)

- **Luyện thi chứng chỉ AWS:** Áp dụng ngay phương pháp *scan keyword* và *chiến thuật loại trừ* vào quá trình ôn luyện thi chứng chỉ.
- **Thiết kế hệ thống:** Cân nhắc kỹ các yếu tố về chi phí, độ trễ và khả năng chịu lỗi (fault-tolerant) khi đề xuất giải pháp công nghệ cho dự án hiện tại.
- **Rèn luyện tâm lý:** Tự đặt giờ và áp dụng luật "sai trừ điểm" khi làm bài thi thử (mock exam) ở nhà để làm quen với áp lực phòng thi.

### Trải nghiệm trong event

Tham gia sự kiện **“AWS GameDay - 8 Đội Tranh Hùng”** dưới góc độ khán giả là một trải nghiệm cực kỳ kịch tính và mang lại nhiều bài học bất ngờ, vượt xa việc chỉ đọc tài liệu thông thường. Một số trải nghiệm nổi bật:

#### Áp lực từ hàng ghế khán giả
- Dù không trực tiếp thi đấu, việc theo dõi 2 đội chịu chung một đồng hồ đếm ngược và luật chơi "Đúng cộng - Sai trừ" cũng khiến tôi cảm nhận rõ áp lực đè nặng lên các thí sinh. 
- Khoảnh khắc hệ thống lật mở đáp án của cả 2 đội cùng một lúc thực sự rất hồi hộp và cảm xúc.

#### Học hỏi từ chiến thuật của người xuất sắc
- Nhìn cách các đội mạnh phản ứng với đề bài dài ngoẵng chỉ trong vài giây giúp tôi nhận ra lỗ hổng trong cách đọc hiểu của bản thân.
- Hiểu được rằng, việc nhớ tài liệu AWS là chưa đủ; khả năng phán đoán, phân tích logic để quản lý rủi ro trong tình huống bắt buộc mới là chìa khóa phân định thắng thua.

#### Đánh giá lại năng lực bản thân
- Việc "thi nhẩm" cùng các đội tuyển giúp tôi tự kiểm tra nhanh kiến thức của mình, đặc biệt là ở mảng Networking và Database.
- Nhận ra rằng mình cần phải thực hành thực tế (Hands-on labs) nhiều hơn thay vì chỉ học lý thuyết suông.

#### Một số hình ảnh khi tham gia sự kiện
* Thêm các hình ảnh của các bạn tại đây
> Nhìn chung, việc quan sát các đội tranh tài tại AWS GameDay là một phương pháp "luyện thi" thực nghiệm vô cùng hiệu quả. Sự kiện đã tiếp thêm cho tôi rất nhiều động lực và định hướng rõ ràng để chinh phục các chứng chỉ AWS trong tương lai.