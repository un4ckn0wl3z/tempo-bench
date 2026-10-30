# Tempo Bench

เมโทรนอมบนเว็บที่ตั้งค่าได้ละเอียด ไฟล์เดียว ไม่ต้อง build

- BPM 20–400 ละเอียดถึงทศนิยม, Tap tempo, ชื่อเทมโป (Largo → Prestissimo)
- กำหนดน้ำหนักทีละจังหวะ (เน้น / ปกติ / เบา / เงียบ), time signature 1–16 / 2,4,8,16
- ซอยโน้ต 1–8, swing 50–75%, polyrhythm
- เสียง Click / Woodblock / Beep / Cowbell / Hi-hat, ปรับความดังและ pitch แยกชั้น
- ฝึกซ้อม: ไต่ความเร็ว, gap click, สุ่มเงียบ, นับนำ, ตั้งเวลาหยุด
- พรีเซ็ต (เก็บใน localStorage)

คีย์ลัด: `Space` เล่น/หยุด · `↑` `↓` ±1 BPM (`Shift` ±10) · `T` แตะจังหวะ

เสียงสร้างด้วย Web Audio API และตั้งเวลาล่วงหน้า (lookahead scheduler) ผ่าน Web Worker เพื่อให้จังหวะแม่นแม้แท็บอยู่เบื้องหลัง
