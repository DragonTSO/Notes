---
title: NPC va Khu Chuc Nang - MineRua Tu Tien
tags:
  - minerua
  - npc
  - tu-tien
  - gameplay-doc
aliases:
  - NPC Tu Tien
  - Khu NPC
---

# NPC va Khu Chuc Nang - MineRua Tu Tien

Tai lieu nay ghi lai NPC, hologram va cac khu chuc nang dang thay tu server `01e721c5`, doi chieu voi notes Tu Tien cu trong vault. Ban nay uu tien cach nhin theo gameplay: moi khu co `List NPC` ngan gon truoc, sau do moi tach ro muc do xac minh.

> [!note]
> Nguon chac chan: `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml`, `DeluxeMenus` va notes cu. Khu nao co gameplay ro nhung chua thay NPC entity rieng trong config se duoc ghi la `chuc nang suy ra tu gameplay`.

## Tong Quan Nhanh

| Khu | Hologram khu | Gameplay chinh | List NPC/chuc nang nhanh |
| :--- | :--- | :--- | :--- |
| K1 | `spawn_island` | Tien Dao, ve dao, nang cap dao | NPC Tien Dao |
| K2 | `spawn_luyenky` | Chon mon phai, lay vu khi, vao giai doan Luyen Khi | NPC Mon Phai, NPC Chon Vu Khi, NPC Luyen Khi |
| K3 | `spawn_tuluyen` | Tu luyen lay Tu Vi, De Tu, Nhap Than, xem thong tin | NPC Thong Tin, NPC Tu Luyen, NPC De Tu, NPC Nhap Than |
| K4 | `spawn_dungeon` | Bi Canh, danh quai, farm trang bi va Dot Pha Dan | NPC Bi Canh, NPC Bang Tang Dungeon |
| K5 | `spawn_dotpha_chuyensinh` | Dot Pha, vuot Thien Loi Kiep, Chuyen Sinh | NPC Dot Pha, NPC Chuyen Sinh, NPC Kiem Tra Dieu Kien |

## Khu 1 - Tien Dao

Khu 1 la noi nguoi choi bat dau vong lap Skyblock Tu Tien: mo Tien Dao, ve dao, nang cap may sinh quang va tich tai nguyen de nuoi tien trinh tu luyen.

```text
spawn_island: 1. TIEN DAO (ISLAND) [K1]
World: test
Toa do: x -1719.129, y 130.860, z -749.891
```

### List NPC

- NPC Tien Dao
- NPC Tien Dao Tutorial

### NPC Da Xac Minh

#### `TienDaoNPC2` - NPC Tien Dao

| Truong | Noi dung |
| :--- | :--- |
| ID config | `TienDaoNPC2` |
| Hologram lien quan | `TienDaoNPC2` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `test`, x `-1718.258`, y `83.0`, z `-792.506` |
| Action | Click chay `tiendao` bang `player_command` |
| Vai tro gameplay | Mo giao dien Tien Dao de nguoi choi quan ly dao va bat dau farm tai nguyen |

Lenh lien quan tu flow gameplay va huong dan:

| Lenh | Cong dung |
| :--- | :--- |
| `/tiendao` | Mo chuc nang Tien Dao |
| `/is panel` | Mo menu Island |
| `/is home` | Ve dao ca nhan |
| `/is visit <ten>` | Tham dao nguoi choi khac |
| `/is top` | Xem bang xep hang dao |
| `/gen` | Nang cap generator, Linh Mach va ore |

#### `TienDaoNPC` - NPC Tien Dao Tutorial

| Truong | Noi dung |
| :--- | :--- |
| ID config | `TienDaoNPC` |
| Hologram lien quan | `TienDaoNPC` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `tutorial`, x `146.469`, y `136.0`, z `-96.752` |
| Action | Click chay `tiendao` bang `player_command` |
| Vai tro gameplay | Ban tutorial cua NPC Tien Dao, dung de gioi thieu he dao truoc khi nguoi choi vao vong lap chinh |

## Khu 2 - Luyen Khi

Khu 2 dai dien cho buoc nguoi choi dinh hinh nhan vat: chon mon phai/class, lay vu khi dau tien va bat dau he Luyen Khi. Notes cu ghi khi dat Luyen Khi nguoi choi chon mot trong 5 huong: Kiem Tien, Thien Co, Kim Than, Linh Duoc, Vo Anh.

