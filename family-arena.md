# 🏟️ FurrMC Leo Tháp — Đấu Trường Gia Tộc

> **Không phải PvP. Không tranh giành lãnh thổ.**  
> Đấu Trường Gia Tộc là hệ thống PvE cạnh tranh gián tiếp, nơi mỗi gia tộc phải duy trì điểm uy tín cao trên BXH bằng nhiệm vụ ngày, boss cột mốc và mức độ hoạt động ổn định của thành viên.

---

## 1. Tổng Quan

Đấu Trường Gia Tộc là chế độ dành cho nhóm người chơi đã có gia tộc. Mỗi gia tộc sở hữu một lượng **Điểm Duy Trì** gọi là **Uy Tín Gia Tộc**. Điểm này tăng khi thành viên hoàn thành nhiệm vụ, clear boss, đóng góp tài nguyên và tham gia hoạt động tuần. Điểm này giảm khi gia tộc bỏ bê nhiệm vụ ngày, thua boss ở round cột mốc, hoặc để nhiều thành viên không hoạt động.

Mục tiêu không phải đánh nhau với gia tộc khác, mà là giữ gia tộc sống, mạnh và có thứ hạng cao. BXH gia tộc trở thành áp lực cộng đồng: mỗi thành viên đều có trách nhiệm đóng góp, nhưng hệ thống cần chống việc một người phá cả gia tộc.

### Trụ Cột Thiết Kế

| Trụ Cột | Mô Tả |
|---|---|
| **PvE cạnh tranh gián tiếp** | Gia tộc đua điểm qua hoạt động PvE, không giết người, không chiếm đất. |
| **Duy trì thay vì bùng nổ** | Gia tộc mạnh là gia tộc hoạt động đều, không chỉ cày một ngày rồi bỏ. |
| **Trách nhiệm tập thể** | Thành viên không làm nhiệm vụ ngày sẽ ảnh hưởng điểm, nhưng có giới hạn để tránh phá hoại. |
| **Boss cột mốc** | Gia tộc phải vượt các round boss định kỳ để giữ hạng. |
| **Dễ hiểu** | Người chơi nhìn menu là biết hôm nay gia tộc thiếu gì, ai đã đóng góp, điểm đang tăng/giảm ra sao. |

---

## 2. Thuật Ngữ Chính

| Thuật Ngữ | Ý Nghĩa |
|---|---|
| **Uy Tín Gia Tộc** | Điểm chính dùng để xếp hạng gia tộc. |
| **Điểm Duy Trì Tối Thiểu** | Mốc điểm cần giữ để không bị tụt cấp gia tộc. |
| **Nhiệm Vụ Ngày Gia Tộc** | Nhiệm vụ cá nhân tính cho gia tộc, reset mỗi ngày. |
| **Round Cột Mốc** | Boss PvE định kỳ của gia tộc, thua sẽ bị trừ điểm. |
| **Đóng Góp Cá Nhân** | Điểm riêng của từng thành viên, dùng để chia thưởng và chống ăn bám. |
| **Mùa Gia Tộc** | Chu kỳ BXH, ví dụ 2 hoặc 4 tuần. |

---

## 3. Vòng Lặp Gameplay

```text
Thành viên nhận nhiệm vụ ngày
        ↓
Đánh boss / farm mỏ / đóng góp tài nguyên / hỗ trợ gia tộc
        ↓
Gia tộc tăng Uy Tín và tiến độ round cột mốc
        ↓
Đến mốc tuần, gia tộc vào boss round cột mốc
        ↓
Thắng: giữ/tăng hạng, mở thưởng
Thua: bị trừ điểm, cần phục hồi bằng nhiệm vụ và đóng góp
        ↓
Cuối mùa: BXH gia tộc phát thưởng theo hạng và đóng góp cá nhân
```

---

## 4. Uy Tín Gia Tộc

### Điểm Khởi Tạo
| Quy Mô Gia Tộc | Điểm Khởi Tạo | Điểm Duy Trì Tối Thiểu |
|---:|---:|---:|
| 3-5 thành viên | 1,000 | 700 |
| 6-10 thành viên | 2,000 | 1,400 |
| 11-20 thành viên | 4,000 | 2,800 |
| 21+ thành viên | 6,000 | 4,200 |

> [!NOTE]
> Điểm duy trì nên scale theo số thành viên hoạt động, không theo tổng thành viên tuyệt đối. Nếu không, gia tộc lớn nhưng nhiều acc phụ sẽ bị phạt quá nặng.

