# 🧭 FurrMC Leo Tháp — UI, NPC Và Lệnh

> Toàn bộ giao diện cần làm người chơi quên cảm giác vanilla: HUD mới, menu rõ ràng, NPC dẫn chuyện, lệnh nhanh cho người đã quen.

---

## Mục Tiêu UI
| Mục Tiêu | Thiết Kế |
|---|---|
| Dễ tiếp cận | Người mới biết ngay nên đi đâu, đánh boss nào, thiếu gì. |
| RPG rõ ràng | Có HP/Mana/Stamina, chiến lực, phẩm chất, loot reveal. |
| Không rối | Menu ít chữ dài, ưu tiên icon, màu, trạng thái khóa/mở. |
| Hỗ trợ combat | Telegraph, boss phase, debuff, cooldown cần đọc nhanh. |
| Đồng bộ pack | UI texture, icon, font, âm thanh đều cùng phong cách. |

---

## HUD Combat
| Thành Phần | Nội Dung |
|---|---|
| HP | Máu hiện tại/tối đa, cảnh báo khi dưới 30%. |
| Mana/Energy | Tài nguyên dùng skill. |
| Stamina | Né, chạy, lướt. Không đủ stamina thì không spam né. |
| Boss Bar | Tên boss, HP, phase, trạng thái giáp/khiên. |
| Telegraph | Vòng đỏ, hình nón, đường thẳng, vùng nguy hiểm. |
| Debuff Tray | Độc, cháy, đóng băng, choáng, dấu ấn tử vong. |
| Quest Tracker | Mục tiêu hiện tại và nút gợi ý `/thap`. |

---

## Menu Chính
| Menu | Lệnh | Nội Dung |
|---|---|---|
| Tháp | `/thap` | 20 boss, trạng thái mở khóa, loot chính, độ khó. |
| Boss nhanh | `/boss <1-20>` | Vào nhanh boss đã mở. |
| Mỏ | `/mo` | Khu mỏ, tài nguyên, độ nguy hiểm, nhiệm vụ ngày. |
| Trang bị | `/trangbi` | Chỉ số, tiến hóa, reroll, set bonus. |
| Cốt truyện | `/truyen` | Mảnh ký ức, cinematic, nhiệm vụ chính. |
| Văn minh | `/vanminh` | Chọn/xem nền văn minh, danh vọng. |

---

## Menu `/thap`
| Slot/Phần | Thiết Kế |
|---|---|
| Boss đã mở | Icon sáng, hiển thị cấp, tên, loot chính. |
| Boss đang khuyến nghị | Có viền vàng, hiện “Nên đánh tiếp”. |
| Boss bị khóa | Icon tối, ghi điều kiện mở khóa. |
| Nút độ khó | Normal/Hard/Mythic nếu đủ điều kiện. |
| Nút lore | Xem mảnh truyện boss đã clear. |
| Nút party | Mời party hoặc vào hàng chờ. |

---

## NPC Chính
| NPC | Vị Trí | Vai Trò | Câu Nói Mẫu |
|---|---|---|---|
| Người Gác Tháp | Sảnh Tháp | Hướng dẫn tiến trình, mở `/thap` | “Muốn sống, hãy học cách nhìn trước khi chém.” |
| Ký Ức Sư | Thư viện ký ức | Xem lại lore/cinematic | “Không ký ức nào mất đi. Chỉ có người quên đọc nó.” |
| Thợ Rèn Dị Giới | Lò rèn | Tiến hóa/reroll trang bị | “Ta không bán sức mạnh. Ta chỉ rèn thứ ngươi tự giành được.” |
| Người Khai Mỏ | Cổng mỏ | Vào khu mỏ, nhiệm vụ farm | “Nếu boss không cho ngươi đồ, lòng đất sẽ cho ngươi cơ hội.” |
| Sứ Giả Văn Minh | Mở sau cấp 20 | Chọn văn minh | “Ngươi đã sống sót qua tận thế. Giờ hãy chọn di sản.” |

---

## Luồng NPC Dẫn Chuyện
| Mốc | NPC | Nội Dung |
|---|---|---|
| Spawn lần đầu | Người Gác Tháp | Giới thiệu boss, loot, không shop trader. |
| Clear boss 1 | Người Gác Tháp | Giải thích trang bị và mảnh boss. |
| Clear boss 5 | Thợ Rèn Dị Giới | Mở tiến hóa bậc II. |
| Clear boss 10 | Ký Ức Sư | Mở nhật ký cốt truyện sâu hơn. |
| Clear boss 15 | Người Gác Tháp | Cảnh báo nhóm boss huyền thoại. |
| Clear boss 20 | Sứ Giả Văn Minh | Chọn nền văn minh, mở endgame. |

---

## Loot Reveal
| Phẩm Chất | Hiệu Ứng |
|---|---|
| Common | Hiện nhanh, âm nhẹ. |
| Rare | Tia xanh, âm sáng. |
| Epic | Tia tím, popup lớn hơn. |
| Legendary | Dừng 1 giây, âm vang, thông báo party. |
| Mythic | Animation mở hộp, hiệu ứng đỏ. |
| Relic | Cinematic ngắn, thông báo server nếu bật. |

---

## Cảnh Báo Combat
| Loại Đòn | Cảnh Báo |
|---|---|
| AoE vòng tròn | Vòng đỏ dưới đất, đầy dần trước khi nổ. |
| Cone | Hình quạt trước mặt boss. |
| Line | Đường sáng dài, có âm “charge”. |
| Grab | Dây/xúc tu nhắm vào người chơi, có 1 giây né. |
| Execute | Màn hình tối viền đỏ, HUD hiện “Nguy hiểm”. |

---

## Lệnh Admin Gợi Ý
| Lệnh | Chức Năng |
|---|---|
| `/thapadmin unlock <player> <level>` | Mở khóa boss cho người chơi. |
| `/thapadmin reset <player>` | Reset progression khi test. |
| `/thapadmin givefragment <player> <boss> <amount>` | Cho mảnh boss. |
| `/thapadmin reload` | Reload config/menu. |
| `/thapadmin debugboss <id>` | Spawn/test boss trong arena dev. |

---

## Chống Rối Cho Người Mới
| Vấn Đề | Giải Pháp |
|---|---|
| Quá nhiều menu | Lần đầu chỉ hiện `/thap`, `/trangbi`, `/mo`. |
| Không biết đi đâu | Quest Tracker luôn hiện boss khuyến nghị. |
| Không hiểu vì sao chết | Death recap: skill nào giết, cách né. |
| Không biết nâng đồ | Sau boss 5 bắt buộc tutorial rèn ngắn. |
| Không biết chọn văn minh | Có preview video/text ngắn và đổi miễn phí 24 giờ. |
