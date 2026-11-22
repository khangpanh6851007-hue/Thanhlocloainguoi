# HỆ THỐNG THANH TẨY 5.0 // CORE-X

Ứng dụng web đơn trang (HTML/CSS/JS thuần) dùng để lưu trữ, tra cứu, lọc và quản lý hồ sơ thực thể theo mô hình **1 Key = 1 Hồ sơ**, kèm liên kết nhanh tới **Cổng Địa Ngục Âm Phủ**.

## Tính năng chính

* **Mô hình 1 Key = 1 Hồ sơ:** Tạo đơn lẻ (nhập tay hoặc sinh mã ngẫu nhiên `KP68-XXXX-XXXX`) hoặc tạo hàng loạt theo từng dòng, tự động cấp mã hồ sơ `ENT-xxx`.
* **Phân quyền Khách / Quản lý:**
  * **Chế độ Khách:** Xem danh sách, tìm kiếm, lọc trạng thái và sao chép mã Key.
  * **Chế độ Quản lý:** Mở khóa bằng mã PIN (mặc định `6868`), hỗ trợ đổi mã PIN, tạo/xóa/thu hồi Key và hồ sơ.
* **Tra cứu & thống kê trực quan:** Tìm theo tên thực thể, mã Key, mã hồ sơ hoặc mô tả; lọc theo *Tất cả*, *Chưa thanh tẩy*, *Đã thanh tẩy* và theo dõi số lượng theo thời gian thực.
* **Website liên kết:** Truy cập nhanh **Cổng Địa Ngục Âm Phủ** tại `https://khangpanh6851007-hue.github.io/AmPhuCongDiaNguc/`.
* **Lưu trữ cục bộ:** Dữ liệu hồ sơ và mã PIN được lưu trên trình duyệt / WebView thông qua `localStorage`.

## Cấu trúc dự án

```text
.
├── index.html   # Giao diện, logic quản lý Key/Hồ sơ và liên kết hệ thống
└── README.md    # Tài liệu hướng dẫn sử dụng
