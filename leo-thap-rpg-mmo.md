# 🏰 FurrMC — Gameplay Chế Độ Leo Tháp RPG MMO

> **Thể loại:** RPG MMO / Boss Rush / Khám phá cốt truyện  
> **Trọng tâm:** 50% cốt truyện, 50% khám phá  
> **Tiến trình chính:** Leo 20 khu tháp, đánh boss, tiến hóa trang bị, chọn nền văn minh ở cấp 20  
> **Triết lý:** Đổi mới, dễ tiếp cận, không shop trader, không vanilla mod, dùng resource/mod pack 100%

---

## 📋 Mục Lục

1. [Tổng Quan](#1-tổng-quan)
2. [Bộ Tài Liệu Chi Tiết](#2-bộ-tài-liệu-chi-tiết)
3. [Vòng Lặp Gameplay Chính](#3-vòng-lặp-gameplay-chính)
4. [Cấu Trúc Tháp 20 Khu Boss](#4-cấu-trúc-tháp-20-khu-boss)
5. [Hệ Thống Cấp Độ Và Mở Khóa](#5-hệ-thống-cấp-độ-và-mở-khóa)
6. [Tóm Tắt Các Trụ Cột](#6-tóm-tắt-các-trụ-cột)

---

## 1. Tổng Quan

**Leo Tháp RPG MMO** là chế độ PvE cốt lõi của FurrMC, nơi người chơi không đi theo kiểu sinh tồn vanilla mà bước vào một thế giới được dựng lại hoàn toàn bằng pack mod, giao diện mới, boss riêng, vật phẩm riêng và chuỗi nhiệm vụ dẫn chuyện.

Người chơi bắt đầu như một kẻ lạc vào Tháp Khởi Nguyên. Mỗi tầng là một khu vực boss độc lập, có bối cảnh, cơ chế chiến đấu, vật phẩm hiếm và mảnh cốt truyện riêng. Mục tiêu ngắn hạn là vượt boss để lên cấp. Mục tiêu dài hạn là tiến hóa trang bị, chọn nền văn minh, mở khóa lối chơi riêng và khám phá bí mật sau 20 khu tháp.

### Trụ Cột Thiết Kế

| Trụ Cột | Mô Tả |
|---|---|
| **Boss là trung tâm** | Mỗi cấp độ gắn với một boss có cơ chế riêng, không chỉ tăng máu và sát thương. |
| **Không shop trader** | Người chơi tìm vật phẩm bằng chiến đấu, khám phá, rơi đồ hiếm và farm tài nguyên. |
| **Nhân phẩm có kiểm soát** | Drop hiếm tạo cảm giác săn đồ, nhưng vẫn có nguyên liệu bảo hiểm để tiến hóa. |
| **Dễ tiếp cận** | Cấp 1-5 dạy né đòn, định vị, đọc cảnh báo, hiểu chỉ số. |
| **Đổi mới toàn diện** | Loại bỏ cảm giác vanilla bằng pack mod, HUD, menu, item, mob model, âm thanh và hiệu ứng mới. |
| **AAA trong Minecraft** | Mỗi boss có arena, phase, telegraph, nhạc nền, cinematic ngắn và loot reveal. |

---

## 2. Bộ Tài Liệu Chi Tiết

| File | Nội Dung |
|---|---|
| [`bosses.md`](bosses.md) | Thiết kế 20 boss, phase, loot, độ khó, pity. |
| [`civilizations.md`](civilizations.md) | 5 nền văn minh mở ở cấp 20, passive, skill, danh vọng. |
| [`equipment.md`](equipment.md) | Trang bị, phẩm chất, tiến hóa, loot table, set bonus. |
| [`mining.md`](mining.md) | Khu mỏ farm tài nguyên, mini event, mỏ hư không. |
| [`ui-npc-commands.md`](ui-npc-commands.md) | HUD, menu, NPC dẫn chuyện, lệnh người chơi/admin. |
| [`progression-endgame.md`](progression-endgame.md) | Tiến trình cấp 1-20, cốt truyện, daily/weekly, endgame. |

---

## 3. Vòng Lặp Gameplay Chính

```text
Nhận mốc truyện / nhiệm vụ
        ↓
Vào khu boss bằng NPC hoặc lệnh
        ↓
Học cơ chế boss, né đòn, đánh bại
        ↓
Nhận EXP, vật phẩm, nguyên liệu, mảnh truyện
        ↓
Nâng cấp / tiến hóa trang bị
        ↓
Farm khu mỏ nếu thiếu tài nguyên
        ↓
Mở khu boss tiếp theo
        ↓
Cấp 20 chọn nền văn minh và bước vào endgame
```

### Nhịp Chơi Một Ngày

| Hoạt Động | Thời Lượng | Mục Đích |
|---|---:|---|
| Đánh boss chính tuyến | 10-25 phút | Lên cấp, mở truyện, nhận loot quan trọng |
| Farm khu mỏ | 10-20 phút | Lấy đá tiến hóa, lõi cường hóa, vật liệu craft |
| Săn lại boss cũ | 10-30 phút | Tìm drop hiếm, hoàn thiện build |
| Khám phá khu phụ | 5-15 phút | Tìm rương ẩn, lore, nguyên liệu nền văn minh |
| Party boss khó | 15-40 phút | Chinh phục phase nâng cao, leaderboard, danh hiệu |

---

## 4. Cấu Trúc Tháp 20 Khu Boss

Tháp có **20 khu boss**, chia thành 4 giai đoạn. Mỗi khu không chỉ là một phòng đánh boss, mà là một tiểu vùng có đường dẫn, NPC, môi trường, rương ẩn, mob phụ và arena cuối.

| Giai Đoạn | Cấp | Vai Trò Gameplay | Mục Tiêu Thiết Kế |
|---|---:|---|---|
| **Khởi Đầu** | 1-5 | Làm quen | Dạy né đòn, định vị, hồi phục, đọc cảnh báo |
| **Thử Thách** | 6-10 | Bắt đầu build | AoE, debuff, phá giáp, phản sát thương |
| **Chinh Phục** | 11-15 | Yêu cầu trang bị | Phase rõ ràng, phối hợp kỹ năng, kiểm soát sân đấu |
| **Huyền Thoại** | 16-20 | Đỉnh cao mùa đầu | Boss nhiều phase, thay đổi địa hình, kiểm tra toàn bộ kỹ năng |

### Quy Tắc Mở Khóa

| Nội Dung | Điều Kiện |
|---|---|
| Khu boss tiếp theo | Đánh bại boss hiện tại ít nhất 1 lần |
| Chế độ khó | Đánh bại boss thường + đạt điểm trang bị khuyến nghị |
| Loot hiếm | Rơi từ boss, rương ẩn hoặc nhiệm vụ phụ, không bán trực tiếp |
| Mảnh truyện | Rơi lần đầu khi hạ boss, có thể xem lại trong nhật ký |
| Nền văn minh | Mở ở cấp 20 sau khi hạ World Ender |

---

## 5. Hệ Thống Cấp Độ Và Mở Khóa

Level trong chế độ này là **mốc tiến trình dễ hiểu**, không phải hệ tu luyện phức tạp. Người chơi nhìn vào cấp là biết mình nên đánh khu nào.

| Cấp | Mở Khóa Chính |
|---:|---|
| 1 | Tutorial, HUD mới, khu Vua Nhầy |
| 2 | Né đòn nâng cao, vật phẩm hồi phục cơ bản |
| 3 | Khiên / chặn đòn / đánh sau lưng |
| 4 | Hiệu ứng trói, giải khống chế |
| 5 | Cơ chế choáng, cảnh báo AoE lớn |
| 6 | Độc, làm chậm, vật phẩm kháng hiệu ứng |
| 7 | Tàng hình, đánh sau lưng, nghe âm thanh cảnh báo |
| 8 | Tầm xa, vùng băng, giữ khoảng cách |
| 9 | Knockback, chống hất văng |
| 10 | Phá giáp phản sát thương, build damage window |
| 11-15 | Boss phase, elite loot, trang bị bậc III |
| 16-19 | Boss huyền thoại, nguyên liệu nền văn minh |
| 20 | Chọn 1 trong 5 nền văn minh, mở endgame |

---

## 6. Tóm Tắt Các Trụ Cột

Các phần bên dưới giữ vai trò tóm tắt nhanh. Bản chi tiết đã được tách ra thành nhiều file để dễ đọc và dễ triển khai.

---

## Hệ Thống 5 Nền Văn Minh

Khi đạt **cấp 20**, người chơi chọn **1 trong 5 nền văn minh**. Đây là lựa chọn định hình endgame, không nên chọn ngay từ đầu để tránh người mới bị rối.

### 5 Nền Văn Minh

| Nền Văn Minh | Phong Cách | Vai Trò | Điểm Mạnh | Điểm Yếu |
|---|---|---|---|---|
| **Aurelia** | Đế quốc ánh sáng | Tank / Paladin | Giáp, khiên, hồi phục ổn định | Sát thương bùng nổ thấp |
| **Varkhan** | Bộ tộc chiến thú | Berserker / Melee DPS | Máu thấp càng mạnh, áp sát tốt | Dễ chết nếu né kém |
| **Myrr** | Pháp giới tinh linh | Mage / Control | AoE, khống chế, nguyên tố | Mỏng, cần giữ vị trí |
| **Noctis** | Thành bang bóng đêm | Assassin / Crit | Burst damage, né tránh, đánh sau lưng | Khó chơi, lỗi combo bị phạt nặng |
| **Eidolon** | Cổ máy hư không | Engineer / Summon | Drone, turret, khiên công nghệ | Cần quản lý tài nguyên kỹ |

### Cơ Chế Nền Văn Minh

| Thành Phần | Mô Tả |
|---|---|
| **Passive văn minh** | Nội tại vĩnh viễn, thay đổi cách chơi. |
| **Kỹ năng chủ động** | 1 skill đặc trưng, dùng trong boss endgame. |
| **Trang bị biểu tượng** | Một dòng tiến hóa riêng cho vũ khí hoặc giáp. |
| **Khu khám phá riêng** | Mỗi văn minh có khu phụ để farm nguyên liệu đặc biệt. |
| **Danh vọng** | Làm nhiệm vụ văn minh để mở cosmetic, title, lore. |

> [!IMPORTANT]
> Chọn nền văn minh là quyết định lớn. Có thể cho đổi 1 lần miễn phí trong 24 giờ đầu sau khi chọn, sau đó cần vật phẩm hiếm từ endgame để đổi.

---

## 6. Trang Bị, Tiến Hóa Và Nhân Phẩm

Không có shop trader bán thẳng vật phẩm mạnh. Sức mạnh đến từ **đánh boss, săn drop, farm mỏ và tiến hóa trang bị**.

### Phẩm Chất Trang Bị

| Phẩm Chất | Màu Gợi Ý | Nguồn Chính | Vai Trò |
|---|---|---|---|
| Common | Xám | Boss đầu, mob phụ | Dùng tạm, làm nguyên liệu |
| Rare | Xanh | Boss 1-10 | Build cơ bản |
| Epic | Tím | Boss 6-15 | Bắt đầu có dòng đặc biệt |
| Legendary | Vàng | Boss 11-20 | Trang bị chủ lực |
| Mythic | Đỏ | Drop hiếm / craft tiến hóa | Endgame |
| Relic | Cầu vồng | World Ender, văn minh | Vật phẩm biểu tượng mùa |

### Tiến Hóa Trang Bị

| Bậc | Tên | Yêu Cầu | Mở Tính Năng |
|---:|---|---|---|
| I | Thô Sơ | Drop từ boss 1-5 | Chỉ số cơ bản |
| II | Tinh Luyện | Nguyên liệu boss 6-10 + mỏ | Dòng phụ đầu tiên |
| III | Cổ Vật | Nguyên liệu boss 11-15 | Kỹ năng trang bị |
| IV | Huyền Thoại | Nguyên liệu boss 16-19 | Hiệu ứng phase / aura |
| V | Di Sản | World Ender + nền văn minh | Thay đổi lối chơi endgame |

### Nhân Phẩm Có Bảo Hiểm

| Cơ Chế | Mục Đích |
|---|---|
| Drop hiếm từ boss | Tạo cảm giác săn đồ và khoảnh khắc may mắn. |
| Mảnh boss | Nếu không rơi đồ, vẫn nhận mảnh để đổi/craft sau nhiều lần. |
| Pity mềm | Sau nhiều lần không có Legendary, tăng nhẹ tỉ lệ rơi. |
| Không bán trực tiếp | Giữ giá trị chiến đấu và khám phá. |
| Roll dòng phụ | Có thể farm để tối ưu, nhưng không bắt buộc cho người mới. |

---

## 7. Khu Mỏ Và Farm Tài Nguyên

Khu mỏ vẫn là phần quan trọng để người chơi có việc làm giữa các lần đánh boss. Mỏ không chỉ đào đá vanilla mà là vùng khai thác có quái canh giữ, sự kiện nhỏ và tài nguyên tiến hóa.

### Loại Mỏ

| Khu Mỏ | Mở Khóa | Tài Nguyên Chính | Rủi Ro |
|---|---:|---|---|
| **Mỏ Rạn Nứt** | Cấp 1 | Đá cường hóa, quặng thường | Mob yếu, sập đá nhỏ |
| **Mỏ Huyết Tinh** | Cấp 6 | Tinh thể đỏ, lõi độc | Quái độc, vùng chảy máu |
| **Mỏ Băng Tủy** | Cấp 8 | Băng ngọc, lõi kháng slow | Đóng băng, trượt chân |
| **Mỏ Lôi Thạch** | Cấp 14 | Lôi thạch, lõi tốc độ | Sét ngẫu nhiên |
| **Mỏ Hư Không** | Cấp 17 | Mảnh hư không, nguyên liệu Mythic | Dịch chuyển, ảo ảnh |

### Vai Trò Của Mỏ

| Vai Trò | Mô Tả |
|---|---|
| Bù nhân phẩm | Không rơi đồ vẫn farm được nguyên liệu tiến hóa. |
| Đổi nhịp chơi | Sau boss căng thẳng, người chơi có hoạt động nhẹ hơn. |
| Khám phá | Mỏ có đường ẩn, rương bí mật, mini event. |
| Party nhỏ | Một số mỏ có khu elite cho 2-3 người. |

---

## 8. NPC Dẫn Chuyện Và Lệnh Di Chuyển

Người chơi có thể vào khu boss bằng **NPC dẫn chuyện** hoặc **lệnh nhanh**. NPC dành cho người chơi mới và người thích cốt truyện. Lệnh dành cho người chơi đã quen.

### NPC Chính

| NPC | Vai Trò |
|---|---|
| **Người Gác Tháp** | Mở menu chọn khu boss, giải thích tiến trình. |
| **Ký Ức Sư** | Cho xem lại mảnh cốt truyện đã mở. |
| **Thợ Rèn Dị Giới** | Tiến hóa trang bị bằng nguyên liệu, không bán đồ mạnh. |
| **Người Khai Mỏ** | Dẫn tới khu mỏ phù hợp cấp độ. |
| **Sứ Giả Văn Minh** | Xuất hiện ở cấp 20, cho chọn nền văn minh. |

### Lệnh Đề Xuất

| Lệnh | Chức Năng |
|---|---|
| `/thap` | Mở menu tháp 20 khu boss. |
| `/boss <1-20>` | Vào nhanh khu boss đã mở khóa. |
| `/mo` | Mở menu khu mỏ. |
| `/trangbi` | Xem trang bị, tiến hóa, chỉ số chiến lực. |
| `/truyen` | Xem nhật ký cốt truyện và mảnh ký ức. |
| `/vanminh` | Xem/chọn nền văn minh khi đủ điều kiện. |

---

## 9. Giao Diện Người Dùng Mới

Toàn bộ UI cần thay đổi để người chơi cảm giác đây là một game RPG MMO riêng, không phải Minecraft vanilla.

### HUD Chính

| Thành Phần | Mô Tả |
|---|---|
| Thanh HP / Mana / Stamina | Hiển thị rõ tài nguyên chiến đấu. |
| Boss Bar tùy chỉnh | Tên boss, phase, trạng thái giáp, kỹ năng sắp dùng. |
| Cảnh báo AoE | Vòng đỏ, đường thẳng, hình nón trước khi boss ra đòn. |
| Quest Tracker | Mục tiêu hiện tại, khu cần đến, phần thưởng chính. |
| Loot Reveal | Hiện vật phẩm rơi theo phong cách RPG, có âm thanh và hiệu ứng. |

### Menu Chính

| Menu | Nội Dung |
|---|---|
| Tháp | 20 khu boss, trạng thái đã mở, độ khó, loot chính. |
| Trang bị | Vũ khí, giáp, phụ kiện, dòng phụ, tiến hóa. |
| Mỏ | Khu farm, tài nguyên, độ nguy hiểm. |
| Cốt truyện | Mảnh ký ức, NPC, cinematic đã mở. |
| Văn minh | Nền văn minh, passive, kỹ năng, danh vọng. |

---

## 10. Mod Pack Và Trải Nghiệm AAA

Pack mod/resource pack là bắt buộc để đạt cảm giác AAA. Vanilla mob, item và UI cần được thay thế hoặc ẩn đi tối đa.

### Thành Phần Cần Có

| Thành Phần | Mục Tiêu |
|---|---|
| Model boss riêng | Mỗi boss có hình dáng nhận diện mạnh. |
| Animation boss | Telegraph, phase change, execute, death animation. |
| Item model riêng | Vũ khí và giáp nhìn khác biệt theo phẩm chất. |
| Âm thanh riêng | Nhạc boss, âm thanh cảnh báo, âm thanh loot hiếm. |
| UI texture | Menu, nút, khung, icon, thanh tài nguyên. |
| Map texture | Arena không còn cảm giác vanilla block thô. |

### Loại Bỏ Vanilla Mod

| Vanilla Cũ | Thay Bằng |
|---|---|
| Mob vanilla thường | Mob model riêng theo khu. |
| Kiếm/giáp vanilla | Vũ khí 3D, giáp cosmetic, icon riêng. |
| Enchant vanilla lộ rõ | Dòng chỉ số RPG: Crit, Pierce, Lifesteal, Resist. |
| Villager trader | NPC dẫn chuyện/thợ rèn không bán đồ mạnh. |
| GUI chest cơ bản | GUI texture riêng, icon riêng, mô tả ngắn gọn. |

---

## 11. Danh Sách 20 Boss Theo Giai Đoạn

## Giai Đoạn 1: Khởi Đầu (Cấp 1-5)

Những boss đầu tiên dạy người chơi cách né đòn, nhìn cảnh báo, giữ vị trí và hiểu vai trò trang bị.

| Cấp | Boss | Cơ Chế Chính | Bài Học |
|---:|---|---|---|
| 1 | **Vua Nhầy** (Slime King) | Kích thước lớn, chậm, chết phân tách thành nhiều slime nhỏ. | Không đứng yên, ưu tiên dọn quái nhỏ. |
| 2 | **Sói Đầu Đàn** (Alpha Wolf) | Di chuyển nhanh, triệu hồi 2-3 sói con. | Kite, né dash, xử lý add. |
| 3 | **Đại Úy Xương** (Skeleton Captain) | Dùng kiếm và khiên, chặn đòn trực diện. | Đánh sau lưng, chờ cửa sổ phản công. |
| 4 | **Tinh Linh Rừng Già** (Forest Ent) | Hồi máu gần cây, trói chân người chơi. | Kéo boss khỏi vùng lợi thế, phá rễ trói. |
| 5 | **Hộ Vệ Đá** (Stone Golem) | Rất chậm, sát thương lớn, dậm đất gây choáng. | Đọc telegraph AoE lớn, không tham damage. |

### Boss Mốc Cấp 5: Hộ Vệ Đá

| Stat | Giá Trị Gợi Ý |
|---|---:|
| HP | 12,000 |
| Sát thương | Cao |
| Tốc độ | Rất chậm |
| Phase 2 | Dưới 35% HP, dậm đất nhanh hơn và rơi đá từ trần |

---

## Giai Đoạn 2: Thử Thách (Cấp 6-10)

Bắt đầu xuất hiện kỹ năng diện rộng, độc, làm chậm, tàng hình và phản sát thương.

| Cấp | Boss | Cơ Chế Chính | Bài Học |
|---:|---|---|---|
| 6 | **Nhện Góa Phụ** (Broodmother) | Phun tơ làm chậm, độc kéo dài. | Quản lý debuff, dùng vật phẩm kháng độc. |
| 7 | **Tướng Cướp Sa Mạc** (Desert Outlaw) | Bom khói ẩn thân, đánh sau lưng. | Nghe âm thanh, quan sát dấu chân/hiệu ứng cát. |
| 8 | **Linh Hồn Băng Giá** (Frost Wraith) | Vùng làm chậm, tia băng tầm xa. | Giữ khoảng cách hợp lý, né line attack. |
| 9 | **Nhân Mã Cuồng Nộ** (Centaur Berserker) | Càn quét, húc văng người chơi. | Đứng lệch hướng charge, tránh mép arena. |
| 10 | **Thủ Vệ Tinh Thể** (Crystal Warden) | Giáp phản sát thương, yếu khi giáp vỡ. | Dồn damage đúng thời điểm. |

### Boss Mốc Cấp 10: Thủ Vệ Tinh Thể

| Phase | Mô Tả |
|---|---|
| Phase 1 | Boss có giáp tinh thể, phản 20% sát thương nhận vào. |
| Break Window | Sau khi phá 4 tinh thể quanh sân, boss mất giáp 10 giây. |
| Phase 2 | Tinh thể mọc lại nhanh hơn, arena có laser xoay. |

---

## Giai Đoạn 3: Chinh Phục (Cấp 11-15)

Giai đoạn này yêu cầu trang bị tốt, hiểu build và biết phối hợp kỹ năng. Người chơi solo vẫn có thể qua, nhưng party sẽ dễ hơn.

| Cấp | Boss | Cơ Chế Chính | Bài Học |
|---:|---|---|---|
| 11 | **Hiệp Sĩ Bóng Đêm** (Dark Paladin) | Hút máu, vòng tròn ma thuật gây nổ. | Không đứng trong rune, ngắt hồi máu. |
| 12 | **Hỏa Long Non** (Fire Drake) | Phun lửa hình nón, tạo bãi cháy. | Quản lý vị trí arena, tránh bị khóa đường. |
| 13 | **Kẻ Săn Đêm** (Abyssal Stalker) | Làm mù màn hình, tấn công liên tục. | Dựa vào âm thanh, phản xạ, phòng thủ đúng lúc. |
| 14 | **Người Khổng Lồ Sấm Sét** (Storm Giant) | Sét đánh vị trí ngẫu nhiên quanh sân. | Di chuyển liên tục, đọc dấu sét. |
| 15 | **Pháp Sư Vong Linh** (The Lich) | Triệu hồi xương liên tục, kết liễu người thấp máu. | Dọn add, giữ máu an toàn, ưu tiên mục tiêu. |

### Boss Mốc Cấp 15: The Lich

| Kỹ Năng | Mô Tả |
|---|---|
| Quân Đoàn Xương | Gọi nhiều skeleton theo từng đợt. |
| Linh Hồn Hấp Thụ | Hút máu từ mob còn sống nếu người chơi không dọn kịp. |
| Dấu Ấn Tử Vong | Nếu người chơi dưới 25% HP, boss chuẩn bị chiêu kết liễu. |
| Phase 3 | Arena tối dần, chỉ còn vùng sáng an toàn. |

---

## Giai Đoạn 4: Huyền Thoại (Cấp 16-20)

Những boss này có nhiều phase biến thân, cinematic ngắn và cơ chế thay đổi sân đấu. Đây là phần tạo cảm giác game lớn.

| Cấp | Boss | Cơ Chế Chính | Bài Học |
|---:|---|---|---|
| 16 | **Phượng Hoàng Lửa** (Phoenix) | Hết máu hóa trứng, không phá kịp sẽ hồi sinh 50% HP. | Dồn damage theo cửa sổ ngắn. |
| 17 | **Sát Thủ Hư Không** (Void Assassin) | Dịch chuyển, tạo bản sao ảo ảnh. | Nhận diện boss thật, không phí skill. |
| 18 | **Thủy Quái Kraken** (Lurker of the Deep) | Arena nước/đầm lầy, xúc tu kéo và quất. | Kiểm soát địa hình, phá xúc tu ưu tiên. |
| 19 | **Rồng Hỗn Mang** (Chaos Dragon) | Đa nguyên tố, hơi thở xuyên giáp. | Đổi kháng nguyên tố, né sát thương chuẩn. |
| 20 | **Kẻ Hủy Diệt Thế Giới** (World Ender) | Máu khổng lồ, đổi địa hình, buộc di chuyển liên tục. | Tổng kiểm tra toàn bộ kỹ năng đã học. |

### Boss Cuối: World Ender

| Phase | Cơ Chế | Cảm Giác |
|---|---|---|
| Phase 1 | Boss đánh vật lý, gọi thiên thạch nhỏ. | Kiểm tra né cơ bản. |
| Phase 2 | Arena nứt vỡ, một số vùng rơi xuống hư không. | Bắt buộc di chuyển. |
| Phase 3 | Boss hấp thụ nguyên tố từ 4 boss trước. | Đổi nhịp liên tục. |
| Phase 4 | Trời tối, chỉ còn các trụ sáng an toàn. | Cao trào cinematic. |
| Kết thúc | Rơi lõi World Ender, mở chọn nền văn minh. | Chuyển sang endgame. |

---

## 12. Luồng Người Chơi Mới

### 0-15 Phút Đầu

1. Người chơi spawn tại **Sảnh Tháp Khởi Nguyên**.
2. NPC Người Gác Tháp giải thích ngắn: đánh boss để lên cấp, không mua đồ mạnh, trang bị đến từ chiến đấu.
3. Người chơi nhận vũ khí cơ bản theo lối chơi: kiếm, cung, trượng hoặc song đao.
4. Vào boss cấp 1 bằng NPC hoặc `/boss 1`.
5. Sau khi hạ Vua Nhầy, mở menu loot reveal và nhiệm vụ tiếp theo.

### 1 Giờ Đầu

| Mốc | Trải Nghiệm |
|---|---|
| 15 phút | Biết vào boss, né đòn, nhận loot. |
| 30 phút | Có trang bị Rare đầu tiên, hiểu tiến hóa. |
| 45 phút | Mở khu mỏ, farm nguyên liệu để nâng cấp. |
| 60 phút | Đánh boss cấp 3-4, thấy boss có cơ chế khác nhau. |

---

## 13. Retention Và Endgame

### Giữ Người Chơi Không Cần Shop Trader

| Cơ Chế | Cách Giữ Chân |
|---|---|
| Drop hiếm | Người chơi săn lại boss để tìm vũ khí đẹp/chỉ số tốt. |
| Mảnh boss | Mỗi lần đánh đều có tiến độ, không bị cảm giác phí thời gian. |
| Weekly boss modifier | Mỗi tuần boss có biến thể: độc hơn, nhanh hơn, nhiều loot hơn. |
| Leaderboard clear time | Người chơi mạnh cạnh tranh thời gian hạ boss. |
| Danh hiệu khám phá | Thưởng người tìm lore, rương ẩn, bí mật arena. |
| Văn minh endgame | Sau cấp 20 có mục tiêu dài hạn theo phe đã chọn. |

### Nội Dung Sau Cấp 20

| Nội Dung | Mô Tả |
|---|---|
| Boss Mythic | Phiên bản khó của 20 boss, thêm phase và loot Relic. |
| Chiến dịch văn minh | Mỗi văn minh có chuỗi nhiệm vụ riêng. |
| Tháp vô tận | Leo tầng ngẫu nhiên để lấy điểm mùa. |
| Raid World Ender | Party nhiều người, loot giới hạn tuần. |
| Bộ sưu tập lore | Hoàn thiện 100% cốt truyện và nhận cosmetic. |

---

## Ghi Chú Triển Khai

| Hạng Mục | Ưu Tiên |
|---|---|
| 20 boss có cơ chế riêng | Rất cao |
| HUD và menu mới | Rất cao |
| Resource/mod pack 100% | Rất cao |
| Khu mỏ farm | Cao |
| NPC dẫn chuyện | Cao |
| Nền văn minh cấp 20 | Cao |
| Không shop trader | Bắt buộc |
| Loại bỏ cảm giác vanilla | Bắt buộc |

> **Định hướng cuối:** FurrMC Leo Tháp phải tạo cảm giác người chơi đang bước vào một RPG MMO độc lập bên trong Minecraft: boss có kỹ năng, loot có giá trị, thế giới có bí mật, và mỗi lần vượt tầng đều là một mốc tiến bộ rõ ràng.
