?# 📖 Hệ Thống Class — Skyblock Tu Tiên

> **Chọn Class tại Cảnh Giới 2 (Luyện Khí)** qua NPC hoặc lệnh `/class`
> Mỗi người chơi chọn **1 trong 5 Class**. Có thể chuyển class tại CG 9 và CG 13.

---

## Tổng Quan 5 Class

| # | Class | Vai Trò | Vũ Khí Chính | Stat Chính | Màu |
|---|-------|---------|-------------|-----------|-----|
| Lv 1     | ⚔️ **Kiếm Tu** | Melee DPS | Kiếm, Đao | ATK, Crit | &c Đỏ |
| Lv 30    | 🔮 **Pháp Tu** | Magic DPS / CC | Pháp Bảo, Staff | Skill DMG, SPD | &5 Tím |
| Lv 60    | 🛡️ **Thể Tu** | Tank / Brawler | Quyền, Thương | DEF, HP | &6 Vàng |
| Lv 100   | 💚 **Y Tu** | Support / Healer | Phù, Trượng | Heal, Buff | &a Xanh lá |
| 5 | 🗡️ **Ám Tu** | Assassin / Burst | Đoản Đao, Ám Khí | Crit, SPD | &8 Xám |

---

## ⚔️ CLASS 1: KIẾM TU (Sword Cultivator)

> *"Một kiếm phá vạn pháp"*

### Mô Tả
Kiếm Tu là con đường tu luyện tập trung vào **kiếm thuật**, sử dụng kiếm khí để tấn công với sát thương bùng nổ. Kiếm Tu giỏi trong combat 1v1, combo nhanh, và burst damage cao. Là class được yêu thích nhất cho PVP và speed-clear dungeon.

### Base Stats (Lv1 → Lv100)

| Stat | Base | Growth/Level | Max (Lv100) |
|------|------|-------------|-------------|
| HP | 100 | +8/lv | 900 |
| ATK | 15 | +3/lv | 315 |
| DEF | 8 | +1.5/lv | 158 |
| SPD | 10 | +1/lv | 110 |
| Crit Rate | 5% | +0.3%/lv | 35% |
| Crit DMG | 150% | +1%/lv | 250% |

### Class Passive

| Passive | Hiệu Ứng | Scale |
|---------|-----------|-------|
| **Kiếm Ý** | Mỗi đòn đánh liên tiếp +5% DMG (max stack 5) | Stack reset sau 3s không đánh |
| **Kiếm Hồn** | Khi HP < 30%, ATK +25%, Crit Rate +15% | Cố định |
| **Phá Giáp** | Đòn đánh thường giảm 5% DEF target, stack 3 lần | 15s duration |

### 5 Skills Chi Tiết

#### Skill 1: Phong Kiếm Trảm — *Unlock: CG 2*

```
Loại: Active — Single Target
Mô tả: Phóng 3 đòn kiếm liên tiếp vào mục tiêu phía trước
DMG: Base 150 (+4.5/level) [Max Lv: 100]
Hiệu ứng: Mỗi đòn cộng dồn +10% DMG
Range: 3 blocks
CD: 5s | Mana: 20
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 150 | — | Mặc định |
| Lv 30    | 250 | +10% Crit | 500 LT |
| Lv 60    | 400 | +20% Crit | 2,000 LT |
| Lv 100   | 600 | +30% Crit, xuyên 1 target | 10,000 LT |

---

#### Skill 2: Kiếm Khí Phóng — *Unlock: CG 3*

```
Loại: Active — Ranged
Mô tả: Phóng kiếm khí theo đường thẳng, xuyên qua mọi mob trên đường bay
DMG: Base 300 (+8.1/level) [Max Lv: 100]
Hiệu ứng: Xuyên mob, giảm 10% DEF target 5s
Range: 15 blocks
CD: 8s | Mana: 35
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 300 | Xuyên mob | Mặc định |
| Lv 30    | 500 | +Slow 20% 3s | 1,500 LT |
| Lv 60    | 750 | +Bleed 50 DMG/s 3s | 5,000 LT |
| Lv 100   | 1,100 | AoE nổ cuối đường bay | 20,000 LT |

