YAI NORI — React 18 FIX

ข้อผิดพลาดเดิม: React 16 ไม่มี useState/useEffect จึงเปิดเว็บไม่ได้
ไฟล์นี้เรียก React 18 จาก cdnjs พร้อมแหล่งสำรอง jsDelivr/unpkg และใช้ createRoot

วิธี Deploy: อัปโหลด index.html พร้อม vendor/ และ assets/ ทั้งหมดเป็นไฟล์ Static Assets ภายใต้ root เดียวกัน
ต้องเชื่อมต่ออินเทอร์เน็ตสำหรับ React 18 CDN, Tailwind CDN และ Google Fonts
ห้ามนำโค้ด JSX วางเป็น index.html
หากเว็บยังไม่เปิดให้ตรวจ Network ว่า CDN ถูกบล็อกหรือไม่
ฐานข้อมูลยังต้องเชื่อมต่อแยกต่างหาก หากยังไม่เชื่อมจะทำงานด้วยข้อมูลตัวอย่าง/localStorage
