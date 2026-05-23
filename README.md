# 🌍 Life Travel Bucket Planner (LTBP)

แอปวางแผนการเดินทางตลอดชีวิต — สร้างด้วย vanilla JS ไฟล์เดียว ใช้งานได้ทันทีในเบราว์เซอร์

## ✨ Features (MVP)

- **🗺️ Country Selector** — เลือกประเทศที่อยากไปจากทั่วโลก จัดกลุ่มตามทวีป
- **📅 Year Plan** — จัดตารางทริปตามปี พร้อมงบประมาณและจำนวนวัน
- **🌤️ Best Months** — แสดงเดือนที่ดีที่สุดสำหรับแต่ละประเทศ (อุณหภูมิ 12-22°C + ฤดูแล้ง)
- **💰 Budget Tracker** — รวมงบประมาณทั้งหมดอัตโนมัติ
- **📤 Share** — Export เป็นไฟล์ .html ส่งให้เพื่อนเปิดดูได้เลย
- **💾 Auto Save** — บันทึกอัตโนมัติใน localStorage

## 🚀 วิธีใช้

### เปิดใช้งาน (Local)
```bash
npx serve -l 5500 .
```
จากนั้นเปิด [http://localhost:5500](http://localhost:5500)

### เปิดใช้งาน (Direct)
ดับเบิ้ลคลิกไฟล์ `index.html` เปิดในเบราว์เซอร์ได้เลย

## 🗂️ โครงสร้างไฟล์

```
Bucket List/
├── index.html       # แอปทั้งหมด (HTML + CSS + JS รวมไฟล์เดียว)
├── .claude/
│   └── launch.json  # Config สำหรับ preview server
├── .gitignore
└── README.md
```

## 💡 Tech Stack

- **Vanilla JS** — ไม่มี framework ไม่ต้อง install อะไร
- **localStorage** — เก็บข้อมูลในเบราว์เซอร์
- **Single HTML file** — แชร์ง่าย พกพาได้

## 🗺️ Roadmap

- [ ] เพิ่มประเทศให้ครบ (Africa, Middle East, Americas)
- [ ] Trip Note บันทึกรายละเอียดแต่ละทริป
- [ ] Budget Chart แสดงกราฟงบประมาณต่อปี
- [ ] Export เป็น PDF
- [ ] Dark mode

## 📦 LocalStorage Keys

| Key | ข้อมูล |
|---|---|
| `ltbp3_profile` | ข้อมูลผู้ใช้ (อายุ, เกษียณ) |
| `ltbp3_sel` | ประเทศที่เลือก |
| `ltbp3_plan` | แผนการเดินทางแต่ละทริป |
| `ltbp3_note` | บันทึกส่วนตัว |