---

#### Skill 3: Vạn Kiếm Quy Tông — *Unlock: CG 5*

```
Loại: Active — AoE
Mô tả: Triệu hồi hàng trăm kiếm ảo bay xuống khu vực xung quanh
DMG: Base 800 (+17.2/level) [Max Lv: 100]
Hiệu ứng: AoE 5 block, xuyên giáp 30%
Range: 5 blocks radius
CD: 15s | Mana: 60
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 800 | Xuyên giáp 30% | Mặc định |
| Lv 30    | 1,200 | Radius +1 block | 3,000 LT |
| Lv 60    | 1,800 | +Knockback | 12,000 LT |
| Lv 100   | 2,500 | Xuyên giáp 50%, slow 30% | 50,000 LT |

---

#### Skill 4: Kiếm Khí Tung Hoành — *Unlock: CG 8*

```
Loại: Active — Cone AoE
Mô tả: Phóng kiếm khí hình quạt phía trước, crit rate tăng mạnh
DMG: Base 2,000 (+40.4/level) [Max Lv: 100]
Hiệu ứng: Cone 60°, 8 blocks, +50% Crit Rate 5s sau khi dùng
CD: 30s | Mana: 100
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 2,000 | +50% Crit Rate 5s | Mặc định |
| Lv 30    | 3,000 | +Crit DMG +30% | 15,000 LT |
| Lv 60    | 4,500 | Cone mở rộng 90° | 60,000 LT |
| Lv 100   | 6,000 | +80% Crit Rate, reset CD skill 1 | 200,000 LT |

---

#### Skill 5 (Ultimate): Nhất Kiếm Phá Thiên — *Unlock: CG 10*

```
Loại: Ultimate — Single Target
Mô tả: Tập trung toàn bộ kiếm khí vào 1 đòn chém duy nhất, bỏ qua mọi phòng thủ
DMG: Base 10,000 (+252.5/level) [Max Lv: 100]
Hiệu ứng: Ignore DEF, ignore Shield, không thể dodge
CD: 120s | Mana: 200
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 10,000 | Ignore DEF | Mặc định |
| Lv 30    | 15,000 | +Execute: x2 DMG nếu target < 20% HP | 50,000 LT |
| Lv 60    | 22,000 | +Hồi 30% HP nếu giết target | 200,000 LT |
| Lv 100   | 35,000 | +3s bất tử sau khi dùng | 1,000,000 LT |

---

## 🔮 CLASS 2: PHÁP TU (Spell Cultivator)

> *"Ngũ hành tương sinh, vạn pháp quy nguyên"*

### Mô Tả
Pháp Tu tu luyện theo con đường **pháp thuật**, sử dụng ngũ hành (Kim, Mộc, Thủy, Hỏa, Thổ) để tấn công diện rộng và khống chế kẻ địch. Là class mạnh nhất trong clear mob AoE và crowd control, nhưng yếu trong 1v1.

### Base Stats (Lv1 → Lv100)

| Stat | Base | Growth/Level | Max (Lv100) |
|------|------|-------------|-------------|
| HP | 80 | +6/lv | 680 |
| ATK | 10 | +2/lv | 210 |
| DEF | 6 | +1/lv | 106 |
| SPD | 12 | +1.2/lv | 132 |
| Skill DMG | 120% | +1.5%/lv | 270% |
| Mana | 150 | +5/lv | 650 |

### Class Passive

| Passive | Hiệu Ứng | Scale |
|---------|-----------|-------|
| **Ngũ Hành Luân Chuyển** | Mỗi skill dùng thay đổi nguyên tố → skill tiếp theo +15% DMG | Vòng lặp 5 nguyên tố |
| **Pháp Lực Hồi Phục** | Hồi 3% Mana/s khi không dùng skill 5s | Cố định |
| **Nguyên Tố Cộng Hưởng** | Đánh trúng 3 skill khác nhau liên tiếp → AoE burst thêm 500 DMG | 8s window |

### 5 Skills Chi Tiết

#### Skill 1: Hỏa Cầu Thuật — *Unlock: CG 2*

```
Loại: Active — AoE (Hỏa)
Mô tả: Phóng quả cầu lửa gây nổ AoE khi chạm mục tiêu
DMG: Base 120 (+4.3/level) [Max Lv: 100]
Hiệu ứng: AoE 3 block, gây Burn 20 DMG/s 3s
Range: 12 blocks
CD: 6s | Mana: 25
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 120 | Burn 3s | Mặc định |
| Lv 30    | 200 | AoE +1 block | 500 LT |
| Lv 60    | 350 | Burn 5s, +40 DMG/s | 2,000 LT |
| Lv 100   | 550 | Nổ 2 lần (aftershock) | 10,000 LT |

