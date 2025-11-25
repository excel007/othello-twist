# 🎮 Othello Twist

> **"Othello ที่ไม่เหมือนใคร"** - เกม Othello ที่มีระบบ Power-Up, Random Event และความเซอร์ไพรส์มากมาย!

![Othello Twist](https://img.shields.io/badge/Game-Othello%20Twist-00f5ff?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-2.0-ff00ff?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📖 เกี่ยวกับเกม

Othello Twist เป็นเกม Othello (Reversi) ที่ถูกพัฒนาให้มีความสนุกและตื่นเต้นมากขึ้น ด้วยระบบ Power-Up ที่พลิกเกม, Random Event ที่ไม่คาดคิด และ AI ที่ท้าทาย 3 ระดับความยาก

### ✨ จุดเด่น

- 🎯 **4 โหมดเกม** - Classic, Chaos, Strategy, Speedrun
- 💥 **6 Power-Ups** - Bomb, Swap, Shield, Double Turn, Ghost, Sniper
- 🌀 **6 Random Events** - Earthquake, Black Hole, Rainbow, Time Warp, Mirror, Chaos
- 🤖 **AI 3 ระดับ** - ง่าย, ปานกลาง, ยาก (ใช้ Minimax Algorithm)
- 📱 **รองรับ Mobile** - เล่นได้ทั้งบน Desktop และ Mobile
- 🎨 **ดีไซน์ Neon Cyberpunk** - สวยงามและทันสมัย

---

## 🚀 วิธีเล่น

### ติดตั้ง

ไม่ต้องติดตั้งอะไรเลย! แค่เปิดไฟล์ HTML ในเบราว์เซอร์

```bash
# Clone repository
git clone https://github.com/excel007/othello-twist.git

# เปิดไฟล์ index.html ในเบราว์เซอร์
```

หรือ [เล่นออนไลน์ได้ที่นี่](https://excel007.github.io/othello-twist/)

### กติกาพื้นฐาน

1. ผู้เล่นใช้หมากสีดำ ⚫, AI ใช้หมากสีขาว ⚪
2. วางหมากเพื่อ "ขนาบ" หมากฝ่ายตรงข้าม
3. หมากที่ถูกขนาบจะพลิกเป็นสีของผู้วาง
4. ผู้ที่มีหมากมากกว่าตอนจบเกมเป็นผู้ชนะ

---

## 🎮 โหมดเกม

| โหมด | คำอธิบาย |
|------|----------|
| 🎯 **Classic** | Othello ดั้งเดิม ไม่มี Power-Up หรือ Event |
| 🌪️ **Chaos** | มี Power-Up และ Random Event เต็มรูปแบบ |
| 🧠 **Strategy** | เริ่มต้นมี Power-Up 3 ชิ้น ไม่มี Random Event |
| ⚡ **Speedrun** | Power-Up ปรากฏบ่อยขึ้น |

---

## 💥 Power-Ups

| Icon | ชื่อ | ผลกระทบ |
|------|------|---------|
| 💣 | **Bomb** | ระเบิดหมาก 3×3 รอบตำแหน่งที่เลือก |
| 🔄 | **Swap** | สลับสีหมากทั้งกระดาน ดำ↔ขาว |
| 🛡️ | **Shield** | ป้องกันหมาก 1 ตัวไม่ให้ถูกพลิก 3 ตา |
| ⚡ | **Double** | เดินได้ 2 ครั้งติดต่อกัน |
| 👻 | **Ghost** | วางหมากที่ไหนก็ได้โดยไม่ต้องขนาบ |
| 🎯 | **Sniper** | พลิกหมากศัตรูตัวไหนก็ได้ |

**วิธีใช้:** คลิกที่ Power-Up ด้านล่างกระดาน แล้วคลิกตำแหน่งที่ต้องการ

---

## 🌀 Random Events

เกิดขึ้นทุก 5-8 ตาในโหมด Chaos!

| Icon | ชื่อ | ผลกระทบ |
|------|------|---------|
| 🌊 | **Earthquake** | หมากทั้งหมดเลื่อนไปทิศทางสุ่ม |
| 🕳️ | **Black Hole** | เกิดหลุมดำ 4 ช่อง วางหมากไม่ได้ |
| 🌈 | **Rainbow** | หมาก 5 ตัวกลายเป็นหมากทอง (2 คะแนน) |
| ⏰ | **Time Warp** | ย้อนเวลากลับไป 3 ตา |
| 🎭 | **Mirror** | กระดานสะท้อนแนวนอน |
| 🌪️ | **Chaos** | หมาก 6 ตัวสลับตำแหน่งกัน |

---

## 🏆 ระบบ Combo

| Combo | เงื่อนไข | รางวัล |
|-------|----------|--------|
| 🔥 **Triple Flip** | พลิกหมาก 8+ ตัวในตาเดียว | +1 Power-Up สุ่ม |
| 👑 **Corner Master** | ยึดมุมกระดาน | หมากกลายเป็นหมากทอง |

---

## 🤖 AI

| ระดับ | อัลกอริทึม |
|-------|-----------|
| 😊 ง่าย | สุ่มเลือก move |
| 😐 ปานกลาง | Greedy + Corner Priority |
| 😈 ยาก | Minimax + Alpha-Beta Pruning (depth 4) |

---

## 📁 โครงสร้างไฟล์

```
othello-twist/
├── index.html    # ไฟล์เกมหลัก
├── SRS.md        # เอกสาร Software Requirements Specification
└── README.md     # ไฟล์นี้
```

---

## 🛠️ เทคโนโลยีที่ใช้

- **React 18** - UI Framework
- **Tailwind CSS** - Styling
- **Web Audio API** - Sound Effects
- **Babel** - JSX Compilation

ทั้งหมดโหลดผ่าน CDN ไม่ต้องติดตั้งอะไรเพิ่ม!

---

## 📱 รองรับอุปกรณ์

- ✅ Desktop (Chrome, Firefox, Safari, Edge)
- ✅ Mobile (iOS Safari, Android Chrome)
- ✅ Tablet

---

## 🎨 Screenshots

### หน้าเมนู
เลือกโหมดเกมและระดับความยาก

### หน้าเกม
กระดาน 8×8 พร้อม Power-Ups และ Event Counter

### Random Event
Popup แสดงเมื่อเกิด Event พิเศษ

---

## 📄 License

MIT License - ใช้งานได้อย่างอิสระ

---

## 👨‍💻 ผู้พัฒนา

สร้างด้วย ❤️ โดย Claude AI

---

## 🙏 ขอบคุณ

- กติกา Othello มาตรฐานจาก World Othello Federation
- Minimax Algorithm จาก AI/ML Community
- ไอเดีย Power-Ups จากเกม Battle Royale ต่างๆ

---

**สนุกกับการเล่น! 🎮**
