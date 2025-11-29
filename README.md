คำอธิบายโครงการ ระบบติดตามค่า BMI และประวัติสุขภาพเบื้องต้น ที่ช่วยให้ผู้ใช้สามารถคำนวณค่า BMI บันทึกประวัติ และดูแนวโน้มการเปลี่ยนแปลงของน้ำหนักและค่า BMI

ฟีเจอร์หลัก

คำนวณค่า BMI จากน้ำหนักและส่วนสูง
แสดงผลการแปลความหมาย BMI (ผอม, ปกติ, น้ำหนักเกิน, อ้วน)
บันทึกประวัติการวัดพร้อมวันที่
แสดงประวัติในรูปแบบตาราง
กราฟเส้นแสดงแนวโน้มการเปลี่ยนแปลง
ลบข้อมูลที่ไม่ต้องการ
Input Validation
Responsive Design
เทคโนโลยีที่ใช้

Frontend: React.js
UI Library: Tailwind CSS
Charts: Recharts
Icons: Lucide React
Storage: LocalStorage (Browser)
การติดตั้งและรัน

วิธีที่ 1: รันผ่าน Create React App

Clone repository:
git clone https://github.com/yourusername/healthtrack-bmi.git
cd healthtrack-bmi
ติดตั้ง dependencies:
npm install
รันโปรเจกต์:
npm start
เปิดเบราว์เซอร์ที่: http://localhost:3000
วิธีที่ 2: รันไฟล์ HTML แบบง่าย (Standalone)

เปิดไฟล์ index.html ด้วยเบราว์เซอร์
ใช้งานได้ทันที ไม่ต้องติดตั้งอะไร
โครงสร้างโค้ด

healthtrack-bmi/
├── src/
│   ├── components/
│   │   └── BMITracker.jsx      # Main Component
│   ├── App.js                   # Root Component
│   └── index.js                 # Entry Point
├── public/
│   └── index.html
├── package.json
└── README.md
วิธีการใช้งาน

กรอกข้อมูล: ใส่น้ำหนัก (kg) และส่วนสูง (cm)
คำนวณ: กดปุ่ม "คำนวณและบันทึก"
ดูผลลัพธ์: ระบบจะแสดงค่า BMI พร้อมคำแนะนำ
ดูประวัติ: ตรวจสอบประวัติการวัดในตาราง
ดูกราฟ: วิเคราะห์แนวโน้มจากกราฟเส้น
ลบข้อมูล: กดปุ่ม "ลบ" ถ้าต้องการลบข้อมูล
สูตรการคำนวณ BMI

BMI = น้ำหนัก (kg) / (ส่วนสูง (m))²
เกณฑ์การแปลผล:

ผอม: BMI < 18.5
ปกติ: 18.5 ≤ BMI < 25
น้ำหนักเกิน: 25 ≤ BMI < 30
อ้วน: BMI ≥ 30
ความปลอดภัยของข้อมูล

ข้อมูลทั้งหมดเก็บใน LocalStorage ของเบราว์เซอร์
ไม่มีการส่งข้อมูลไปยังเซิร์ฟเวอร์ภายนอก
ข้อมูลจะถูกลบเมื่อล้าง Browser Cache
จัดทำโดย

ชื่อ: [ณัฐพล วงศ์สัมฤทธิ์]
รหัสนักศึกษา: [1670707312] SECTION 227C