---

#### Skill 2: Băng Phong Bão — *Unlock: CG 3*

```
Loại: Active — AoE CC (Thủy/Băng)
Mô tả: Tạo bão băng xung quanh, gây DMG và đóng băng kẻ địch
DMG: Base 400 (+10.1/level) [Max Lv: 100]
Hiệu ứng: AoE 4 block, Freeze 2s, Slow 40% 5s
Range: Self-centered
CD: 12s | Mana: 45
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 400 | Freeze 2s | Mặc định |
| Lv 30    | 650 | Slow +50%, 6s | 1,500 LT |
| Lv 60    | 950 | Freeze 3s, AoE +1 | 5,000 LT |
| Lv 100   | 1,400 | Frozen target nhận +30% DMG | 20,000 LT |

---

#### Skill 3: Lôi Đình Vạn Quân — *Unlock: CG 5*

```
Loại: Active — AoE Burst (Lôi/Kim)
Mô tả: Triệu hồi sét từ trời đánh xuống khu vực rộng
DMG: Base 1,200 (+28.3/level) [Max Lv: 100]
Hiệu ứng: AoE 6 block, Stun 3s, chain lightning lây sang 3 mob gần
Range: 15 blocks (targeted)
CD: 20s | Mana: 80
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 1,200 | Stun 3s | Mặc định |
| Lv 30    | 1,800 | Chain +5 mob | 3,000 LT |
| Lv 60    | 2,700 | Stun 4s, AoE +2 | 12,000 LT |
| Lv 100   | 4,000 | Đánh sét 3 lần liên tiếp | 50,000 LT |

---

#### Skill 4: Ngũ Hành Luân Chuyển — *Unlock: CG 8*

```
Loại: Active — AoE + Debuff
Mô tả: Giải phóng 5 nguyên tố cùng lúc, gây DMG + random debuff mạnh
DMG: Base 1,800 (+37.4/level) [Max Lv: 100]
Hiệu ứng: AoE 5 block, random 1 trong 5 debuff:
  - Hỏa: Burn 100 DMG/s 5s
  - Thủy: Freeze 3s
  - Lôi: Stun 2.5s
  - Mộc: Heal bản thân 500 HP
  - Thổ: Target -30% DEF 8s
CD: 25s | Mana: 120
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 1,800 | 1 random debuff | Mặc định |
| Lv 30    | 2,800 | 2 random debuff | 15,000 LT |
| Lv 60    | 4,000 | 3 random debuff | 60,000 LT |
| Lv 100   | 5,500 | Tất cả 5 debuff cùng lúc | 200,000 LT |

---

#### Skill 5 (Ultimate): Thiên Địa Pháp Tướng — *Unlock: CG 10*

```
Loại: Ultimate — Transformation
Mô tả: Biến thành Pháp Tướng khổng lồ 15s, toàn bộ skill được buff cực mạnh
DMG: Không gây DMG trực tiếp
Hiệu ứng:
  - +200% Skill DMG
  - AoE mọi skill x2
  - CD tất cả skill giảm 50%
  - Immune to CC
  - Size x3 (visual)
