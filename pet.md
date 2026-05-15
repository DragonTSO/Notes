---
title: Hệ Thống Đệ Tử - TurtlePet Design
tags:
  - minerua
  - turtlepet
  - tu-tien
  - design
aliases:
  - Pet Design
  - Đệ Tử Design
---

# Hệ Thống Đệ Tử - TurtlePet Design

## 1. Tổng Quan

Tại MineRua Skyblock Tu Tiên, hệ thống pet nên được định hướng lại thành **Đệ Tử**.

Đệ Tử là đồng hành đi theo chủ nhân, hỗ trợ chiến đấu, farm quái, vượt Bí Cảnh và tiến hóa sức mạnh theo thời gian. Cách gọi này hợp hơn với theme Tu Tiên so với từ `Pet` thuần túy.

Mục tiêu thiết kế:

- Chuẩn hóa TurtlePet theo style server.
- Biến pet thành một phần của hành trình tu luyện.
- Tạo danh sách Sư Đệ theo cảnh giới để dùng cho config/code sau này.
- Giữ khả năng mở rộng cosmetic, skill và event.

## 2. Định Hướng Theme

Style hiện tại của server dùng nhiều khái niệm Tu Tiên:

- Đệ Tử
- Tu Vi
- Cảnh Giới
- Đột Phá
- Bí Cảnh
- Tông Môn
- Động Phủ
- Linh Mạch
- Nhập Thần

Vì vậy TurtlePet nên tránh các tên lệch theme như anime hoặc tên nhân vật ngoại truyện. Nếu vẫn giữ để không mất dữ liệu player, nên xem chúng là cosmetic cũ/event cũ, còn hướng mới cần dùng tên Việt hóa Tu Tiên.

Tên gọi khuyến nghị:

| Thành phần | Tên player-facing |
| :--- | :--- |
| Pet | Đệ Tử |
| Pet collection | Đệ Tử Các |
| Cosmetic | Chân Hồn |
| Cosmetic item | Ấn Chân Hồn |
| Equip pet | Xuất Chiến |
| Unequip pet | Thu Hồi |
| Evolve pet | Đột Phá Đệ Tử |
| Pet skill | Tuyệt Kỹ |

## 3. Hệ Tier Hiện Tại

TurtlePet hiện đang có 8 tier từ `0` đến `7`, tương ứng `E -> SSS`.

Đề xuất đổi display name cho hợp Tu Tiên:

| Tier | Tên cũ | Tên mới | Vai trò |
| :--- | :--- | :--- | :--- |
| 0 | E / Thường | Đệ Tử Ngoại Môn | nhập môn |
| 1 | D / Hiếm | Đệ Tử Nội Môn | early game |
| 2 | C / Siêu Hiếm | Tinh Anh Đệ Tử | farm ổn định |
| 3 | B / Sử Thi | Chân Truyền Đệ Tử | mid game |
| 4 | A / Tinh Anh | Hộ Đạo Đệ Tử | mid-late game |
| 5 | S / Cực Phẩm | Linh Anh Hộ Pháp | late game |
| 6 | SS / Huyền Thoại | Tiên Linh Hộ Pháp | late/endgame |
| 7 | SSS / Thần Thoại | Thần Hồn Hộ Pháp | endgame |

> [!note]
> Nếu muốn mỗi cảnh giới có một tier riêng, cần mở rộng TurtlePet từ 8 tier lên 10 tier hoặc tách hệ Sư Đệ khỏi tier hiện tại.

## 4. Danh Sách Sư Đệ Theo Cảnh Giới

Chi tiết kỹ thuật nằm trong [[sude|sude.yml]]. Bảng dưới đây là bản tóm tắt để dễ đọc.

| Cảnh Giới | Sư Đệ | Mốc Tu Vi | Vai trò |
| :--- | :--- | :--- | :--- |
| Phàm Nhân | Sư Đệ Nhập Môn | 0 | cân bằng |
| Luyện Khí | Sư Đệ Luyện Khí | 10,000 | farm |
| Trúc Cơ | Sư Đệ Trúc Cơ | 120,000 | cân bằng |
| Kim Đan | Sư Đệ Kim Đan | 750,000 | sát thương |
| Nguyên Anh | Sư Đệ Nguyên Anh | 4,000,000 | pháp thuật |
| Hóa Thần | Sư Đệ Hóa Thần | 20,000,000 | khống chế |
| Luyện Hư | Sư Đệ Luyện Hư | 85,000,000 | tốc độ / chí mạng |
| Đại Thừa | Sư Đệ Đại Thừa | 320,000,000 | hộ vệ |
| Độ Kiếp | Sư Đệ Độ Kiếp | 800,000,000 | burst damage |
| Chân Tiên | Sư Đệ Chân Tiên | 990,000,000 | endgame |

