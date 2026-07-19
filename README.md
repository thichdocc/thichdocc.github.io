# Template GitHub Pages cho truyện ngôn tình cổ đại

## 1. Cách dùng nhanh

1. Tạo repository tên `ten-tai-khoan.github.io`.
2. Chép toàn bộ các file trong bộ template này vào repository.
3. Mở `_config.yml` và thay:
   - `url`
   - `title`
   - `affiliate_url`
4. Vào **Settings → Pages** trên GitHub.
5. Chọn **Deploy from a branch**, branch `main`, thư mục `/root`.

## 2. Cấu trúc mỗi truyện

Mỗi truyện nằm trong một thư mục riêng:

```text
ten-truyen/
├── gioithieu.md
├── chuong-1.md
├── chuong-2.md
└── chuong-3.md
```

Địa chỉ sau khi xuất bản:

```text
https://site.github.io/ten-truyen/gioithieu/
https://site.github.io/ten-truyen/chuong-1/
https://site.github.io/ten-truyen/chuong-2/
```

## 3. Tạo truyện mới

Sao chép thư mục `ten-truyen-mau`, đổi tên thư mục và sửa các trường đầu mỗi file.

Ví dụ trong một chương:

```yaml
---
layout: chapter
title: "Tên chương"
story_title: "Tên truyện"
chapter_number: 3
permalink: /ten-truyen/chuong-3/
intro_url: /ten-truyen/gioithieu/
prev_url: /ten-truyen/chuong-2/
next_url: /ten-truyen/chuong-4/
---
```

Popup affiliate tự xuất hiện khi người đọc bấm sang chương tiếp theo ở cuối chương 3, 6, 9... dựa trên `chapter_number`.

## 4. Thay link affiliate toàn website

Chỉ sửa một dòng trong `_config.yml`:

```yaml
affiliate_url: "https://s.shopee.vn/LINK-CUA-BAN"
```

Tất cả popup trên website sẽ tự dùng link mới.

## 5. Lưu ý

- Nút tiếp tục đọc luôn hiển thị rõ.
- Link affiliate mở ở tab mới.
- Nên công khai đây là liên kết tiếp thị liên kết.
- Có thể đổi màu sắc trong `assets/css/style.css`.