Duration: 15s
CD: 150s | Mana: 250
```

| Mốc Level | Duration | Bonus | Upgrade Cost |
|----------|----------|-------|-------------|
| Lv 1     | 15s | +200% Skill DMG | Mặc định |
| Lv 30    | 18s | +250% Skill DMG | 50,000 LT |
| Lv 60    | 22s | +300% Skill DMG, hồi Mana 50/s | 200,000 LT |
| Lv 100   | 25s | +400% Skill DMG, team cũng được +50% | 1,000,000 LT |

---

## 🛡️ CLASS 3: THỂ TU (Body Cultivator)

> *"Lấy thân thể làm khí mãnh, toàn thân đều là vũ khí"*

### Mô Tả
Thể Tu tu luyện **thể xác**, biến cơ thể thành vũ khí và lá chắn. Tank tốt nhất, có thể chịu đòn cho đồng đội, taunt mob, và phản dame. Không gây nhiều sát thương nhưng cực kỳ khó chết.

### Base Stats (Lv1 → Lv100)

| Stat | Base | Growth/Level | Max (Lv100) |
|------|------|-------------|-------------|
| HP | 150 | +12/lv | 1,350 |
| ATK | 10 | +1.5/lv | 160 |
| DEF | 15 | +3/lv | 315 |
| SPD | 8 | +0.5/lv | 58 |
| Block Rate | 5% | +0.3%/lv | 35% |
| DMG Reduction | 0% | +0.2%/lv | 20% |

### Class Passive

| Passive | Hiệu Ứng | Scale |
|---------|-----------|-------|
| **Đồng Bì Thiết Cốt** | Giảm 10% DMG nhận vĩnh viễn | Cố định |
| **Nộ Khí** | Mỗi lần nhận DMG, +2% ATK (max stack 10) | Reset khi hết combat 5s |
| **Hộ Thể** | Tự động chặn 1 đòn chí mạng mỗi 60s, giữ 1 HP | 60s internal CD |

### 5 Skills Chi Tiết

#### Skill 1: Thạch Bì Thuật — *Unlock: CG 2*

```
Loại: Active — Self Buff
Mô tả: Hóa đá bề mặt da, tăng phòng thủ lớn
DMG: 0
Hiệu ứng: +50% DEF 8s, giảm DMG nhận 20%
CD: 10s | Mana: 20
```

| Mốc Level | DEF Bonus | Duration | Upgrade Cost |
|----------|-----------|----------|-------------|
| Lv 1     | +50% DEF | 8s | Mặc định |
| Lv 30    | +70% DEF | 10s | 500 LT |
| Lv 60    | +90% DEF, +30% DMG Reduction | 12s | 2,000 LT |
| Lv 100   | +120% DEF, reflect 10% DMG | 15s | 10,000 LT |

---

#### Skill 2: Bá Vương Quyền — *Unlock: CG 3*

```
Loại: Active — Melee AoE + CC
Mô tả: Đấm mạnh xuống đất, gây knockback và taunt kẻ địch
DMG: Base 400 (+11.1/level) [Max Lv: 100]
Hiệu ứng: AoE 3 block, Knockback 5 block, Taunt 3s
Range: Self-centered
CD: 12s | Mana: 40
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 400 | Taunt 3s | Mặc định |
| Lv 30    | 650 | Taunt 4s, +stun 1s | 1,500 LT |
| Lv 60    | 1,000 | AoE +2, slow 30% | 5,000 LT |
| Lv 100   | 1,500 | Taunt 5s, hồi 10% MaxHP | 20,000 LT |

---

#### Skill 3: Thiết Bích — *Unlock: CG 5*

```
Loại: Active — Shield + Reflect
Mô tả: Tạo khiên năng lượng hấp thụ sát thương và phản lại
DMG: 0 (phản 20% DMG nhận)
Hiệu ứng: Shield 500/800/1,200/2,000 HP, phản 20% DMG 6s
CD: 18s | Mana: 60
```