## 5. Cosmetic Chuẩn Style Server

Cosmetic nên được gọi là **Chân Hồn**. Mỗi Chân Hồn đổi ngoại hình, tên hiển thị, bonus stat và có thể gắn một skill MythicMobs.

### 5.1 Nhóm Môn Phái

Nhóm này bám theo 5 môn phái server đang có.

| ID | Tên | Hướng chơi |
| :--- | :--- | :--- |
| `kiem_tien` | Kiếm Tiên Linh Ảnh | sát thương thuần |
| `thien_co` | Thiên Cơ Linh Điệp | mana / khống chế |
| `kim_than` | Kim Thân Thạch Linh | phòng thủ |
| `linh_duoc` | Linh Dược Tiểu Tiên | hồi phục |
| `vo_anh` | Vô Ảnh Ma Miêu | tốc độ / chí mạng |

### 5.2 Nhóm Nguyên Tố

Nhóm này hợp Bí Cảnh, boss và event theo vùng.

| ID | Tên | Nguồn đề xuất |
| :--- | :--- | :--- |
| `bang_phong` | Băng Phong Linh Hồ | Bí Cảnh Băng Phong |
| `xich_viem` | Xích Viêm Kỳ Lân | Hỏa Vực / boss lửa |
| `tu_dien` | Tử Điện Lôi Linh | Thiên Lôi Kiếp |
| `huyen_vu` | Huyền Vũ Hộ Thân | event thủ hộ |
| `chu_tuoc` | Chu Tước Hỏa Vũ | event hỏa linh |

### 5.3 Nhóm Endgame

Nhóm này nên hiếm, dùng cho top player hoặc sự kiện lớn.

| ID | Tên | Ghi chú |
| :--- | :--- | :--- |
| `thanh_long` | Thanh Long Ấn | Tứ Tượng |
| `bach_ho` | Bạch Hổ Sát Ý | Tứ Tượng |
| `chan_tien` | Chân Tiên Uy Linh | cảnh giới cuối |
| `hong_mong` | Hồng Mông Hộ Pháp | cosmetic cực hiếm |

## 6. Định Hướng Triển Khai

Có ba hướng triển khai:

1. Giữ cosmetic cũ, thêm cosmetic Tu Tiên mới.
2. Đổi tên cosmetic cũ sang style Tu Tiên nhưng giữ ID cũ.
3. Xóa hẳn hệ cũ, thay bằng bộ cosmetic Tu Tiên mới.

Khuyến nghị chọn hướng 1 trước vì an toàn dữ liệu player. Sau khi player quen với bộ mới, có thể migrate hoặc ẩn dần cosmetic cũ.

## 7. Lộ Trình Đề Xuất

### Giai đoạn 1: Design

- Tạo `sude.yml` làm nguồn thiết kế Sư Đệ.
- Tạo `pet.md` làm tài liệu tổng quan.
- Chốt tên, role, stat và nguồn mở khóa.

### Giai đoạn 2: Config TurtlePet

- Thêm các cosmetic Tu Tiên vào `config.yml`.
- Việt hóa `messages.yml` từ Pet sang Đệ Tử.
- Sửa `pet_menu.yml` thành Đệ Tử Các.
- Sửa `pet_evolve.yml` thành Đột Phá Đệ Tử.

### Giai đoạn 3: Skill và Test

- Đọc lại MythicMobs skills hiện có.
- Tạo skill còn thiếu cho từng Chân Hồn.
- Reload TurtlePet hoặc restart server.
- Test mở menu, trang bị, tiến hóa, áp dụng cosmetic, đánh quái và nhận stat.

## 8. Ghi Chú Kỹ Thuật

- `sude.yml` hiện là file design riêng, plugin chưa bắt buộc đọc.
- TurtlePet hiện chỉ có 8 tier, trong khi hệ cảnh giới có 10 mốc lớn.
- Đại Thừa, Độ Kiếp và Chân Tiên có thể cùng dùng tier `7`, nhưng khác cosmetic, stat và skill.
- Nếu muốn 10 tier thật, cần sửa code TurtlePet hoặc mở rộng cấu hình tier.
- Các skill như `LinhKhiTram`, `KimDanNo`, `DoKiepThienLoi` cần kiểm tra/tạo trong MythicMobs trước khi đưa vào runtime.

## 9. Nguyên Tắc Style

- Ưu tiên tiếng Việt player-facing.
- Giữ nguyên ID kỹ thuật không dấu, snake_case.
- Dùng màu hex gradient giống DeluxeMenus khi hiển thị tên đẹp.
- Lore nên ngắn, có hình ảnh Tu Tiên, không quá dài.
- Tránh tên nhân vật anime nếu không phải event riêng.
