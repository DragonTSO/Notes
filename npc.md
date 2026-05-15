---
title: NPC và Khu Chức Năng - MineRua Tu Tiên
tags:
  - minerua
  - npc
  - tu-tien
  - gameplay-doc
aliases:
  - NPC Tu Tiên
  - Khu NPC
---

# NPC và Khu Chức Năng - MineRua Tu Tiên

Tài liệu này ghi lại NPC, hologram và khu chức năng đang thấy từ server `01e721c5`, đối chiếu với notes Tu Tiên cũ trong vault.

> [!note]
> Nguồn chắc chắn: `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml`, `DeluxeMenus` và notes cũ. Khu nào có hologram nhưng chưa thấy NPC riêng trong config sẽ được ghi rõ là cần kiểm tra ingame.

## Tổng Quan Nhanh

| Khu | Hologram khu | Chức năng chính | Lệnh nổi bật | Trạng thái NPC |
| :--- | :--- | :--- | :--- | :--- |
| K1 | `spawn_island` | Tiên Đảo / Island | `/tiendao`, `/is panel`, `/is home`, `/gen` | Có NPC Tiên Đảo |
| K2 | `spawn_luyenky` | Luyện Khí / chọn hướng nhân vật | `/monphai`, `/class` | Có NPC Môn Phái ở spawn/tutorial; chưa thấy NPC riêng tại K2 |
| K3 | `spawn_tuluyen` | Tu luyện lấy Tu Vi, Đệ Tử, Nhập Thần | `/tuluyen`, `/pet`, `/dode` | Chưa thấy NPC riêng tại K3 |
| K4 | `spawn_dungeon` | Thí Luyện / Bí Cảnh / Dungeon | `/warp dungeon`, `/warps` | Chưa thấy NPC dungeon riêng tại K4 |
| K5 | `spawn_dotpha_chuyensinh` | Đột Phá / Chuyển Sinh | `/dotpha` | Chưa thấy NPC riêng tại K5 |

## Khu 1 - Tiên Đảo

Khu 1 là nơi người chơi bắt đầu vòng lặp Skyblock Tu Tiên: mở Tiên Đảo, về đảo, nâng cấp máy sinh quặng và tích tài nguyên để nuôi tiến trình tu luyện.

```text
spawn_island: 1. TIÊN ĐẢO (ISLAND) [K1]
World: test
Tọa độ: x -1719.129, y 130.860, z -749.891
```

### NPC Tiên Đảo - `TienDaoNPC2`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `TienDaoNPC2` |
| Hologram liên quan | `TienDaoNPC2` |
| Plugin/nguồn config | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/tọa độ | `test`, x `-1718.258`, y `83.0`, z `-792.506` |
| Lệnh hoặc action | Click chạy `tiendao` bằng `player_command` |
| Vai trò gameplay | Mở giao diện Tiên Đảo để người chơi quản lý đảo và bắt đầu farm tài nguyên |
| Điều kiện xuất hiện/mở khóa | Không thấy điều kiện trong NPC config |
| Ghi chú đặt map | NPC nằm gần vùng K1 theo trục khu spawn; hologram khu là bảng lớn chỉ hướng |

Lệnh liên quan từ menu hướng dẫn:

| Lệnh | Công dụng |
| :--- | :--- |
| `/is panel` | Mở menu Island |
| `/is home` | Về đảo cá nhân |
| `/is visit <tên>` | Thăm đảo người chơi khác |
| `/is top` | Xem bảng xếp hạng đảo |
| `/gen` | Mở nâng cấp generator, gồm Linh Mạch và Generator Ore |

### NPC Tiên Đảo Tutorial - `TienDaoNPC`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `TienDaoNPC` |
| Hologram liên quan | `TienDaoNPC` |
| Plugin/nguồn config | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/tọa độ | `tutorial`, x `146.469`, y `136.0`, z `-96.752` |
| Lệnh hoặc action | Click chạy `tiendao` bằng `player_command` |
| Vai trò gameplay | Bản tutorial của NPC Tiên Đảo, dùng để giới thiệu hệ đảo trước khi người chơi vào vòng lặp chính |
| Điều kiện xuất hiện/mở khóa | Không thấy điều kiện trong NPC config |

## Khu 2 - Luyện Khí

Khu 2 đại diện cho bước người chơi định hình nhân vật: chọn môn phái/class, lấy vũ khí đầu tiên và bắt đầu hệ Luyện Khí. Notes cũ ghi khi đạt Luyện Khí người chơi chọn một trong 5 hướng: Kiếm Tiên, Thiên Cơ, Kim Thân, Linh Dược, Vô Ảnh.

