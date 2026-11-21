# HỆ THỐNG THANH TẨY 5.0 | HỒ SƠ THỰC THỂ (`CORE-X`)

Giao diện web quản lý, truy quét và thanh tẩy hồ sơ thực thể theo phong cách Cyberpunk / Huyền huyễn, tích hợp cơ chế **1 Key = 1 Hồ Sơ**, phân quyền **Quản Lý (Admin)** và lưu trữ cục bộ qua `localStorage` để chạy mượt trên cả Android, iOS lẫn máy tính.

---

## ✨ Tính Năng Chính

* **Phân Quyền Khách & Quản Lý (Admin):**
  * **Chế độ Khách:** Xem danh sách thực thể, lọc trạng thái, tìm kiếm theo tên/mã Key/ID/mô tả và sao chép mã Key.
  * **Quyền Quản Lý:** Đăng nhập bằng mã PIN (mặc định: `6868`, hỗ trợ đổi mã PIN trực tiếp trên giao diện).
* **Tạo Key = Khởi Tạo Hồ Sơ (`1 Key = 1 Hồ Sơ`):**
  * Tạo đơn lẻ: Nhập mã Key tùy chỉnh hoặc bấm **Sinh Mã** (`KP68-XXXX-XXXX`), chọn cấp độ (`SSS` / `SS`) và điền thông tin thực thể.
  * Tạo hàng loạt: Nhập nhiều mã Key (mỗi dòng 1 Key) để tự động tạo các hồ sơ độc bản tương ứng.
* **Danh Sách Key Đã Cấp Phát:**
  * Theo dõi liên kết trực tiếp giữa **Mã Key**, **Mã Hồ Sơ (`ENT-xxx`)**, **Tên Thực Thể**, **Cấp Độ**, **Trạng Thái** và **Ngày Tạo**.
  * Hỗ trợ **Copy**, chuyển trạng thái **Thanh tẩy / Khôi phục**, hoặc **Thu hồi Key** (xóa hồ sơ).
* **Lưu Trữ Tự Động (`localStorage`):**
  * Dữ liệu hồ sơ/Key (`entities_v5_key_profiles`) và mã PIN (`system5_admin_pin`) được lưu trên trình duyệt của thiết bị.

---

## 🚀 Cách Chạy & Triển Khai

### 1. Chạy trực tiếp trên máy hoặc điện thoại
1. Lưu mã nguồn giao diện thành tệp `index.html`.
2. Mở `index.html` bằng trình duyệt bất kỳ (Chrome, Safari, Edge...) hoặc tải tệp lên điện thoại Android/iOS để mở xem trực tiếp.

### 2. Xuất bản lên GitHub Pages (2026)
1. Tạo repository mới trên GitHub và đẩy tệp `index.html` (cùng `README.md`) lên nhánh chính (`main`).
2. Vào **Settings** → **Pages** của repository.
3. Trong mục **Build and deployment**, chọn nguồn triển khai từ nhánh `main` (thư mục `/ (root)`) và lưu lại để nhận đường dẫn truy cập web.

---

## 🔐 Hướng Dẫn Quản Lý Nhanh

* **Mã PIN mặc định:** `6868` — nên đổi mã PIN ngay sau khi đăng nhập lần đầu.
* **Quy ước Key:** Hệ thống tự động chuẩn hóa chữ hoa và chặn tạo trùng mã Key đã liên kết với hồ sơ hiện có.
* **Phạm vi lưu trữ:** Do dữ liệu lưu tại `localStorage` của từng trình duyệt/thiết bị, nếu chuyển sang thiết bị khác hoặc xóa dữ liệu duyệt web, bạn cần sao lưu danh sách Key trước.

---

## 🛠️ Công Nghệ Sử Dụng

* **HTML5** & **CSS3** (CSS Variables, Grid/Flexbox, Glassmorphism, Neon HUD)
* **Vanilla JavaScript** (DOM Rendering, Clipboard API, `localStorage`)

---

*Thiết kế bởi **KhangPanh68** — Tối ưu cho nền tảng Android / iOS.*
