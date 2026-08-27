ĐUA VỊT ONLINE — bản tách assets (nhẹ để deploy)
=================================================

Cấu trúc:
  index.html            (~110 KB, toàn bộ code)
  assets/sprites/*.png   (nhân vật vịt/rùa/thỏ theo 3 theme)
  assets/bg/*.jpg        (nền 3 theme)
  assets/audio/*.mp3     (trống, chúc mừng, vỗ tay)

CÁCH DEPLOY
- Upload NGUYÊN thư mục này (index.html + thư mục assets/) lên bất kỳ static host nào
  (Netlify, Vercel, Cloudflare Pages, GitHub Pages, hosting thường, S3...).
- Truy cập index.html là chạy. Đường dẫn asset là tương đối nên không cần cấu hình gì.

XEM THỬ Ở MÁY (localhost)
- Cần chạy qua HTTP server (không mở trực tiếp bằng double-click file://,
  vì trình duyệt chặn tải mp3 qua file://).
- Ví dụ: mở terminal trong thư mục này rồi chạy:  python -m http.server 8000
  sau đó vào http://localhost:8000
- Nếu vẫn mở bằng file:// thì game vẫn chạy được, chỉ 3 tiếng mp3 sẽ tự thay bằng
  âm thanh tổng hợp dự phòng (không lỗi).

GHI CHÚ
- Font chữ lấy từ Google Fonts (cần internet). Không có mạng thì tự dùng font hệ thống.
---