```text
spawn_luyenky: 2. LUYỆN KHÍ [K2]
World: test
Tọa độ: x -1724.897, y 94.860, z -838.962
```

### NPC Môn Phái - `Spawn_Class`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `Spawn_Class` |
| Hologram liên quan | `Spawn_Class` |
| Plugin/nguồn config | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/tọa độ | `test`, x `-1719.171`, y `110.0`, z `-714.183` |
| Lệnh hoặc action | Click chạy `monphai` bằng `player_command` |
| Vai trò gameplay | Mở chọn Môn Phái/Class, định hướng lối chơi và stat chính |
| Điều kiện xuất hiện/mở khóa | Notes cũ ghi chọn class tại Cảnh Giới 2 Luyện Khí; config NPC không thấy điều kiện khóa |
| Ghi chú đặt map | NPC ở vùng spawn/test, không nằm trực tiếp tại tọa độ hologram K2; cần check ingame xem có được dùng như cổng vào K2 không |

### NPC Chọn Môn Phái Tutorial - `ChonMonPhai`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `ChonMonPhai` |
| Hologram liên quan | `ChonMonPhai`, `Tutorial_1_MonPhai` |
| World/tọa độ | `tutorial`, x `-22.595`, y `68.0`, z `11.936` |
| Lệnh hoặc action | Click chạy `monphai` bằng `player_command` |
| Vai trò gameplay | Bắt người chơi chọn môn phái đầu tiên trong tutorial |
| Ghi chú đặt map | Hologram `Tutorial_1_MonPhai` ghi: `Hãy chọn môn phái đầu tiên của bạn` |

### NPC Lấy Vũ Khí - `ChonVuKhi`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `ChonVuKhi` |
| Hologram liên quan | `ChonVuKhi`, `Tutorial_2_VuKhi` |
| World/tọa độ | `tutorial`, x `-22.470`, y `68.0`, z `33.332` |
| Lệnh hoặc action | Click chạy console command `chonvukhi {player}` |
| Vai trò gameplay | Phát vũ khí đầu tiên theo môn phái đã chọn |
| Ghi chú đặt map | Hologram `Tutorial_2_VuKhi` ghi: `Hãy lấy vũ khí theo phái của bạn` |

### Hologram Luyện Khí Tutorial - `LuyenKhi`

Không thấy NPC link trực tiếp, nhưng hologram mô tả bước dùng Linh Thạch để luyện khí:

```text
Hãy dùng Linh Thạch của bạn
để luyện khí, tích cực luyện khí = trang bị
NGON!!!
```

## Khu 3 - Tu Luyện

Khu 3 là vòng lặp lấy Tu Vi và tăng sức mạnh lâu dài: `/tuluyen`, hệ Đệ Tử, Nhập Thần và thông tin cá nhân. Notes cũ mô tả Tu Vi là kinh nghiệm tu luyện chính, dùng để đạt mốc cảnh giới và đủ điều kiện đột phá.

```text
spawn_tuluyen: 3. TU LUYỆN [K3]
World: test
Tọa độ: x -1726.807, y 94.860, z -902.516
```

### Tình Trạng NPC K3

Chưa thấy NPC riêng đặt trực tiếp tại K3 trong `FancyNpcs/npcs.yml`. Các chức năng liên quan đang được mở qua menu/lệnh:

| Chức năng | Lệnh/menu | Nguồn |
| :--- | :--- | :--- |
| Tu Luyện | `/tuluyen` | `huongdan_menu.yml` item `tu_luyen` |
| Thông tin bản thân | `/info` hoặc NPC `Spawn_Infomation` | `FancyNpcs`, `FancyHolograms` |
| Đệ Tử | `/pet`, alias `/dode` | `huongdan_menu.yml`, `TurtlePet/command.yml` |
| Nhập Thần | Tìm NPC Nhập Thần ở Spawn | `huongdan_menu.yml` ghi có NPC, nhưng chưa thấy NPC tương ứng trong `FancyNpcs/npcs.yml` |

### NPC Thông Tin - `Spawn_Infomation`

| Trường | Nội dung |
| :--- | :--- |
| Tên NPC | `Spawn_Infomation` |
| Hologram liên quan | `Spawn_Information` |
| World/tọa độ | `test`, x `-1713.181`, y `110.0`, z `-714.339` |
| Lệnh hoặc action | Click chạy console command `dm open info_menu %player_name%` |
| Vai trò gameplay | Cho người chơi xem hồ sơ tu sĩ: rank, Linh Thạch, Cổ Thạch, môn phái, cảnh giới, Tu Vi |
| Ghi chú đặt map | Nên đặt gần spawn/hướng dẫn để người chơi kiểm tra tiến trình trước khi sang K3/K5 |