### Nguồn Cộng Điểm
| Hoạt Động | Điểm Gia Tộc | Giới Hạn |
|---|---:|---|
| Thành viên hoàn thành nhiệm vụ ngày | +20 mỗi người | Tính tối đa theo số thành viên hoạt động |
| Clear boss cá nhân đúng cấp khuyến nghị | +5 | Tối đa 5 lần/người/ngày |
| Clear boss gia tộc thường | +100 đến +300 | Theo độ khó |
| Clear round cột mốc | +500 đến +2,000 | Theo cấp round |
| Đóng góp tài nguyên mỏ | +1 mỗi gói tài nguyên | Có cap ngày |
| Hoàn thành nhiệm vụ tuần | +1,000 | 1 lần/tuần |
| Thành viên mới hoạt động đủ 3 ngày | +100 | Chống tạo acc rồi bỏ |

---

## 5. Cơ Chế Trừ Điểm

Cơ chế trừ điểm tạo áp lực duy trì, nhưng phải công bằng. Không nên để một thành viên troll làm sập cả gia tộc.

### Bảng Trừ Điểm
| Lý Do | Điểm Trừ | Giới Hạn / Chống Lạm Dụng |
|---|---:|---|
| Thành viên hoạt động không hoàn thành nhiệm vụ ngày | -10 mỗi người | Chỉ tính người online từ 15 phút trở lên trong ngày |
| Thành viên bỏ nhiệm vụ 3 ngày liên tiếp | -30 mỗi người | Chỉ tính nếu vẫn còn trong danh sách active |
| Thua boss round cột mốc | -300 đến -1,500 | Theo cấp round, không trừ quá 20% điểm hiện có |
| Bỏ cuộc giữa round cột mốc | -200 | Chỉ khi gia tộc tự rời, không tính crash/server lỗi |
| Không tham gia round tuần | -500 | Có 1 lần miễn trừ mỗi mùa |
| Điểm đóng góp tuần quá thấp | -5 mỗi thành viên dưới chuẩn | Cap tổng trừ để tránh phá gia tộc |
| Gia tộc không đủ hoạt động 3 ngày | -5% điểm hiện có | Chỉ áp dụng gia tộc trên 7 ngày tuổi |

### Quy Tắc Công Bằng
| Vấn Đề | Cách Xử Lý |
|---|---|
| Thành viên mới vào rồi không chơi | 72 giờ đầu là thời gian thử, không tính phạt nhiệm vụ ngày. |
| Thành viên xin nghỉ | Leader/officer có thể đặt trạng thái nghỉ tối đa 3 ngày/mùa. |
| Người chơi online ít | Chỉ bị tính nếu online đủ 15 phút trong ngày. |
| Gia tộc nhỏ | Điểm yêu cầu scale theo số thành viên active. |
| Troll cố ý fail boss | Boss cột mốc cần quyền đăng ký từ leader/officer, không phải ai cũng mở được. |

---

## 6. Nhiệm Vụ Ngày Gia Tộc

Mỗi thành viên nhận 3 nhiệm vụ ngày. Chỉ cần hoàn thành **2/3 nhiệm vụ** để được tính là hoàn thành ngày, giúp hệ thống dễ tiếp cận hơn.

### Nhóm Nhiệm Vụ
| Nhóm | Ví Dụ | Điểm Cá Nhân | Điểm Gia Tộc |
|---|---|---:|---:|
| Boss | Hạ 1 boss đúng cấp hoặc thấp hơn tối đa 3 cấp | +50 | +20 |
| Mỏ | Đào 100 tài nguyên ở mỏ đã mở khóa | +40 | +15 |
| Hỗ trợ | Đi boss cùng thành viên gia tộc yếu hơn | +60 | +25 |
| Trang bị | Tiến hóa/reroll 1 món trang bị | +30 | +10 |
| Khám phá | Tìm 1 rương ẩn hoặc mảnh ký ức | +40 | +15 |
| Đóng góp | Nộp gói tài nguyên gia tộc | +30 | +10 |

### Chuẩn Hoàn Thành Ngày
| Điều Kiện | Kết Quả |
|---|---|
| Hoàn thành 0/3 | Cá nhân không nhận thưởng, gia tộc có thể bị trừ nếu người đó active. |
| Hoàn thành 1/3 | Nhận ít thưởng cá nhân, chưa tính hoàn thành ngày. |
| Hoàn thành 2/3 | Tính hoàn thành ngày, gia tộc nhận điểm đầy đủ. |
| Hoàn thành 3/3 | Nhận bonus cá nhân, gia tộc thêm điểm phụ nhỏ. |

---

## 7. Boss Round Cột Mốc

