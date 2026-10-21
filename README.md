# KT Thai Reference

เว็บแอป Static/PWA สำหรับคลังศัพท์และดัชนีแหล่งข้อมูล Kill Team ภาษาไทยแบบไม่เป็นทางการ

## นำขึ้น GitHub Pages

1. สร้าง repository ใหม่บน GitHub เช่น `kt-thai-reference`
2. แตก ZIP แล้วอัปโหลดไฟล์ทั้งหมด โดยให้ `index.html` อยู่ที่ root ของ repository
3. เปิด `Settings` > `Pages`
4. ใน `Build and deployment` เลือก `Deploy from a branch`
5. เลือก branch `main` และ folder `/(root)` แล้วกด `Save`
6. รอประมาณ 1-3 นาที แล้วเปิด URL ที่ GitHub แสดง

URL โดยทั่วไปจะเป็น:

`https://USERNAME.github.io/kt-thai-reference/`

## ทดสอบบนเครื่อง

ต้องเปิดผ่านเว็บเซิร์ฟเวอร์ ไม่ควรดับเบิลคลิก index.html โดยตรง

```bash
python3 -m http.server 8080
```

แล้วเปิด `http://localhost:8080`

## แก้ไขข้อมูล

- `data/glossary.json` คลังศัพท์ EN/TH
- `data/teams.json` ดัชนีทีมและลิงก์ต้นทาง
- `data/sources.json` แหล่งข้อมูลทางการ

## ข้อควรระวัง

โปรเจกต์ตั้งใจไม่รวม artwork, logo, rules text หรือ stats ฉบับเต็มจาก Games Workshop โปรดตรวจสอบสิทธิ์ก่อนเพิ่มและเผยแพร่เนื้อหาใด ๆ
