# Nhật ký chúc mừng 20/10

Một cuốn sách tương tác mừng Ngày Phụ nữ Việt Nam 20/10. Bốn trang đầu lần lượt mở bốn tấm ảnh có sẵn; ở trang cuối, người nhận chọn một trong bốn ảnh để mở lời chúc đặc biệt, được bao quanh bởi các tranh chibi. Ảnh được lưu cục bộ dưới định dạng WebP đã tối ưu và được tải trước khi mở sách để lật trang nhanh hơn. Thiết bị cấu hình thấp hoặc bật tiết kiệm dữ liệu sẽ tự giảm mật độ hiệu ứng để trang chạy nhẹ hơn. Chữ hiện dần, hoa nở, cánh hoa bay và hiệu ứng lấp lánh. Dự án dùng HTML, CSS và JavaScript thuần, không cần cài thư viện hay tải ảnh từ bên ngoài.

## Xem thiệp

Mở `index.html` trực tiếp trong trình duyệt rồi chạm vào bìa. Lật lần lượt bốn trang ảnh, sau đó chọn một trong bốn tấm ở trang cuối để mở lời chúc. Các ảnh được lưu trong thư mục `assets/` và hiển thị ngay trên thiết bị; không có ảnh nào được tải lên máy chủ. Nếu muốn chạy qua máy chủ cục bộ, dùng một static file server bất kỳ, ví dụ:

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