Round cột mốc là thử thách PvE của gia tộc, diễn ra theo tuần hoặc khi gia tộc đạt mốc điểm nhất định. Đây là nguồn điểm lớn nhất nhưng cũng có rủi ro trừ điểm nếu thua.

### Mốc Round
| Round | Điều Kiện | Boss Chủ Đề | Thắng | Thua |
|---:|---|---|---:|---:|
| 1 | 2,000 Uy Tín | Hộ Vệ Gia Tộc | +500 | -300 |
| 2 | 5,000 Uy Tín | Tinh Thể Cộng Hưởng | +800 | -500 |
| 3 | 10,000 Uy Tín | Kỵ Sĩ Phán Xét | +1,200 | -800 |
| 4 | 18,000 Uy Tín | Long Ảnh Gia Tộc | +1,600 | -1,100 |
| 5 | 30,000 Uy Tín | Thẩm Phán Tận Thế | +2,000 | -1,500 |

### Luật Round
| Luật | Mô Tả |
|---|---|
| Số người | 3-8 thành viên, scale theo số người vào. |
| Quyền mở | Chỉ leader/officer mở được. |
| Thời gian | 10-20 phút tùy round. |
| Hồi sinh | Giới hạn số lần hồi sinh của toàn đội. |
| Thua | Hết thời gian, toàn đội chết, hoặc tự bỏ cuộc. |
| Thắng | Nhận Uy Tín, rương gia tộc, điểm cá nhân theo đóng góp. |

---

## 8. Bảng Xếp Hạng Gia Tộc

BXH không chỉ xếp theo tổng điểm. Cần nhiều chỉ số phụ để gia tộc không spam một hoạt động duy nhất.

### Chỉ Số BXH
| Chỉ Số | Vai Trò |
|---|---|
| Uy Tín Gia Tộc | Điểm xếp hạng chính. |
| Tỉ lệ hoàn thành nhiệm vụ ngày | Đo độ ổn định. |
| Round cột mốc cao nhất | Đo sức mạnh PvE. |
| Số thành viên active | Đo quy mô thật. |
| Điểm hỗ trợ nội bộ | Đo việc người mạnh giúp người yếu. |
| Điểm khám phá | Đo hoạt động ngoài boss. |

### Hạng Gia Tộc
| Hạng | Điều Kiện Gợi Ý | Quyền Lợi |
|---|---|---|
| Đồng | Đạt điểm duy trì tối thiểu | Rương tuần cơ bản |
| Bạc | Top 50% BXH | Bonus tài nguyên mỏ |
| Vàng | Top 25% BXH | Cosmetic banner gia tộc |
| Bạch Kim | Top 10% BXH | Aura sảnh gia tộc, title mùa |
| Huyền Thoại | Top 3 gia tộc | Hiệu ứng đặc biệt, tượng danh vọng |

---

## 9. Thưởng Gia Tộc

### Thưởng Tuần
| Điều Kiện | Thưởng |
|---|---|
| Đủ điểm duy trì | Rương Gia Tộc thường |
| Top 25% | Rương Gia Tộc hiếm |
| Clear round cột mốc | Mảnh trang bị gia tộc, nguyên liệu tiến hóa |
| Tỉ lệ nhiệm vụ ngày trên 80% | Bonus tài nguyên cho cả gia tộc |

### Thưởng Mùa
| Hạng | Thưởng |
|---|---|
| Top 50% | Title mùa, rương vật liệu |
| Top 25% | Banner gia tộc, cosmetic nhỏ |
| Top 10% | Aura gia tộc, hiệu ứng tên |
| Top 3 | Tượng gia tộc tại sảnh, Relic cosmetic |

### Chia Thưởng Công Bằng
| Điều Kiện Cá Nhân | Quyền Nhận Thưởng |
|---|---|
| Đóng góp dưới 10% chuẩn tuần | Không nhận thưởng mùa cao cấp. |
| Đóng góp 10-50% chuẩn tuần | Nhận 50% thưởng. |
| Đóng góp đủ chuẩn | Nhận 100% thưởng. |
| Top đóng góp gia tộc | Nhận thêm title/cosmetic nhỏ. |

---

## 10. Chống Phá Hoại Và Chống Ép Buộc

| Rủi Ro | Giải Pháp |
|---|---|
| Thành viên troll không làm nhiệm vụ | Chỉ phạt người active, có cap trừ điểm/ngày. |
| Leader ép member online quá nhiều | Chỉ cần 2/3 nhiệm vụ ngày, không yêu cầu cày dài. |
| Gia tộc kick người trước khi bị trừ điểm | Thành viên bị kick vẫn tính lịch sử ngày đó nếu đã active. |
| Gia tộc lớn dùng acc phụ | Chỉ tính active member có hoạt động thật. |
| Thua boss do lag/server lỗi | Round lỗi có thể hoàn trả bằng admin log. |
| Người mới bị gánh nặng | 72 giờ đầu không tính phạt. |

