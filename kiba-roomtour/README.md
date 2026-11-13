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

## Bản phối cảnh nội thất

[Xem / tải roomtour với nội thất gợi ý](renders/kiba-roomtour-styled.mp4).

Bản này kết hợp cảnh quay hiện trạng với ảnh phối cảnh AI được tạo từ các khung hình thật, thêm chuyển động nhẹ và hòa cảnh theo nhạc. Các cảnh phối nội thất đều ghi **PHỐI CẢNH NỘI THẤT GỢI Ý** trên video. Đây là ý tưởng trang trí, không phải xác nhận nội thất đã có trong phòng hoặc bản vẽ có đo đạc kích thước.

- Trên gác: nệm thấp, chăn ga kem, điểm nhấn sage, đèn ấm, giữ khoảng trống tại lối lên.
- Dưới phòng: bàn nhỏ kiêm làm việc/ăn uống, ghế gọn, giỏ đựng đồ.
- Góc bếp: tận dụng kệ sẵn có, đồ dùng nhỏ và giỏ chứa đồ.

Nguồn dựng: `styled.html`, `edit-styled.json`, `assets/staged-*.png`. Bản hiện trạng trước đó vẫn ở `index.html` và `renders/kiba-roomtour-final.mp4`.

```sh
npx --yes hyperframes@0.9.41 render --composition styled.html --output renders/kiba-roomtour-styled.mp4 --quality high
```