```text
spawn_luyenky: 2. LUYEN KHI [K2]
World: test
Toa do: x -1724.897, y 94.860, z -838.962
```

### List NPC

- NPC Mon Phai
- NPC Chon Mon Phai Tutorial
- NPC Chon Vu Khi
- NPC Luyen Khi

### NPC Da Xac Minh

#### `Spawn_Class` - NPC Mon Phai

| Truong | Noi dung |
| :--- | :--- |
| ID config | `Spawn_Class` |
| Hologram lien quan | `Spawn_Class` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `test`, x `-1719.171`, y `110.0`, z `-714.183` |
| Action | Click chay `monphai` bang `player_command` |
| Vai tro gameplay | Mo chon Mon Phai/Class, dinh huong loi choi va stat chinh |
| Ghi chu | Notes cu ghi chon class tai Canh Gioi 2 Luyen Khi |

#### `ChonMonPhai` - NPC Chon Mon Phai Tutorial

| Truong | Noi dung |
| :--- | :--- |
| ID config | `ChonMonPhai` |
| Hologram lien quan | `ChonMonPhai`, `Tutorial_1_MonPhai` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `tutorial`, x `-22.595`, y `68.0`, z `11.936` |
| Action | Click chay `monphai` bang `player_command` |
| Vai tro gameplay | Bat nguoi choi chon mon phai dau tien trong tutorial |

#### `ChonVuKhi` - NPC Chon Vu Khi

| Truong | Noi dung |
| :--- | :--- |
| ID config | `ChonVuKhi` |
| Hologram lien quan | `ChonVuKhi`, `Tutorial_2_VuKhi` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `tutorial`, x `-22.470`, y `68.0`, z `33.332` |
| Action | Click chay console command `chonvukhi {player}` |
| Vai tro gameplay | Phat vu khi dau tien theo mon phai da chon |

### Chuc Nang Suy Ra Tu Gameplay

#### NPC Luyen Khi

Khong thay NPC ID rieng cho `Luyen Khi`, nhung hologram tutorial mo ta ro buoc nay:

```text
Hay dung Linh Thach cua ban
de luyen khi, tich cuc luyen khi = trang bi
NGON!!!
```

Flow gameplay gan voi K2:

- Dat Canh Gioi 2 de mo chon class/mon phai.
- Lay vu khi khoi dau theo huong da chon.
- Bat dau xay build quanh trang bi, class va tang Tu Vi.

## Khu 3 - Tu Luyen

Khu 3 la vong lap lay Tu Vi va tang suc manh lau dai: `/tuluyen`, he De Tu, Nhap Than va thong tin ca nhan. Notes cu mo ta Tu Vi la kinh nghiem tu luyen chinh, dung de dat moc canh gioi va du dieu kien dot pha.

```text
spawn_tuluyen: 3. TU LUYEN [K3]
World: test
Toa do: x -1726.807, y 94.860, z -902.516
```

### List NPC

- NPC Thong Tin
- NPC Tu Luyen
- NPC De Tu
- NPC Nhap Than

### NPC Da Xac Minh

#### `Spawn_Infomation` - NPC Thong Tin

| Truong | Noi dung |
| :--- | :--- |
| ID config | `Spawn_Infomation` |
| Hologram lien quan | `Spawn_Information` |
| Nguon | `FancyNpcs/npcs.yml`, `FancyHolograms/holograms.yml` |
| World/toa do | `test`, x `-1713.181`, y `110.0`, z `-714.339` |
| Action | Click chay console command `dm open info_menu %player_name%` |
| Vai tro gameplay | Cho nguoi choi xem ho so tu si: rank, Linh Thach, Co Thach, mon phai, canh gioi, Tu Vi |

### Chuc Nang Suy Ra Tu Gameplay

#### NPC Tu Luyen

| Muc | Noi dung |
| :--- | :--- |
| Lenh gan voi gameplay | `/tuluyen` |
| Nguon | `huongdan_menu.yml`, `gameplay.md` |
| Vai tro gameplay | Tu tap de lay Tu Vi, day thanh tien trinh canh gioi va chuan bi cho dot pha |

#### NPC De Tu

| Muc | Noi dung |
| :--- | :--- |
| Lenh gan voi gameplay | `/pet`, alias `/dode` |
| Nguon | `huongdan_menu.yml`, `TurtlePet/command.yml`, `pet.md` |
| Vai tro gameplay | Quan ly he De Tu, xuat chien, thu hoi, dot pha De Tu va tang suc manh dong hanh |