| Mốc Level | Shield | Reflect | Upgrade Cost |
|----------|--------|---------|-------------|
| Lv 1     | 500 HP | 20% | Mặc định |
| Lv 30    | 800 HP | 25% | 3,000 LT |
| Lv 60    | 1,200 HP | 30%, chặn CC | 12,000 LT |
| Lv 100   | 2,000 HP | 40%, heal từ DMG phản | 50,000 LT |

---

#### Skill 4: Bất Động Minh Vương — *Unlock: CG 8*

```
Loại: Active — Mega Tank + Taunt
Mô tả: Biến thành tượng Minh Vương, không thể di chuyển nhưng cực kỳ tank
DMG: 0
Hiệu ứng: +100% DEF, phản 40% DMG, AoE Taunt 8 block, 6s duration
Hạn chế: Không thể di chuyển trong thời gian cast
CD: 25s | Mana: 100
```

| Mốc Level | DEF Bonus | Reflect | Upgrade Cost |
|----------|-----------|---------|-------------|
| Lv 1     | +100% | 40% | Mặc định |
| Lv 30    | +130% | 45%, hồi 5% HP/s | 15,000 LT |
| Lv 60    | +160% | 50%, Taunt 10 block | 60,000 LT |
| Lv 100   | +200% | 60%, có thể di chuyển chậm | 200,000 LT |

---

#### Skill 5 (Ultimate): Kim Cang Bất Hoại — *Unlock: CG 10*

```
Loại: Ultimate — Invulnerability
Mô tả: Thân thể biến thành Kim Cang bất hoại, hoàn toàn bất tử
DMG: 0
Hiệu ứng:
  - Bất tử 8s (không thể chết)
  - Phản 50% DMG nhận
  - AoE Taunt toàn bộ mob trong 15 block
  - Heal 2% MaxHP/s
CD: 180s | Mana: 200
```

| Mốc Level | Duration | Bonus | Upgrade Cost |
|----------|----------|-------|-------------|
| Lv 1     | 8s | Bất tử + 50% reflect | Mặc định |
| Lv 30    | 10s | +60% reflect, heal 3%/s | 50,000 LT |
| Lv 60    | 12s | +70% reflect, team +20% DEF | 200,000 LT |
| Lv 100   | 15s | +80% reflect, nổ AoE 5,000 DMG khi hết | 1,000,000 LT |

---

## 💚 CLASS 4: Y TU (Healer Cultivator)

> *"Cứu nhân tế thế, Linh Dược diệu thủ"*

### Mô Tả
Y Tu tu luyện theo con đường **y thuật**, sử dụng linh dược và linh khí để chữa thương, buff đồng đội, và cleanse debuff. Là class không thể thiếu trong party dungeon, đặc biệt dungeon cấp cao.

### Base Stats (Lv1 → Lv100)

| Stat | Base | Growth/Level | Max (Lv100) |
|------|------|-------------|-------------|
| HP | 90 | +7/lv | 790 |
| ATK | 8 | +1/lv | 108 |
| DEF | 10 | +2/lv | 210 |
| SPD | 11 | +1/lv | 111 |
| Heal Power | 100% | +1.5%/lv | 250% |
| Mana | 200 | +6/lv | 800 |

### Class Passive

| Passive | Hiệu Ứng | Scale |
|---------|-----------|-------|
| **Linh Y Diệu Thủ** | Heal hiệu quả +20% cho ally HP < 30% | Cố định |
| **Tự Hồi** | Hồi 2% MaxHP/s khi không chiến đấu 3s | Cố định |
| **Linh Khí Lan Tỏa** | Ally trong 5 block +5% HP regen | Aura |

### 5 Skills Chi Tiết

#### Skill 1: Linh Dược Thuật — *Unlock: CG 2*

```
Loại: Active — Single Target Heal
Mô tả: Chữa lành mục tiêu bằng linh dược
Heal: Base 200 (+6.1/level) [Max Lv: 100]
Range: 10 blocks
CD: 6s | Mana: 25
```