---

## 11. Menu Và Lệnh

### Lệnh Người Chơi
| Lệnh | Chức Năng |
|---|---|
| `/giatoc` | Mở menu gia tộc. |
| `/giatoc nhiemvu` | Xem nhiệm vụ ngày cá nhân. |
| `/giatoc bxh` | Xem BXH gia tộc. |
| `/giatoc donggop` | Xem đóng góp cá nhân và gia tộc. |
| `/giatoc round` | Xem round cột mốc hiện tại. |

### Lệnh Quản Lý
| Lệnh | Chức Năng |
|---|---|
| `/giatocadmin addpoint <family> <amount>` | Cộng điểm Uy Tín. |
| `/giatocadmin removepoint <family> <amount>` | Trừ điểm Uy Tín. |
| `/giatocadmin resetdaily <family>` | Reset nhiệm vụ ngày khi cần hỗ trợ. |
| `/giatocadmin startround <family> <round>` | Test/mở round cột mốc. |
| `/giatocadmin reload` | Reload config. |

---

## 12. UI Menu Gia Tộc
| Khu Vực Menu | Nội Dung |
|---|---|
| Tổng quan | Uy Tín hiện tại, hạng BXH, điểm cần duy trì. |
| Nhiệm vụ ngày | Ai đã hoàn thành, ai còn thiếu, thời gian reset. |
| Round cột mốc | Boss hiện tại, điều kiện mở, phần thưởng, rủi ro thua. |
| Đóng góp | Top đóng góp tuần, cảnh báo người dưới chuẩn. |
| Lịch sử điểm | Log cộng/trừ điểm gần nhất để minh bạch. |
| Thưởng | Rương tuần/mùa, điều kiện nhận. |

---

## 13. Tích Hợp Với Gameplay Leo Tháp
| Hệ Thống | Cách Tích Hợp |
|---|---|
| Boss 20 tầng | Nhiệm vụ gia tộc yêu cầu clear boss đúng cấp/khuyến nghị. |
| Khu mỏ | Đóng góp gói tài nguyên gia tộc. |
| Trang bị | Round cột mốc rơi nguyên liệu tiến hóa gia tộc. |
| Văn minh | Sau cấp 20, gia tộc có bonus nhỏ nếu nhiều nền văn minh phối hợp. |
| Endgame | Raid World Ender có mục tiêu phụ cho gia tộc. |

---

## 14. Ví Dụ Một Ngày Hoạt Động
| Thời Điểm | Hoạt Động | Tác Động Điểm |
|---|---|---:|
| Sáng | 6/10 thành viên hoàn thành 2/3 nhiệm vụ | +120 |
| Trưa | 3 người farm mỏ nộp gói tài nguyên | +45 |
| Tối | Gia tộc clear boss round 2 | +800 |
| Cuối ngày | 2 người active nhưng không làm nhiệm vụ | -20 |
| Tổng | Gia tộc hoạt động tốt | +945 |

---

## 15. Tiêu Chí Thành Công
| Tiêu Chí | Dấu Hiệu Đạt |
|---|---|
| Không biến thành PvP | Người chơi cạnh tranh bằng PvE, không cần đánh nhau. |
| Gia tộc có trách nhiệm | Member tự nhắc nhau làm nhiệm vụ ngày. |
| Không quá áp lực | Người bận vẫn chỉ cần 2/3 nhiệm vụ ngắn. |
| BXH có ý nghĩa | Gia tộc top cao là gia tộc đều, mạnh và phối hợp tốt. |
| Không bị phá hoại dễ | Một người troll không thể kéo sập cả gia tộc. |

---

## Ghi Chú Cân Bằng
| Hạng Mục | Khuyến Nghị |
|---|---|
| Mùa đầu | Nên chạy mùa 2 tuần để lấy dữ liệu. |
| Cap trừ điểm | Không quá 10-15% tổng Uy Tín/ngày. |
| Nhiệm vụ ngày | Hoàn thành trong 10-20 phút. |
| Round cột mốc | 10-20 phút, cần phối hợp nhưng không quá hardcore. |
| Thưởng | Ưu tiên cosmetic, danh hiệu, nguyên liệu; tránh pay-to-win hoặc snowball quá mạnh. |
