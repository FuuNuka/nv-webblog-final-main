# ☕ NV Web Blog 

โปรเจกต์ระบบเว็บบล็อกแบบ Full-Stack ที่พัฒนาขึ้นมาเพื่อใช้สำหรับเขียนและจัดการบทความเว็บบล็อก

## 🛠 Tech Stack
- **Frontend:** Vue.js (Webpack)
- **Backend:** Node.js, Express.js

## ✨ Key Features (ความสามารถหลัก)
- **Full CRUD Operations:** สามารถสร้าง (Create), อ่าน (Read), แก้ไข (Update), และลบ (Delete) บทความเว็บบล็อกได้
- **Full-Stack Architecture:** แยกระบบฝั่งหน้าบ้าน (Client) และหลังบ้าน (Server) ออกจากกันอย่างชัดเจน และสื่อสารกันผ่าน RESTful API
- **Dynamic Content:** แสดงรายการบทความพร้อมวันที่สร้าง (Create Date) และรูปภาพประกอบ

## 🚀 How to Run (วิธีรันโปรเจกต์)
โปรเจกต์นี้ถูกแบ่งเป็น 2 ส่วนคือหน้าเว็บ (`client`) และระบบหลังบ้าน (`server`) คุณจำเป็นต้องเปิด Terminal 2 หน้าต่างเพื่อรันระบบควบคู่กัน

### 🖥️ 1. รันฝั่ง Server (ระบบหลังบ้าน)
1. เข้าไปในโฟลเดอร์ server: `cd server`
2. ติดตั้งแพ็กเกจ: `npm install`
3. รันเซิร์ฟเวอร์: `npm run dev` (หรือ `npx nodemon src/app.js`)

### 💻 2. รันฝั่ง Client (หน้าเว็บ Vue.js)
1. เข้าไปในโฟลเดอร์ client: `cd client`
2. ติดตั้งแพ็กเกจ: `npm install`
3. รันหน้าเว็บ: `npm run dev` 
4. เปิดเบราว์เซอร์และเข้าไปที่ `http://localhost:8080`