### Gợi Ý NPC Cần Có Cho K3

| NPC đề xuất | Lệnh | Lý do |
| :--- | :--- | :--- |
| NPC Tu Luyện | `/tuluyen` | Hologram K3 đã có nhưng chưa thấy NPC mở trực tiếp |
| NPC Đệ Tử | `/pet` hoặc `/dode` | Hệ Đệ Tử là phần progression quan trọng theo notes `pet.md` |
| NPC Nhập Thần | menu Nhập Thần hoặc lệnh plugin tương ứng | Menu hướng dẫn nói có NPC Nhập Thần ở Spawn, nhưng config hiện chưa thấy |

## Khu 4 - Thí Luyện Dungeon

Khu 4 là khu Bí Cảnh/Thí Luyện để người chơi đánh quái, boss, farm trang bị hiếm và nguyên liệu như Đột Phá Đan. Notes cũ mô tả dungeon mở dần theo cảnh giới và thực lực.

```text
spawn_dungeon: 4. THÍ LUYỆN (DUNGEON) [K4]
World: test
Tọa độ: x -1730.229, y 94.860, z -960.841
```

### Tình Trạng NPC K4

Chưa thấy NPC dungeon riêng trong `FancyNpcs/npcs.yml`. Người chơi hiện được hướng qua menu warp:

| Chức năng | Lệnh/menu | Nguồn |
| :--- | :--- | :--- |
| Mở menu warp | `/warps`, `/warp` | `warp_menu.yml` |
| Vào dungeon | `/warp dungeon` | `warp_menu.yml` item `warp_dungeon` |
| Hướng dẫn Bí Cảnh | item `Bí Cảnh` trong `/huongdan` | `huongdan_menu.yml` |

Dungeon chính từ notes cũ:

| Tầng | Tên | Yêu cầu gợi ý |
| :--- | :--- | :--- |
| 1 | Yêu Thú Lâm | Luyện Khí Sơ Kỳ, thực lực 500 |
| 2 | Âm Hồn Động | Luyện Khí Hậu Kỳ, thực lực 1,500 |
| 3 | Hỏa Diễm Sơn | Trúc Cơ Sơ Kỳ, thực lực 3,000 |
| 4 | Băng Phong Cốc | Trúc Cơ Hậu Kỳ, thực lực 6,000 |

### Gợi Ý NPC Cần Có Cho K4

| NPC đề xuất | Lệnh/action | Lý do |
| :--- | :--- | :--- |
| NPC Bí Cảnh | `/warp dungeon` hoặc menu dungeon riêng | Khu K4 đã có hologram nhưng thiếu NPC tương tác |
| NPC Bảng Tầng | mở danh sách dungeon theo cảnh giới | Giúp người chơi biết tầng nào phù hợp với cảnh giới/thực lực |

## Khu 5 - Đột Phá và Chuyển Sinh

Khu 5 là điểm người chơi kiểm tra điều kiện, kích hoạt đột phá và xử lý các hệ reset/nâng giới hạn như chuyển sinh. Notes cũ mô tả Đột Phá là bước sống sót qua Thiên Lôi Kiếp để lên cảnh giới mới.

```text
spawn_dotpha_chuyensinh: 5. ĐỘT PHÁ - CHUYỂN SINH [K5]
World: test
Tọa độ: x -1723.166, y 94.860, z -1020.303
```

### Tình Trạng NPC K5

Chưa thấy NPC Đột Phá/Chuyển Sinh riêng trong `FancyNpcs/npcs.yml`. Chức năng đang được hướng dẫn qua menu:

| Chức năng | Lệnh/menu | Nguồn |
| :--- | :--- | :--- |
| Đột Phá | `/dotpha` | `huongdan_menu.yml` item `tu_luyen` |
| Tu Luyện trước khi đột phá | `/tuluyen` | `huongdan_menu.yml` |
| Xem hồ sơ/tiến trình | `info_menu`, NPC `Spawn_Infomation` | `FancyNpcs`, `huongdan_menu.yml` |

Điều kiện theo notes cũ:

| Điều kiện | Ghi chú |
| :--- | :--- |
| Đủ Tu Vi | Người chơi đạt mốc cảnh giới tiếp theo |
| Đủ điều kiện đột phá | Có thể gồm cảnh giới, thực lực, vật phẩm hoặc cooldown tùy config thực tế |
| Sống sót Thiên Lôi Kiếp | Thành công thì lên cảnh giới; thất bại có hình phạt/cooldown |

### Gợi Ý NPC Cần Có Cho K5

| NPC đề xuất | Lệnh/action | Lý do |
| :--- | :--- | :--- |
| NPC Đột Phá | `/dotpha` | Khu K5 đã có hologram nhưng thiếu NPC tương tác |
| NPC Chuyển Sinh | menu/lệnh chuyển sinh thực tế | Hologram ghi `Chuyển Sinh`, nhưng chưa thấy config/lệnh tương ứng |
| NPC Kiểm Tra Điều Kiện | mở hồ sơ hoặc checklist | Giảm nhầm lẫn trước khi người chơi kích hoạt thiên kiếp |

## NPC Spawn Chung

Các NPC này không gắn trực tiếp với K1-K5 trong hologram khu, nhưng là hub chức năng quan trọng.

| NPC | Hologram | World/tọa độ | Action | Vai trò |
| :--- | :--- | :--- | :--- | :--- |
| `Spawn_Menu` | `Spawn_Menu` | `Spawn`, x `1000.5`, y `65.0`, z `1018.5` | Player command `menu` | Mở menu chính server |
| `Spawn_HuongDan` | `Spawn_Huongdan` | `test`, x `-1725.800`, y `110.0`, z `-714.738` | Player command `huongdan` | Mở hướng dẫn MineRua |
| `Spawn_Shop` | `Spawn_Shop` | `Spawn`, x `1007.5`, y `64.0`, z `1007.5` | Không thấy action trong NPC config | Cửa hàng `/shop` theo hologram |
| `Spawn_AH` | `Spawn_AH` | `Spawn`, x `986.963`, y `65.0`, z `1017.904` | Không thấy action trong NPC config | Thiên Bảo Các `/ah` theo hologram |
| `Spawn_Quest` | `Spawn_Quest` | `Spawn`, x `992.5`, y `65.0`, z `1017.5` | Không thấy action trong NPC config | Nhiệm vụ `/quest` theo hologram |
| `Spawn_Team` | `Spawn_Team` | `Spawn`, x `1008.5`, y `65.0`, z `1016.5` | Không thấy action trong NPC config | Liên minh/Tông Môn, liên quan `/team` |

## Hologram Không Gắn NPC

| Hologram | Nội dung | Ghi chú |
| :--- | :--- | :--- |
| `Welcome_title` | Logo/ảnh title tại Spawn | Trang trí chào mừng |
| `Welcome` | Giới thiệu thế giới Tu Tiên | Có mô tả Dungeon, Đồ Đệ, Trang Bị, Lực Chiến |
| `TOP_Money` | Đua top địa chủ/money | Bảng top kinh tế |
| `TOP_Kills` | Đua top thợ săn/kills | Bảng top PvP/kills |
| `Spawn_Huongdan2` | Dấu `?` lớn | Chỉ dẫn phụ tại Spawn, không link NPC |
| `Tutorial_1_BuNhin` | Đánh bại 5 bù nhìn để tiếp tục | Bước combat tutorial |

## Thiếu Dữ Liệu Cần Check Ingame

| Mục | Lý do cần check |
| :--- | :--- |
| NPC K2 đặt trực tiếp tại hologram `spawn_luyenky` | Config chỉ thấy NPC Môn Phái ở vùng spawn/test và tutorial, chưa thấy NPC riêng tại tọa độ K2 |
| NPC K3 Tu Luyện/Đệ Tử/Nhập Thần | Menu hướng dẫn có chức năng, nhưng `FancyNpcs` chưa có NPC tương ứng |
| NPC K4 Dungeon | Hologram K4 có khu, nhưng menu hiện dùng `/warp dungeon`; chưa thấy NPC dungeon riêng |
| NPC K5 Đột Phá/Chuyển Sinh | Hologram K5 có khu, nhưng chưa thấy NPC riêng hoặc lệnh chuyển sinh trong dữ liệu đã đọc |
| Action của `Spawn_Shop`, `Spawn_AH`, `Spawn_Quest`, `Spawn_Team` | Hologram có lệnh hiển thị, nhưng NPC config chưa có click action |
| File gameplay server đầy đủ | `/plugins/TuTienCore/gameplay.md` bị truncate trong lần đọc trước, nên chưa dùng làm nguồn chính |