| Mốc Level | Heal | Bonus | Upgrade Cost |
|----------|------|-------|-------------|
| Lv 1     | 200 HP | — | Mặc định |
| Lv 30    | 350 HP | +Cleanse 1 debuff | 500 LT |
| Lv 60    | 550 HP | +HoT 30 HP/s 5s | 2,000 LT |
| Lv 100   | 800 HP | +Shield 200HP 5s | 10,000 LT |

---

#### Skill 2: Sinh Cơ Quyết — *Unlock: CG 3*

```
Loại: Active — Party Heal over Time
Mô tả: Tạo vùng hồi máu cho toàn party
Heal: Base 50 (+1/level) [Max Lv: 100]
Duration: 10s
Range: 8 block radius
CD: 15s | Mana: 50
```

| Mốc Level | HoT | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 50 HP/s | Party AoE | Mặc định |
| Lv 30    | 70 HP/s | +5% ATK buff | 1,500 LT |
| Lv 60    | 100 HP/s | +10% ATK buff, radius +2 | 5,000 LT |
| Lv 100   | 150 HP/s | +15% ATK + DEF buff | 20,000 LT |

---

#### Skill 3: Linh Khí Hộ Thể — *Unlock: CG 5*

```
Loại: Active — Party Shield + Buff
Mô tả: Bọc toàn party trong lớp Linh Khí bảo vệ
Shield: Base 400 (+11.1/level) [Max Lv: 100]
Buff: +15% ATK toàn party 8s
Range: 10 block radius
CD: 18s | Mana: 70
```

| Mốc Level | Shield | ATK Buff | Upgrade Cost |
|----------|--------|----------|-------------|
| Lv 1     | 400 HP | +15% ATK | Mặc định |
| Lv 30    | 600 HP | +20% ATK | 3,000 LT |
| Lv 60    | 900 HP | +25% ATK + SPD | 12,000 LT |
| Lv 100   | 1,500 HP | +30% ATK + SPD + Crit | 50,000 LT |

---

#### Skill 4: Tịnh Hóa — *Unlock: CG 8*

```
Loại: Active — Cleanse + Shield
Mô tả: Thanh tẩy mọi debuff và tạo shield mạnh cho party
Shield: Base 800 (+22.2/level) [Max Lv: 100]
Hiệu ứng: Cleanse ALL debuff toàn party + Shield
Range: 12 block radius
CD: 20s | Mana: 100
```

| Mốc Level | Shield | Bonus | Upgrade Cost |
|----------|--------|-------|-------------|
| Lv 1     | 800 HP | Cleanse all | Mặc định |
| Lv 30    | 1,200 HP | +Immune debuff 3s | 15,000 LT |
| Lv 60    | 1,800 HP | +Immune 5s, heal 300 | 60,000 LT |
| Lv 100   | 3,000 HP | +Immune 8s, reflect debuff | 200,000 LT |

---

#### Skill 5 (Ultimate): Luân Hồi Mộc — *Unlock: CG 10*

```
Loại: Ultimate — Mass Resurrect + Full Heal
Mô tả: Sức mạnh của luân hồi - hồi sinh mọi đồng đội đã chết và full heal
Heal: Full HP toàn party
Hiệu ứng:
  - Rez tất cả ally đã chết (trong 15 block)
  - Full heal toàn party
  - Immune to DMG 3s sau khi hồi sinh
CD: 240s | Mana: 300
```

| Mốc Level | Bonus | Upgrade Cost |
|----------|-------|-------------|
| Lv 1     | Rez + Full heal | Mặc định |
| Lv 30    | +Immune 5s, rez với 100% HP | 50,000 LT |
| Lv 60    | +Buff rez'd ally: +30% ATK 15s | 200,000 LT |
| Lv 100   | +Hồi sinh không giới hạn range, party +50% stat 10s | 1,000,000 LT |

---

## 🗡️ CLASS 5: ÁM TU (Shadow Cultivator)

> *"Ẩn trong bóng tối, một击 tất sát"*