Theo `pet.md`, he nay nen duoc goi player-facing la `De Tu`, khong chi la `Pet`.

#### NPC Nhap Than

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | Chua thay ID NPC config ro rang |
| Nguon | `huongdan_menu.yml`, `gameplay.md`, `rank.md` |
| Vai tro gameplay | Hy sinh hoac dung trang bi de tang chi so lau dai, day `Nhap_Than_Score` va `Thuc Luc` |

Flow gameplay chinh o K3:

- Cay Tu Vi qua `/tuluyen` va cac hoat dong song song.
- Nang he De Tu de bo sung sat thuong, ho tro va tien trinh lau dai.
- Nhap Than de day suc manh tong the truoc khi vao dungeon kho hon hoac dot pha.

## Khu 4 - Thi Luyen Dungeon

Khu 4 la khu Bi Canh/Thi Luyen de nguoi choi danh quai, boss, farm trang bi hiem va nguyen lieu nhu Dot Pha Dan. Notes cu mo ta dungeon mo dan theo canh gioi va thuc luc.

```text
spawn_dungeon: 4. THI LUYEN (DUNGEON) [K4]
World: test
Toa do: x -1730.229, y 94.860, z -960.841
```

### List NPC

- NPC Bi Canh
- NPC Bang Tang Dungeon

### Chuc Nang Suy Ra Tu Gameplay

#### NPC Bi Canh

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | `/warps`, `/warp`, `/warp dungeon` |
| Nguon | `warp_menu.yml`, `huongdan_menu.yml`, `Dungeon.md` |
| Vai tro gameplay | Dua nguoi choi vao khu dungeon de farm gear, vat pham hiem, Dot Pha Dan va tai nguyen progression |

#### NPC Bang Tang Dungeon

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | Chua thay NPC entity rieng |
| Nguon | `Dungeon.md`, `gameplay.md` |
| Vai tro gameplay | Giai thich moi tang dungeon yeu cau canh gioi va thuc luc nao |

Dungeon som game duoc notes cu nhac den:

| Tang | Ten | Yeu cau goi y |
| :--- | :--- | :--- |
| 1 | Yeu Thu Lam | Luyen Khi So Ky, thuc luc 500 |
| 2 | Am Hon Dong | Luyen Khi Hau Ky, thuc luc 1,500 |
| 3 | Hoa Diem Son | Truc Co So Ky, thuc luc 3,000 |
| 4 | Bang Phong Coc | Truc Co Hau Ky, thuc luc 6,000 |

Flow gameplay chinh o K4:

- Vao Bi Canh theo moc canh gioi va thuc luc.
- Danh quai va boss de farm gear, skill book, trung Linh Thu, Tien Hoa Thach va Dot Pha Dan.
- Quay lai K3/K5 de tiep tuc nang luc chien va dot pha.

## Khu 5 - Dot Pha va Chuyen Sinh

Khu 5 la diem nguoi choi kiem tra dieu kien, kich hoat dot pha va xu ly cac he nang gioi han nhu chuyen sinh. Notes cu mo ta Dot Pha la buoc song sot qua Thien Loi Kiep de len canh gioi moi.

```text
spawn_dotpha_chuyensinh: 5. DOT PHA - CHUYEN SINH [K5]
World: test
Toa do: x -1723.166, y 94.860, z -1020.303
```

### List NPC

- NPC Dot Pha
- NPC Chuyen Sinh
- NPC Kiem Tra Dieu Kien

### Chuc Nang Suy Ra Tu Gameplay

#### NPC Dot Pha

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | `/dotpha` |
| Nguon | `huongdan_menu.yml`, `dotpha.md`, `gameplay.md` |
| Vai tro gameplay | Kich hoat vuot Kiep Loi de tien len dai canh gioi moi |

#### NPC Chuyen Sinh

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | Chua thay lenh ro rang trong phan da doc |
| Nguon | Hologram khu K5, notes cu |
| Vai tro gameplay | Moc gameplay muon game/endgame de reset hoac mo them gioi han phat trien neu server co dung he nay |

#### NPC Kiem Tra Dieu Kien

