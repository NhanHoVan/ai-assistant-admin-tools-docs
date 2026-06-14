# Hướng Dẫn Cấu Hình

Sau khi cài đặt thành công plugin, bạn hãy truy cập vào menu **AI Assistant and Admin Tools** trong WordPress Admin để bắt đầu thiết lập. Dưới đây là hướng dẫn chi tiết từng phần cấu hình.

---

## ⚙️ 1. Cấu Hình Chung (General Settings)

Truy cập **AI Assistant and Admin Tools** -> **General Settings** để cài đặt các tùy chọn cơ bản:

*   **Activate assistant:** Tích chọn để kích hoạt hiển thị bong bóng Chatbot trợ lý ảo ở ngoài giao diện Frontend của website.
*   **Customize login page & Login logo URL:** Bật tính năng tùy biến giao diện trang đăng nhập. Nhấn nút **Upload** để chọn logo thương hiệu từ thư viện media của WordPress.
*   **Advertising options:** Thiết lập banner quảng cáo hiển thị ở góc dưới chatbot:
    *   **Vietnamese Ad Image & Link:** Điền link ảnh banner quảng cáo và đường dẫn đích khi người dùng click vào dành cho giao diện Tiếng Việt (`vi`).
    *   **English Ad Image & Link:** Điền link ảnh banner quảng cáo và đường dẫn đích khi người dùng click vào dành cho giao diện Tiếng Anh (`en`).
*   **Generate post with AI:** Tích chọn để kích hoạt tính năng viết bài bằng AI trực tiếp trong trình soạn thảo bài viết.

---

## 🤖 2. Cấu Hình Trợ Lý Ảo (AI Assistant)

Truy cập **AI Assistant and Admin Tools** -> **AI Assistant**. Giao diện cấu hình được chia thành các tab chức năng sau:

### Tab: Cấu hình API (AI Settings)
Thiết lập kết nối với nhà cung cấp dịch vụ AI:
*   **Model:** Nhập tên model AI muốn sử dụng (ví dụ: `gpt-4o`, `gpt-3.5-turbo`, `gemini-2.5-flash`,...).
*   **API Key:** Điền khóa API của tài khoản OpenAI hoặc nhà cung cấp của bạn (Key này sẽ được mã hóa bảo mật khi lưu vào cơ sở dữ liệu).
*   **API URL:** Đường dẫn endpoint kết nối API (mặc định: `https://api.openai.com/v1/chat/completions`).

### Tab: Thiết lập Prompt (Prompts)
Cấu hình câu lệnh hệ thống (System Prompts) điều hướng hành vi của AI:
*   **Generate post:** Câu lệnh định hình phong cách viết bài của AI (mặc định: *Bạn là một chuyên gia viết nội dung SEO, sử dụng các thẻ HTML phù hợp và đảm bảo tối ưu SEO.*).
*   **AI Assistant:** Câu lệnh định hình tính cách và hành vi cho Chatbot. Bạn có thể sử dụng biến động `{assistant_name}` để đồng bộ với tên Trợ lý đã thiết lập.
*   **AI Assistant (Training Data):** Dữ liệu huấn luyện, cung cấp thông tin về sản phẩm, dịch vụ hoặc doanh nghiệp của bạn để chatbot sử dụng trả lời khách hàng. Bạn có thể dùng các biến động:
    *   `{assistant_name}`: Thay thế bằng tên Trợ lý đã đặt.
    *   `{language_label}`: Tự động chuyển đổi ngôn ngữ hiện tại của khách chat ("Tiếng Việt" hoặc "English").

### Tab: Thiết lập Trợ Lý (Assistant Settings)
Tùy chỉnh giao diện hiển thị của chatbot:
*   **Upload Avatar:** Tải lên ảnh đại diện của chatbot trợ lý ảo.
*   **Assistant name:** Tên hiển thị của trợ lý (ví dụ: *Mimi*, *Jarvis*).
*   **Background/Text Color:** Thay đổi màu nền bong bóng chat và màu chữ để đồng bộ với giao diện website của bạn.
*   **Display position:** Lựa chọn hiển thị ở góc dưới bên trái (Bottom Left) hoặc bên phải (Bottom Right) của màn hình.
*   **Enable display:** Bật hoặc tắt nhanh tính năng hiển thị Chatbot ở Frontend.

### Tab: Gợi Ý Từ Khóa (Suggestions)
Thiết lập bộ hỏi đáp tự động giúp phản hồi ngay lập tức và tối ưu hóa chi phí API:
1. Nhấn nút **Add Suggestion** để tạo một mục mới.
2. Điền các từ khóa cách nhau bằng dấu phẩy (ví dụ: `giá cả, chi phí, bao nhiêu tiền`).
3. Nhập câu hỏi gợi ý và câu trả lời tương ứng.
4. Khi tin nhắn của khách hàng chứa một trong các từ khóa trên, chatbot sẽ hiển thị câu trả lời ngay lập tức mà không gọi đến API OpenAI.

### Tab: Lịch Sử Trò Chuyện (Histories)
Quản lý thông tin khách hàng và lịch sử hội thoại:
*   Danh sách khách hàng đã điền form xác thực (Tên, Email, Ngành nghề) sẽ được liệt kê tại đây.
*   Nhấp vào từng khách hàng để xem chi tiết lịch sử toàn bộ nội dung trò chuyện giữa khách hàng và Chatbot.

---

## 💡 Hỏi Đáp Chuyên Sâu Theo Danh Mục/Sản Phẩm

Chatbot hỗ trợ tính năng cho phép khách hàng lựa chọn các chuyên mục bài viết hoặc danh mục sản phẩm (WooCommerce) để hỏi đáp chuyên sâu.

### 📝 Cách thiết lập Danh mục hiển thị trên Chatbot
Admin chỉ cần thêm phần **Mô tả (Description)** cho Chuyên mục bài viết (tại `Posts` -> `Categories`) hoặc Danh mục sản phẩm (tại `Products` -> `Categories`). Bất kỳ danh mục nào chứa nội dung mô tả sẽ tự động xuất hiện thành nút bấm lựa chọn ngoài giao diện Chatbot khi khách hàng bắt đầu chat.

### ⚙️ Cách thức hoạt động
1. Ngoài giao diện chat, sau khi xác thực danh tính, khách hàng có thể lựa chọn tối đa **2 danh mục** quan tâm.
2. Khi khách hàng gửi câu hỏi, hệ thống sẽ tự động tìm kiếm nội dung mô tả của danh mục đó, đồng thời lấy danh sách **5 bài viết/sản phẩm mới nhất** thuộc danh mục đó để gửi kèm sang API làm dữ liệu tham khảo (Context).
3. AI sẽ dựa trên ngữ cảnh này để đưa ra câu trả lời cực kỳ chính xác theo chủ đề được chọn, đồng thời cung cấp sẵn các đường dẫn bài viết hoặc sản phẩm liên quan để người dùng có thể click xem ngay lập tức.