### Mô Tả
Ám Tu tu luyện **ám thuật**, sống trong bóng tối và tấn công bất ngờ. Class có burst damage cao nhất trong game, có thể tàng hình và one-shot target. Yếu điểm là máu thấp, dễ chết nếu bị phát hiện.

### Base Stats (Lv1 → Lv100)

| Stat | Base | Growth/Level | Max (Lv100) |
|------|------|-------------|-------------|
| HP | 70 | +5/lv | 570 |
| ATK | 12 | +2.5/lv | 262 |
| DEF | 5 | +0.8/lv | 85 |
| SPD | 15 | +1.5/lv | 165 |
| Crit Rate | 8% | +0.5%/lv | 58% |
| Crit DMG | 200% | +2%/lv | 400% |

### Class Passive

| Passive | Hiệu Ứng | Scale |
|---------|-----------|-------|
| **Ám Ảnh** | Đòn đánh từ tàng hình luôn crit + x2 DMG | Cố định |
| **Thoát Thân** | Khi HP < 20%, tự động tàng hình 3s (CD 120s) | Internal CD |
| **Chí Mạng** | Crit DMG +5% mỗi khi giết 1 mob (max +50%, reset khi chết) | Stack trong 1 life |

### 5 Skills Chi Tiết

#### Skill 1: Ám Ảnh Bộ — *Unlock: CG 2*

```
Loại: Active — Self Buff (Stealth)
Mô tả: Biến mất vào bóng tối, đòn đánh tiếp theo gây DMG khủng
DMG: 0 (buff đòn tiếp theo +100/150/200/300% DMG)
Hiệu ứng: Tàng hình 5s, đòn đánh tiếp +DMG, crit guaranteed
CD: 10s | Mana: 20
```

| Mốc Level | Stealth | DMG Bonus | Upgrade Cost |
|----------|---------|-----------|-------------|
| Lv 1     | 5s | +100% DMG | Mặc định |
| Lv 30    | 6s | +150% DMG, +SPD 30% | 500 LT |
| Lv 60    | 7s | +200% DMG, xuyên giáp 20% | 2,000 LT |
| Lv 100   | 8s | +300% DMG, stun target 1.5s | 10,000 LT |

---

#### Skill 2: Độc Nhẫn — *Unlock: CG 3*

```
Loại: Active — Single Target + DoT
Mô tả: Phi ám khí tẩm độc vào mục tiêu
DMG: Base 250 (+6.6/level) [Max Lv: 100]
Hiệu ứng: Poison 50/80/120/200 DMG/s trong 5s
Range: 10 blocks
CD: 8s | Mana: 30
```

| Mốc Level | Instant DMG | Poison/s | Upgrade Cost |
|----------|-------------|----------|-------------|
| Lv 1     | 250 | 50 | Mặc định |
| Lv 30    | 400 | 80, -10% heal received | 1,500 LT |
| Lv 60    | 600 | 120, -20% heal, slow 20% | 5,000 LT |
| Lv 100   | 900 | 200, -30% heal, slow 40% | 20,000 LT |

---

#### Skill 3: Ám Sát — *Unlock: CG 5*