| Muc | Noi dung |
| :--- | :--- |
| Lenh/menu | Ho so thong tin, checklist dot pha |
| Nguon | `Spawn_Infomation`, `dotpha.md`, `gameplay.md` |
| Vai tro gameplay | Giup nguoi choi xem da du Tu Vi, du thuc luc va du vat pham chua truoc khi kich hoat Kiep Loi |

Dieu kien gameplay co the gan voi K5:

| Dieu kien | Ghi chu |
| :--- | :--- |
| Du Tu Vi | Nguoi choi dat moc canh gioi tiep theo |
| Du dieu kien dot pha | Co the gom canh gioi, thuc luc, vat pham hoac cooldown tuy config thuc te |
| Song sot Thien Loi Kiep | Thanh cong thi len canh gioi; that bai co hinh phat hoac cooldown |

Flow gameplay chinh o K5:

- Kiem tra moc Tu Vi va thuc luc.
- Chuan bi vat pham nhu Dot Pha Dan, Ho The Phu, Thien Loi Ho Phu neu server co ap dung.
- Kich hoat Dot Pha, song sot qua Kiep Loi, mo khoa canh gioi moi va noi dung moi.

## NPC Spawn Chung

Nhung NPC nay khong gan truc tiep voi K1-K5 trong hologram khu, nhung la hub chuc nang quan trong.

| NPC | Hologram | World/toa do | Action | Vai tro |
| :--- | :--- | :--- | :--- | :--- |
| `Spawn_Menu` | `Spawn_Menu` | `Spawn`, x `1000.5`, y `65.0`, z `1018.5` | Player command `menu` | Mo menu chinh server |
| `Spawn_HuongDan` | `Spawn_Huongdan` | `test`, x `-1725.800`, y `110.0`, z `-714.738` | Player command `huongdan` | Mo huong dan MineRua |
| `Spawn_Shop` | `Spawn_Shop` | `Spawn`, x `1007.5`, y `64.0`, z `1007.5` | Chua thay action ro trong config doc duoc | Cua hang `/shop` theo hologram |
| `Spawn_AH` | `Spawn_AH` | `Spawn`, x `986.963`, y `65.0`, z `1017.904` | Chua thay action ro trong config doc duoc | Thien Bao Cac `/ah` theo hologram |
| `Spawn_Quest` | `Spawn_Quest` | `Spawn`, x `992.5`, y `65.0`, z `1017.5` | Chua thay action ro trong config doc duoc | Nhiem vu `/quest` theo hologram |
| `Spawn_Team` | `Spawn_Team` | `Spawn`, x `1008.5`, y `65.0`, z `1016.5` | Chua thay action ro trong config doc duoc | Lien minh/Tong Mon, lien quan `/team` |

## Hologram Khong Gan NPC

| Hologram | Noi dung | Ghi chu |
| :--- | :--- | :--- |
| `Welcome_title` | Logo/anh title tai Spawn | Trang tri chao mung |
| `Welcome` | Gioi thieu the gioi Tu Tien | Co mo ta Dungeon, Do De, Trang Bi, Luc Chien |
| `TOP_Money` | Dua top dia chu/money | Bang top kinh te |
| `TOP_Kills` | Dua top tho san/kills | Bang top PvP/kills |
| `Spawn_Huongdan2` | Dau `?` lon | Chi dan phu tai Spawn, khong link NPC |
| `Tutorial_1_BuNhin` | Danh bai 5 bu nhin de tiep tuc | Buoc combat tutorial |

## Can Check Ingame

| Muc | Ly do can check |
| :--- | :--- |
| NPC K2 dat truc tiep tai hologram `spawn_luyenky` | Config chi thay NPC Mon Phai o vung spawn/test va tutorial, chua thay NPC rieng tai toa do K2 |
| NPC K3 Tu Luyen/De Tu/Nhap Than | Gameplay va menu ro, nhung `FancyNpcs` chua co ID NPC tuong ung |
| NPC K4 Dungeon | Hologram K4 co khu, nhung gameplay hien dung `/warp dungeon`; chua thay NPC dungeon rieng |
| NPC K5 Dot Pha/Chuyen Sinh | Hologram K5 co khu, nhung chua thay NPC rieng hoac lenh chuyen sinh trong du lieu da doc |
| Action cua `Spawn_Shop`, `Spawn_AH`, `Spawn_Quest`, `Spawn_Team` | Hologram co lenh hien thi, nhung NPC config chua co click action ro rang |
