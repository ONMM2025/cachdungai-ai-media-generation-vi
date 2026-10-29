---
name: ai-media-generation-vi
description: Chọn quy trình phù hợp để tạo ảnh, video hoặc âm thanh; chuẩn hóa brief, prompt, biến thể và kiểm tra quyền sử dụng.
license: MIT
---

# Điều phối tạo ảnh, video & âm thanh

## Vai trò

Skill giúp Agent điều phối nhiều loại tác vụ media thay vì dùng cùng một prompt cho mọi thứ. Nó phân loại đầu ra, hỏi đúng thông tin, xác nhận khả năng công cụ trong phiên hiện tại, chuẩn hóa prompt và đề xuất quy trình fallback. Khi không có công cụ tạo media, Agent vẫn bàn giao được prompt, shot brief hoặc thông số cần thiết nhưng phải nói rõ chưa tạo tệp.

Kích hoạt skill khi người dùng muốn chọn đúng loại tài nguyên và quy trình sinh ảnh, video hoặc âm thanh theo mục đích, đầu vào, giới hạn công cụ và chi phí. Kết thúc bằng đầu ra có cấu trúc, giả định được nêu rõ và việc cần người dùng duyệt được đánh dấu.

## Khi không nên dùng

- Người dùng chỉ cần một câu trả lời ngắn không liên quan đến sản xuất hình ảnh/video/âm thanh.
- Người dùng yêu cầu đăng, gửi, mua lượt tạo hoặc công khai nội dung nhưng chưa xác định đích đến, quyền sử dụng hoặc giới hạn chi phí. Hãy chuẩn bị bản nháp và dừng trước hành động đó.
- Thiếu dữ liệu thiết yếu khiến kết quả dễ gây hiểu lầm. Hỏi ngắn gọn, ưu tiên câu hỏi ảnh hưởng trực tiếp đến nội dung, quyền và ngân sách.

## Thông tin đầu vào cần thu thập

- Người xem, kênh đăng, mục tiêu và hành động mong đợi
- Loại tài nguyên cần: ảnh tĩnh, video, giọng đọc, nhạc hay hiệu ứng
- Kích thước/tỉ lệ, thời lượng, số biến thể, định dạng bàn giao
- Brief thương hiệu, tài liệu tham chiếu và quyền sử dụng
- Công cụ sẵn có, mức chi phí cho phép, thời hạn và quy trình duyệt

Nếu brief thiếu một vài chi tiết có thể tự quyết định an toàn, hãy ghi giả định và tiếp tục. Hỏi tối đa năm câu gộp một lần khi thiếu thông tin làm thay đổi thông điệp, quyền dùng tài sản, định dạng hoặc chi phí. Không yêu cầu lại thông tin người dùng đã cung cấp.

## Quy trình thực hiện

### 1. Phân loại yêu cầu

Xác định tài nguyên cuối cùng và vai trò của nó trong bài đăng. Phân biệt ảnh minh họa với ảnh sản phẩm chính xác; video diễn giải với video ghi lại sự kiện; giọng tổng hợp với bản ghi có sự đồng ý. Chuyển yêu cầu mơ hồ thành một deliverable đo được.

### 2. Kiểm tra công cụ có thật

Đọc các công cụ được cấp trong phiên và xác định chúng có tạo đúng modality, độ dài, tỉ lệ, định dạng hay không. Không giả vờ đã gọi công cụ, không khẳng định đã lưu tệp nếu chưa nhận đường dẫn xác thực. Nếu chỉ có khả năng viết prompt, bàn giao prompt thay vì tạo kết quả giả.

### 3. Chọn quy trình và xác nhận chi phí

Lập phương án chính và một phương án thay thế theo chất lượng cần thiết, thời gian và chi phí. Nếu công cụ tính theo lượt, độ dài hoặc tín dụng, ước lượng theo thông tin hiện có và hỏi trước khi vượt giới hạn đã nêu. Không gửi tài sản riêng tư lên dịch vụ chưa được người dùng chọn.

### 4. Chuẩn hóa creative brief

Khóa mục tiêu, chủ thể, bối cảnh, phong cách, bố cục, màu sắc, nội dung phải xuất hiện và những điều bị cấm. Dùng brief chung cho cả bộ media để ảnh bìa, clip và giọng đọc không lệch tông.

### 5. Viết prompt theo modality

Ảnh tập trung vào bố cục, chất liệu và chi tiết; video tập trung hành động và camera; giọng đọc tập trung người nghe, sắc thái, tốc độ và phát âm; nhạc/hiệu ứng tập trung chức năng và không gian trong bản phối. Không đưa yêu cầu chữ dài vào prompt ảnh nếu có thể dàn chữ hậu kỳ.

### 6. Sinh biến thể có chủ đích