```
Loại: Active — Teleport + Burst
Mô tả: Dịch chuyển tức thì ra sau lưng target và đâm chí mạng
DMG: Base 1,500 (+35.4/level) [Max Lv: 100]
Hiệu ứng: Teleport sau lưng target, DMG x2 nếu đang tàng hình
Range: 15 blocks
CD: 15s | Mana: 60
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 1,500 | x2 từ stealth | Mặc định |
| Lv 30    | 2,200 | +Bleed 100/s 5s | 3,000 LT |
| Lv 60    | 3,500 | +Reset Ám Ảnh Bộ CD | 12,000 LT |
| Lv 100   | 5,000 | x3 từ stealth, reset nếu target chết | 50,000 LT |

---

#### Skill 4: Vạn Ám Thiên La — *Unlock: CG 8*

```
Loại: Active — AoE + Debuff
Mô tả: Phóng mạng lưới ám khí bao phủ khu vực
DMG: Base 2,000 (+45.5/level) [Max Lv: 100]
Hiệu ứng: AoE 6 block, Blind 3s + Slow 50%
Range: 12 blocks
CD: 25s | Mana: 100
```

| Mốc Level | DMG | Bonus | Upgrade Cost |
|----------|-----|-------|-------------|
| Lv 1     | 2,000 | Blind 3s + Slow 50% | Mặc định |
| Lv 30    | 3,200 | Blind 4s, -20% DEF | 15,000 LT |
| Lv 60    | 4,500 | Blind 5s, -30% DEF, AoE +2 | 60,000 LT |
| Lv 100   | 6,500 | Blind 6s, -40% DEF, trap kéo mob lại trung tâm | 200,000 LT |

---

#### Skill 5 (Ultimate): Tử Thần Giáng Lâm — *Unlock: CG 10*

```
Loại: Ultimate — Single Target Execute
Mô tả: Mark mục tiêu bằng dấu Tử Thần, mọi đòn đánh đều crit, kết thúc bằng DMG khủng
Hiệu ứng:
  - Mark 1 target trong 10s
  - Mọi đòn đánh vào target đều CRIT (100% Crit Rate)
  - Kết thúc mark: gây bonus 8,000 DMG burst
  - Nếu target chết trong thời gian mark: reset CD 50%
CD: 150s | Mana: 200
```

| Mốc Level | Mark Duration | Final Burst | Upgrade Cost |
|----------|--------------|-------------|-------------|
| Lv 1     | 10s | 8,000 DMG | Mặc định |
| Lv 30    | 12s | 12,000 DMG, +tàng hình 3s sau kill | 50,000 LT |
| Lv 60    | 15s | 18,000 DMG, mark lây sang target gần nếu kill | 200,000 LT |
| Lv 100   | 18s | 30,000 DMG, mark 2 target cùng lúc | 1,000,000 LT |

---

## Quy Tắc Chung

### Chọn & Chuyển Class

| Quy Tắc | Chi Tiết |
|----------|---------|
| **Chọn Class** | Tại Cảnh Giới 2 (Luyện Khí), qua NPC hoặc `/class` |
| **Chuyển Class** | Tại CG 9 (Độ Kiếp) và CG 13 (Thái Ất), tốn 500 Linh Ngọc |
| **Reset Skill** | 200 Linh Ngọc mỗi lần reset skill level |
| **Skill Point** | Nhận 1 Skill Point mỗi 10 level, dùng để lên skill |

### Party Bonus (Ngũ Hành)

| Số Class Khác Nhau | Bonus |
|--------------------|-------|
| 2 class | +5% toàn stat |
| 3 class | +10% toàn stat |
| 4 class | +15% toàn stat |
| **5 class (đủ Ngũ Hành)** | **+20% toàn stat + 10% Drop Rate** |

### Tương Khắc (PVP)

```
⚔️ Kiếm Tu ──▶ 💚 Y Tu ──▶ 🗡️ Ám Tu ──▶ 🔮 Pháp Tu ──▶ 🛡️ Thể Tu ──▶ ⚔️ Kiếm Tu
   (chém)        (trị)        (ám sát)       (pháp)         (đấm)        (chém)

Class KHẮC target: +15% DMG dealt, -10% DMG received
Class BỊ KHẮC: -15% DMG dealt, +10% DMG received
```

### Class Gear (Trang Bị Riêng)

| Class | Gear Exclusive | Bonus |
|-------|---------------|-------|
| ⚔️ Kiếm Tu | Kiếm Tiên, Đao Linh | +20% Crit DMG |
| 🔮 Pháp Tu | Pháp Bảo Tiên, Staff Cổ | +20% Skill DMG |
| 🛡️ Thể Tu | Giáp Huyền Thiết, Quyền Bao | +20% DEF |
| 💚 Y Tu | Trượng Linh, Phù Tiên | +20% Heal Power |
| 🗡️ Ám Tu | Đoản Đao Ám, Ám Khí Tiên | +20% Crit Rate |
