# Điều phối tạo ảnh, video & âm thanh

Chọn đúng loại tài nguyên và quy trình sinh ảnh, video hoặc âm thanh theo mục đích, đầu vào, giới hạn công cụ và chi phí.

## Skill này giúp gì?

Skill giúp Agent điều phối nhiều loại tác vụ media thay vì dùng cùng một prompt cho mọi thứ. Nó phân loại đầu ra, hỏi đúng thông tin, xác nhận khả năng công cụ trong phiên hiện tại, chuẩn hóa prompt và đề xuất quy trình fallback. Khi không có công cụ tạo media, Agent vẫn bàn giao được prompt, shot brief hoặc thông số cần thiết nhưng phải nói rõ chưa tạo tệp.

## Nội dung gói

- `SKILL.md`: quy trình chi tiết, đầu vào, đầu ra và tiêu chí tự kiểm tra.
- `README.md`: hướng dẫn cài và prompt bắt đầu.
- `LICENSE`: giấy phép MIT.

## Cách cài và dùng

1. Tải ZIP rồi giải nén; giữ nguyên thư mục có `SKILL.md`.
2. Mở phần Skills/Agent Skills của ứng dụng AI đang dùng và thêm thư mục hoặc tải gói theo hướng dẫn trong ứng dụng. Nếu ứng dụng chưa hỗ trợ nạp skill, dán nội dung `SKILL.md` vào chỉ dẫn của một cuộc trò chuyện/dự án và dùng prompt mẫu bên dưới.
3. Bắt đầu cuộc trò chuyện bằng mục tiêu, người xem, nền tảng, giới hạn và tệp tham chiếu bạn có quyền sử dụng. Không gửi mật khẩu, mã xác minh, token hoặc dữ liệu khách hàng không cần thiết.
4. Đọc phần **Giả định** và **Cần người dùng duyệt**. Kiểm tra kỹ quyền dùng tài nguyên, dữ liệu, giá và quy định hiện hành trước khi tạo tệp tốn phí hoặc đăng công khai.
5. Lặp lại bằng cách nêu một thay đổi cụ thể; yêu cầu Agent giữ nguyên những phần đã duyệt.

Cách nạp skill khác nhau giữa ứng dụng và tài khoản. Hãy làm theo giao diện hiện hành của ChatGPT, Claude hoặc Agent khác; đừng giả định một nút cài đặt giống nhau có ở mọi gói.

## Prompt bắt đầu

> Tôi cần bộ media cho bài ra mắt lớp học online: một ảnh cover vuông, một video dọc 10 giây và giọng đọc ấm, không phô trương. Hãy kiểm tra công cụ hiện có trước, hỏi ngân sách tối đa nếu chưa có, lập brief chung, soạn prompt riêng từng loại, đánh dấu phần nào chưa thể tạo trong phiên và checklist duyệt trước khi đăng.

## Tác giả và watermark

Biên soạn: [cachdungai.blog](https://cachdungai.blog/)

Gói được phân phối miễn phí theo điều khoản trong `LICENSE`. Kết quả tạo media có thể cần công cụ, tài khoản hoặc chi phí riêng; hãy duyệt đầu ra trước khi dùng công khai.
