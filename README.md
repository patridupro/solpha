# SOLPHA — SOL/USDT Perpetual Desk

PWA theo dõi SOL/USDT futures đa khung (5M, 15M, 1H, 4H, 1D), RSI / EMA / Bollinger, cảnh báo khi **đồng pha + chạm band**.

## Deploy lên Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/patridupro/solpha)

1. Bấm nút trên (hoặc vào app.netlify.com → **Add new site → Import an existing project → GitHub** → chọn repo `patridupro/solpha`).
2. Build command: để trống. Publish directory: `.` (đã cấu hình sẵn trong `netlify.toml`).
3. Bấm **Deploy site** → Netlify cấp domain dạng `https://<tên-ngẫu-nhiên>.netlify.app`, mở bằng Chrome là xem được ngay.
4. Mỗi lần push lên nhánh `main`, Netlify tự build lại và deploy lại.

## Bật GitHub Pages (một lần)
1. Repo **Settings → Pages**
2. Source: **GitHub Actions** (hoặc Deploy from branch `main` / root)
3. Mở: https://patridupro.github.io/solpha/

## Cài lên Chrome
1. Mở link Pages bằng Chrome.
2. Thanh địa chỉ → **Cài đặt ứng dụng**, hoặc menu Chrome → Cast, save and share → Install page as app.
3. Trong app bấm **Bật cảnh báo**. Giữ cửa sổ app mở để quét mỗi giờ và mỗi 5 phút.

## Rule
- Đồng pha = 1D + 4H + 1H cùng hướng, 15M không ngược mạnh.
- Cảnh báo khi đồng pha và chạm BB trên ≥2 khung, có ≥1 khung ≥1H.
- Không phải tư vấn tài chính. Tự quản size/leverage.