Tạo vài biến thể khác nhau ở một yếu tố quyết định như góc nhìn, màu, hook hoặc nhịp, thay vì lặp prompt gần như nhau. Gắn nhãn mỗi biến thể và nêu tiêu chí chọn, tránh tạo nhiều tài nguyên không dùng.

### 7. Kiểm tra và bàn giao

Kiểm tra tệp/preview, tên file, kích thước, nội dung, lỗi sinh hình/âm thanh, phụ đề, quyền và khả năng đọc trên thiết bị mục tiêu. Bàn giao kèm prompt, công cụ đã dùng nếu biết, biến thể được chọn, giới hạn và việc cần người duyệt.

## Chuẩn đầu ra

Bảng kế hoạch gồm loại tài nguyên, mục đích, công cụ/khả năng sẵn có, prompt, biến thể, chi phí/giới hạn đã biết, tiêu chí chọn, trạng thái tạo tệp và checklist bàn giao.

Dùng nhãn rõ ràng như **Bản nháp**, **Giả định**, **Cần xác minh** và **Cần người dùng duyệt**. Tách nội dung có thể dùng ngay khỏi ghi chú sản xuất. Nếu chưa có công cụ hoặc tệp nguồn, bàn giao đặc tả có thể thực hiện và nói chính xác điều gì chưa được tạo.

## Quy tắc biên tập và vận hành

- Viết tiếng Việt tự nhiên, đúng chính tả; giữ thuật ngữ cần thiết và giải thích lần đầu. Tránh câu sáo, giọng hô hào, tiêu đề gây sốc và lời hứa không có bằng chứng.
- Nếu thông tin có thể thay đổi theo nền tảng, công cụ, giá hoặc quy định, yêu cầu dữ liệu hiện hành hoặc kiểm tra từ giao diện/tài liệu được người dùng cho phép. Không bịa kích thước, tính năng hay giới hạn.
- Không khẳng định ảnh/video là tư liệu thật nếu có nội dung tổng hợp. Không làm giả lời chứng thực, sự kiện, sản phẩm, bằng chứng hoặc kết quả.
- Tôn trọng quyền riêng tư, quyền hình ảnh, quyền tác giả, nhãn hiệu và quyền sử dụng nhạc/giọng. Nếu chưa rõ quyền, đề xuất thay bằng nhân vật hư cấu, ảnh tự tạo hoặc tài nguyên được cấp phép phù hợp.
- Không tải ảnh, video, transcript, giọng nói hoặc dữ liệu riêng tư lên dịch vụ ngoài khi chưa xác định đó là công cụ người dùng chọn và chưa có căn cứ gửi dữ liệu. Không đưa thông tin nhạy cảm, mật khẩu, mã xác thực hoặc token vào prompt.
- Không nói đã tạo, xem, chỉnh sửa, render hoặc lưu tệp nếu công cụ chưa xác nhận kết quả. Khi có công cụ, kiểm tra tệp đầu ra và báo đường dẫn thực tế.
- Các nền tảng thay đổi tiêu chuẩn định dạng và phân phối. Hãy dùng brief hiện hành; không bảo đảm viral, lượt xem, doanh thu hay kết quả kinh doanh.

## Tự kiểm tra trước khi bàn giao

- Modality và tệp bàn giao khớp yêu cầu.
- Chi phí, quyền, tài sản tham chiếu và bước gửi dữ liệu được làm rõ.
- Không bịa trạng thái của công cụ hay file đã tạo.
- Biến thể khác nhau có lý do, không chỉ đổi từ ngẫu nhiên.
- Có kế hoạch hậu kỳ cho chữ, logo, phụ đề và lỗi nhỏ.
- Mục tiêu, đối tượng và bước tiếp theo phù hợp với nhau.
- Không có thông tin được thêm vào chỉ để làm nội dung có vẻ thuyết phục.
- Đã phân biệt phần đã làm, phần đề xuất và phần còn chờ công cụ/người dùng.
- Bản bàn giao có thể được chỉnh tiếp mà không phải viết lại toàn bộ.

Nếu có lỗi, sửa phần gây lỗi trước; tránh làm mới toàn bộ khi chỉ cần điều chỉnh một thành phần. Nêu lỗi còn lại nếu không thể giải quyết đáng tin cậy.

## Prompt mẫu

> Tôi cần bộ media cho bài ra mắt lớp học online: một ảnh cover vuông, một video dọc 10 giây và giọng đọc ấm, không phô trương. Hãy kiểm tra công cụ hiện có trước, hỏi ngân sách tối đa nếu chưa có, lập brief chung, soạn prompt riêng từng loại, đánh dấu phần nào chưa thể tạo trong phiên và checklist duyệt trước khi đăng.

---

Biên soạn và watermark: [Cách Dùng AI](https://cachdungai.blog/)
