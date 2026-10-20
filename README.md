# Nhật ký chúc mừng 20/10

Một cuốn sách tương tác mừng Ngày Phụ nữ Việt Nam 20/10. Bốn trang đầu lần lượt mở bốn tấm ảnh có sẵn; ở trang thứ năm, người nhận chọn một trong bốn ảnh để mở lời chúc đặc biệt. Trang cuối là hộp quà có thể chạm để mở, bên trong hiện lời nhắn “RA CỔNG ĐỂ NHẬN QUÀ”. Ảnh được lưu cục bộ dưới định dạng WebP và được tải trước khi mở sách. Thiết bị cấu hình thấp hoặc bật tiết kiệm dữ liệu sẽ tự giảm mật độ hiệu ứng; trang cũng tôn trọng cài đặt giảm chuyển động của thiết bị. Dự án dùng HTML, CSS và JavaScript thuần.

## Xem thiệp

Mở `index.html` trực tiếp trong trình duyệt rồi chạm vào bìa. Lật bốn trang ảnh, chọn một tấm ở trang thứ năm để đọc lời chúc, rồi lật sang trang cuối và chạm hộp quà. Các ảnh được lưu trong thư mục `assets/` và hiển thị ngay trên thiết bị; không có ảnh nào được tải lên máy chủ. Nếu muốn chạy qua máy chủ cục bộ, dùng một static file server bất kỳ, ví dụ:

```sh
python -m http.server 8000
```

Sau đó truy cập `http://localhost:8000`.

## Tùy chỉnh lời chúc

Sửa `CONFIG` ở đầu `script.js`:

- `titleLines`: các dòng tiêu đề.
- `wishes`: danh sách lời chúc.
- `closing`: câu chúc kết; để chuỗi rỗng nếu không cần.
- `titleCharDelay` và `wordDelay`: tốc độ hiện chữ.

Màu sắc và bố cục có thể chỉnh trong `style.css`. Phông chữ Google Fonts cần kết nối Internet; trang có phông dự phòng khi ngoại tuyến.

## Đưa lên GitHub Pages

Trong repository, vào **Settings → Pages**, chọn nhánh muốn xuất bản và thư mục gốc (`/root`). Sau khi lưu, GitHub Pages sẽ cung cấp đường dẫn để chia sẻ tấm thiệp.
