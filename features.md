# Các Tính Năng Nổi Bật

**ITE Software Plus** cung cấp một bộ giải pháp toàn diện giúp tối ưu hóa quản trị website, thu thập leads khách hàng, tạo nội dung tự động bằng trí tuệ nhân tạo và cá nhân hóa trải nghiệm đăng nhập thương hiệu.

---

## 1. Trợ Lý Ảo AI Chatbot (Virtual Assistant)

Đây là tính năng tương tác khách hàng thông minh hiển thị ngoài giao diện Frontend của website.

*   **Xác thực danh tính khách hàng (Lead Capture):** Yêu cầu khách hàng nhập thông tin gồm Tên, Email và Ngành nghề hoạt động trước khi bắt đầu cuộc hội thoại. Giúp doanh nghiệp thu thập dữ liệu khách hàng tiềm năng một cách tự nhiên.
*   **Tùy chỉnh giao diện trực quan:** Cho phép quản trị viên cá nhân hóa giao diện bong bóng chat:
    *   Đặt tên riêng cho Trợ lý ảo (ví dụ: *Mimi*, *Jarvis*).
    *   Tải lên ảnh đại diện (Avatar) riêng.
    *   Tùy biến màu nền (Background) và màu chữ bong bóng chat phù hợp với màu sắc nhận diện của website.
    *   Thiết lập vị trí hiển thị (Dưới cùng bên trái hoặc bên phải màn hình).
*   **Tự động gợi ý từ khóa (Q&A Keyword Matching):** Thiết lập các bộ câu hỏi và câu trả lời nhanh dựa trên từ khóa. Khi người dùng nhập tin nhắn chứa các từ khóa định sẵn, chatbot sẽ trả lời ngay lập tức mà không cần gọi API OpenAI, giúp phản hồi nhanh và tối ưu chi phí sử dụng API.
*   **Hỏi đáp thông minh theo Danh mục / Sản phẩm:** Khách hàng có thể lựa chọn tối đa 2 danh mục bài viết hoặc danh mục sản phẩm (WooCommerce) để khoanh vùng câu hỏi. Hệ thống sẽ tự động gửi kèm mô tả danh mục cùng danh sách 5 bài viết/sản phẩm mới nhất làm ngữ cảnh cho AI, giúp câu trả lời tập trung và cung cấp trực tiếp link xem bài viết/sản phẩm.
*   **Lịch sử chat chi tiết:** Lưu trữ toàn bộ các cuộc hội thoại của khách hàng trực tiếp trong trang quản trị giúp Admin có thể theo dõi hành vi và hỗ trợ kịp thời.

---

## 2. Viết Bài Tự Động Bằng AI (AI Post Generator)

Hỗ trợ các quản trị viên và biên tập viên tạo nội dung bài viết chuẩn SEO trực tiếp bên trong trình soạn thảo bài viết của WordPress.

*   **Tạo bài viết chuẩn SEO:** Tích hợp OpenAI viết bài dựa trên các yêu cầu tiêu đề, từ khóa mục tiêu, dàn bài,... với định dạng thẻ HTML chuẩn SEO.
*   **Hàng đợi tạo bài viết (Generator Queue):** Các yêu cầu viết bài số lượng lớn hoặc tốn nhiều thời gian sẽ được đẩy vào hàng đợi và xử lý ngầm (sử dụng WP Cron), ngăn chặn tình trạng quá tải server hoặc gặp lỗi quá hạn thời gian thực thi (timeout).

---

## 3. Tùy Biến Trang Đăng Nhập (Custom Login)

Cá nhân hóa trang đăng nhập mặc định của WordPress (`/wp-login.php`) để tăng nhận diện thương hiệu đối với khách hàng hoặc nhân viên.

*   **Thay đổi Logo thương hiệu:** Thay logo WordPress mặc định bằng logo thương hiệu của bạn (có nút Upload và quản lý ảnh trực quan).
*   **Thay đổi Link Logo:** Đường dẫn khi bấm vào logo sẽ trỏ về trang chủ của website thay vì trang chủ `WordPress.org`.
*   **Tự động chọn "Remember Me":** Luôn tự động tích chọn hộp kiểm "Tự động đăng nhập" để thuận tiện cho người dùng.

---

## 4. Banner Quảng Cáo Đa Ngôn Ngữ

Quảng bá sản phẩm hoặc dịch vụ trực tiếp thông qua bong bóng chat.

*   **Định cấu hình đa ngôn ngữ:** Hỗ trợ cấu hình đường dẫn ảnh banner và liên kết hành động riêng biệt cho Tiếng Việt và Tiếng Anh.
*   **Hiển thị thông minh:** Banner tự động xuất hiện ở góc dưới khung chatbot giúp thu hút sự chú ý của khách hàng một cách tự nhiên.

---

## 5. Ghi Log Hệ Thống & Bảo Mật (Security Logs)

Đảm bảo hệ thống hoạt động ổn định và dễ dàng xử lý sự cố.

*   **Ghi nhận lỗi API:** Tự động ghi nhận chi tiết các lỗi kết nối đến API OpenAI (sai key, hết hạn mức, quá thời gian chờ,...).
*   **Thông tin ngữ cảnh đầy đủ:** Log ghi lại địa chỉ IP, hành động cụ thể và thời gian chính xác xảy ra lỗi.
*   **Giao diện quản lý trực quan:** Admin có thể dễ dàng tìm kiếm, lọc và phân trang các bản ghi lỗi ngay trên trang quản trị.
