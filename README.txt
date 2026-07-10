Bộ GitHub Pages cho web Viễn Đông.

File chính:
- index.html

Favicon:
- favicon.png
- favicon.ico

Bản index.html đã nhúng favicon dạng base64, nên chỉ cần upload index.html cũng đổi được icon tab.
Nếu muốn dùng file favicon rời, upload thêm favicon.png/favicon.ico vào cùng thư mục repo.

API_BASE_URL hiện tại:
https://script.google.com/macros/s/AKfycbxvZz9InMwT-j9RenWiCL9HF0e5sbpvX9Etk6ljtZxpBGe6l9gP09u-Yqcpbm4aVUJy/exec

Nếu web GitHub không tải album/logo/nền:
- Mở index.html, tìm dòng:
  const API_BASE_URL = '...';
- Dán link Apps Script Web App dạng /exec vào đó.
- Apps Script cần deploy New version sau khi thay Code.gs.

Đổi favicon thủ công:
Trong <head>, thay link rel="icon" bằng:
<link rel="icon" type="image/png" href="favicon.png?v=5">
<link rel="apple-touch-icon" href="favicon.png?v=5">

Nếu icon tab chưa đổi ngay, đổi ?v=5 thành ?v=6 hoặc Ctrl+Shift+R.
