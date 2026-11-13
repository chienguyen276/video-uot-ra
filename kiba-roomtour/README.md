# Kiba Livingspace · Thủ Đức — Roomtour

Video roomtour khung dọc 9:16, dài 42,2 giây. Note tiếng Việt với phong cách nhẹ nhàng, màu kem và xanh sage. Nhạc được tách từ video do chủ dự án cung cấp; các điểm hòa cảnh được căn theo điểm nhấn của nhạc.

## Xem và tải video

[Video roomtour hoàn chỉnh có nhạc](renders/kiba-roomtour-final.mp4)

Mở file trên rồi chọn **Download raw file** để tải bản MP4 720 × 1280, 30 fps, H.264/AAC.

## Chỉnh sửa

- `index.html`: bố cục, note và hiệu ứng GSAP trong HyperFrames.
- `edit.json`: thứ tự clip, điểm cắt và nội dung note.
- `assets/`: các clip nguồn đã chọn, font và nhạc tách.
- `DESIGN.md`: màu sắc và hướng thiết kế.
- `renders/kiba-roomtour-final.mp4`: bản xuất hoàn chỉnh.

Yêu cầu Node.js 22+, FFmpeg và Chromium/Chrome.

```sh
npm run check
npm run dev
npm run render -- --output renders/kiba-roomtour-final.mp4 --quality high
```

Kiểm tra bản hiện tại: runtime, bố cục, chuyển động, tương phản chữ và âm thanh đều đạt. Nhạc vào nhẹ 0,35 giây, nhỏ dần trong 1,5 giây cuối.
