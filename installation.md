# Hướng Dẫn Cài Đặt

Để cài đặt và sử dụng plugin **ITE Software Plus**, bạn hãy thực hiện theo các bước đơn giản sau:

## 📥 Các Bước Cài Đặt

### Cách 1: Tải lên qua WordPress Admin (Khuyên dùng)
1. Tải về tệp nén định dạng `.zip` của plugin.
2. Truy cập vào trang quản trị WordPress (Admin Dashboard).
3. Đi tới mục **Plugins** -> **Add New** (Thêm mới).
4. Nhấp vào nút **Upload Plugin** (Tải plugin lên) ở đầu trang.
5. Chọn tệp `.zip` đã tải về và nhấp **Install Now** (Cài đặt ngay).
6. Sau khi cài đặt hoàn tất, nhấp vào **Activate Plugin** (Kích hoạt plugin).

### Cách 2: Tải lên qua FTP hoặc File Manager
1. Giải nén tệp `.zip` của plugin trên máy tính của bạn.
2. Kết nối với máy chủ của bạn bằng FTP client (như FileZilla) hoặc công cụ File Manager của CPanel/DirectAdmin.
3. Tải thư mục `ite-software-plus` lên thư mục `/wp-content/plugins/` của website WordPress.
4. Truy cập trang quản trị WordPress, đi tới mục **Plugins** -> **Installed Plugins**.
5. Tìm plugin **ITE Software Plus** trong danh sách và nhấp **Activate** (Kích hoạt).

---

## ⚙️ Sau Khi Kích Hoạt

Sau khi kích hoạt thành công:
- Menu quản trị **ITE Software Plus** sẽ xuất hiện trong thanh menu bên trái của WordPress Admin.
- Hệ thống sẽ tự động khởi tạo các bảng cơ sở dữ liệu cần thiết để lưu trữ cấu hình, lịch sử chat và hàng đợi tạo bài viết.
- Một tác vụ định kỳ (WP Cron) sẽ được lên lịch chạy hàng giờ để xử lý hàng đợi tạo bài viết bằng AI.

Tiếp theo, hãy chuyển sang mục **[Cấu Hình Hệ Thống](configuration.md)** để thiết lập kết nối API OpenAI và bắt đầu sử dụng.
