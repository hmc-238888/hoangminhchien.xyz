# HMC HUB Company — Website

Website cá nhân của Hoàng Minh Chiến kết hợp giới thiệu HMC HUB Company.
Thuần HTML/CSS/JS, không framework, chạy trên GitHub Pages với domain riêng `hoangminhchien.xyz`.

## Cấu trúc file

```
index.html          # Toàn bộ trang (HTML + CSS + JS)
CNAME               # Domain riêng cho GitHub Pages
favicon.png / favicon-32.png / apple-touch-icon.png   # Icon từ logo HMC HUB
avatar.jpg / avatar.webp                              # Ảnh đại diện Hoàng Minh Chiến
logo.png / logo.webp                                  # Logo HMC HUB Company (đầy đủ)
robots.txt
sitemap.xml
```

## Cách deploy lên GitHub Pages với domain riêng

1. Tạo repo GitHub mới (ví dụ `hmc-hub-website`), push toàn bộ các file trong thư mục này lên nhánh `main`.
2. Vào **Settings → Pages** của repo → chọn nguồn build là nhánh `main`, thư mục `/ (root)`.
3. File `CNAME` đã có sẵn nội dung `hoangminhchien.xyz` — GitHub Pages sẽ tự nhận domain này, không cần tạo lại.
4. Sang phần quản lý DNS của domain `hoangminhchien.xyz` (nơi bạn mua domain), thêm bản ghi:
   - Loại `A` trỏ `@` tới 4 IP của GitHub Pages:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - (Tuỳ chọn) bản ghi `CNAME` cho `www` trỏ về `<username>.github.io`
5. Quay lại **Settings → Pages**, tick **Enforce HTTPS** sau khi DNS đã trỏ xong (có thể mất vài phút đến vài giờ để chứng chỉ SSL được cấp).
6. Kiểm tra lại các link Facebook / Discord / Email trong `index.html` (đang là placeholder) và thay bằng link thật của bạn trước khi công khai.

## Cần thay thế trước khi public

- Link Facebook cá nhân thật (hiện: `facebook.com/hoangminhchien`)
- Link Discord Server thật (hiện: `discord.gg/hmchub`)
- Email thật (hiện: `contact@hoangminhchien.xyz`)
