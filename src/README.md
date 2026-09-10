# Gia Phả Việt — Bản Một Dòng họ

Đây là bản dành cho một gia đình hoặc một dòng họ tự lập gia phả của mình. Ứng dụng không có chức năng quản lý nhiều dòng họ và không có Dropdown chuyển dòng họ.

Hướng dẫn vận hành, chia sẻ và yêu cầu phân quyền nhiều người dùng nằm trong file `../HUONG-DAN-SU-DUNG-CHIA-SE-VA-PHAN-QUYEN.md`.

## Mở ứng dụng

- Cách nhanh và an toàn khi nâng cấp: mở `mo-ban-moi.html`. Trang này tự xóa bộ nhớ giao diện cũ rồi chuyển sang ứng dụng.
- Có thể mở trực tiếp `index.html` sau lần nâng cấp đầu tiên.
- Để dùng chế độ cài đặt PWA/offline đầy đủ, chạy thư mục bằng một web server cục bộ rồi mở trên `localhost`.

## Dữ liệu

- Tự động lưu trong bộ nhớ của trình duyệt (`localStorage`).
- Vào **Dữ liệu & sao lưu → Sao lưu toàn bộ** để tải bản JSON định kỳ.
- Có thể khôi phục JSON, nhập CSV/GEDCOM, xuất JSON/CSV/GEDCOM và in sách ra PDF.
- Dữ liệu minh họa không được nạp mặc định; chỉ tạo khi người dùng chủ động chọn **Khôi phục dữ liệu mẫu**.
- Mọi thao tác tra cứu, chỉnh sửa, nhập/xuất và in ấn chỉ áp dụng cho một dòng họ duy nhất của người sử dụng.

## Quy tắc Nam hệ

- Nam thuộc dòng họ tiếp tục mở rộng hậu duệ.
- Nữ vẫn có hồ sơ, đời, chi/nhánh và tư liệu đầy đủ nhưng cây chính dừng tại nữ.
- Hậu duệ bên nữ có thể lưu với vai trò `external` (ngoại hệ) và không tự xuất hiện trong cây Nam hệ.
- Chuyển sang chế độ “Mở rộng hai bên” chỉ đổi cách hiển thị, không xóa dữ liệu.

## Phạm vi MVP

Đã có: dữ liệu mẫu, CRUD hồ sơ, chi/nhánh, cây nhiều tầng, tìm kiếm, ảnh/tư liệu nhẹ, cấu hình dòng họ, backup/restore, CSV, JSON, GEDCOM cơ bản, bản sách và in/PDF.

Để dùng quy mô lớn hoặc nhiều người cùng biên soạn, bước tiếp theo nên chuyển lớp lưu trữ sang IndexedDB/SQLite, bổ sung phân quyền, nhật ký thay đổi, GEDCOM parser đầy đủ và đóng gói media riêng.
