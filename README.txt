================================================================
HƯỚNG DẪN CÀI ĐẶT VÀ SỬ DỤNG
PHẦN MỀM QUẢN LÝ GIÁO VIÊN PHỔ THÔNG
================================================================
Sinh viên thực hiện:
Huỳnh Phúc Lâm - DPM245446
Lê Nguyễn Đăng Khoa - DPM245442
Lớp: DH25PM
================================================================

I. YÊU CẦU HỆ THỐNG
-------------------
1. Hệ điều hành: Windows 10/11.
2. Phần mềm bắt buộc: MySQL Server (Có thể dùng XAMPP hoặc MySQL Workbench) để chạy cơ sở dữ liệu.
   Lưu ý: Phần mềm đã được đóng gói (.exe) nên không cần cài Python và thư viện liên quan.

================================================================

II. HƯỚNG DẪN CÀI ĐẶT CƠ SỞ DỮ LIỆU (QUAN TRỌNG)
------------------------------------------------
Trước khi mở phần mềm, Thầy/Cô vui lòng nạp dữ liệu vào MySQL.
Thầy/Cô có thể chọn 1 trong 2 cách dưới đây tùy theo phần mềm đang sử dụng.

------------------------------------------------
CÁCH 1: DÙNG PHPMYADMIN (NẾU SỬ DỤNG XAMPP)
------------------------------------------------
BƯỚC 1: Khởi động XAMPP
   - Mở XAMPP Control Panel.
   - Bấm "Start" ở 2 mục: Apache và MySQL (Đợi hiện màu xanh).

BƯỚC 2: Tạo Cơ sở dữ liệu
   - Mở trình duyệt web, truy cập: http://localhost/phpmyadmin/
   - Ở cột bên trái, bấm "New" (Mới).
   - Nhập tên Database chính xác là: qlgiaovien
     (Lưu ý: Phải nhập đúng tên này thì phần mềm mới nhận diện được).
   - Chọn bảng mã: utf8mb4_unicode_ci (Để hiển thị tiếng Việt không lỗi).
   - Bấm "Create" (Tạo).

BƯỚC 3: Nạp file dữ liệu (.sql)
   - Bấm vào tên database "qlgiaovien" vừa tạo.
   - Chọn thẻ "Import" (Nhập) trên thanh menu.
   - Bấm "Choose File" (Chọn tệp) -> Chọn file "qlgiaovien.sql" trong thư mục nộp bài.
   - Kéo xuống dưới cùng bấm nút "Go" (Thực hiện).

------------------------------------------------
CÁCH 2: DÙNG MYSQL WORKBENCH
------------------------------------------------
BƯỚC 1: Tạo Schema (Database)
   - Mở MySQL Workbench và kết nối vào Local instance.
   - Bấm chuột phải vào khoảng trắng ở cột SCHEMAS (bên trái), chọn "Create Schema...".
   - Nhập tên Name: qlgiaovien
   - Bấm "Apply" -> "Apply" -> "Finish".

BƯỚC 2: Import dữ liệu
   - Trên thanh menu, chọn Server -> Data Import.
   - Chọn mục "Import from Self-Contained File".
   - Bấm nút 3 chấm (...) và chọn file "qlgiaovien.sql" trong thư mục nộp bài.
   - Ở mục "Default Target Schema", chọn: qlgiaovien
   - Bấm nút "Start Import" ở góc dưới bên phải.

================================================================

III. HƯỚNG DẪN CHẠY PHẦN MỀM
----------------------------
1. Chạy file "Setup.exe" để cài đặt phần mềm vào máy.
2. Sau khi cài xong, mở biểu tượng "Quản lý giáo viên phổ thông" ngoài Desktop.
3. Phần mềm sẽ tự động kết nối và hiển thị dữ liệu.

================================================================

IV. XỬ LÝ LỖI KẾT NỐI (NẾU CÓ)
------------------------------
Nếu mở phần mềm báo lỗi "Lỗi kết nối CSDL", vui lòng kiểm tra:

1. Đã bật MySQL (trong XAMPP hoặc Services) chưa?
2. Tên Database đã tạo có đúng chính xác là "qlgiaovien" không?
3. Cấu hình User/Pass của MySQL:
   - Phần mềm được cấu hình mặc định cho môi trường XAMPP chuẩn:
     + User: root
     + Password: không có hoặc rỗng
   - Nếu máy Thầy đã đặt mật khẩu cho tài khoản root (thường thấy khi dùng Workbench), phần mềm sẽ không kết nối được. 
   - Kính mong Thầy tạm thời xóa mật khẩu root hoặc cấu hình về mặc định.

----------------------------------------------------------------
Xin cảm ơn Thầy đã chấm bài!