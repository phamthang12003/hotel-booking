# 🏨 Hotel Booking Management System

Một ứng dụng quản lý và đặt phòng khách sạn hiện đại, cung cấp giao diện trực quan để quản lý hệ thống phòng nghỉ. Dự án được xây dựng với kiến trúc Front-end mạnh mẽ, tích hợp sẵn hệ thống xác thực người dùng bảo mật cao.

## ✨ Tính năng cốt lõi
* **Xác thực bảo mật:** Tích hợp Clerk Authentication quản lý đăng nhập/đăng ký an toàn.
* **Dashboard trực quan:** Trang tổng quan hiển thị các số liệu thống kê nhanh về hệ thống khách sạn.
* **Quản lý phòng nghỉ (Room Management):**
  * Hiển thị danh sách phòng chi tiết kèm hình ảnh.
  * Hỗ trợ chức năng thêm phòng mới vào hệ thống một cách nhanh chóng.
* **Tối ưu hóa hiệu suất:** Ứng dụng được đóng gói và biên dịch siêu tốc nhờ công cụ Vite.

## 🛠️ Công nghệ sử dụng
* **Core Framework:** ReactJS, Vite.
* **Authentication:** Clerk.
* **Package Manager:** npm (Quản lý qua `package-lock.json`).

## 📁 Cấu trúc thư mục chính
```text
hotel-booking/
├── client/
│   ├── public/              
│   ├── src/
│   │   ├── assets/           # Chứa tài nguyên hình ảnh (roomImg1, roomImg2, regImage...)
│   │   ├── components/       # Các UI component tái sử dụng
│   │   ├── pages/            # Các trang giao diện chính (Dashboard, List Room, Add Room)
│   │   ├── App.jsx               
│   │   └── main.jsx              
│   ├── .env                  # Cấu hình biến môi trường (Clerk API Key)
│   ├── package.json              
│   └── vite.config.js

🚀 Hướng dẫn Cài đặt & Khởi chạy môi trường Dev
Thực hiện các bước sau để chạy dự án trên máy tính cục bộ của bạn:

1. Clone dự án và di chuyển vào thư mục Client
Bash
git clone [https://github.com/phamthang12003/hotel-booking.git](https://github.com/phamthang12003/hotel-booking.git)
cd hotel-booking/client
2. Cài đặt các thư viện phụ thuộc (Dependencies)
Bash
npm install
3. Cấu hình biến môi trường
Dự án yêu cầu khóa API của Clerk để hệ thống đăng nhập hoạt động.

Tạo một file tên là .env tại thư mục client/.

Thêm khóa Publishable Key của Clerk vào file .env theo định dạng sau:

Đoạn mã
VITE_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key_here"

4. Chạy ứng dụng
Bash
npm run dev
Truy cập vào liên kết cục bộ được cung cấp trên Terminal (thường là http://localhost:5173) để sử dụng hệ thống.