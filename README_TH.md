# PharmaCom GitHub Pages (แบบง่ายและดีที่สุดตอนนี้)

ชุดไฟล์นี้ทำไว้สำหรับ **GitHub Pages + PWA wrapper**  
โดยหน้าเว็บอยู่บน GitHub Pages และเปิดระบบจริงจาก Google Apps Script ผ่าน `iframe`

## ปลายทาง Apps Script ที่ตั้งไว้แล้ว
`https://script.google.com/macros/s/AKfycbwi1Uj2CS4SKnzxBTNFgkHCmUQvYd8wkxKR5A25_H_6xAdS-F_hOoTIqDD_D8reTY1hLA/exec`

## หน้าใช้งานที่มีให้
- `/dashboard/`
- `/wards/sarocha/`
- `/wards/sattabongkot/`
- `/wards/busabong/`
- `/wards/busaban/`
- `/wards/patama/`
- `/wards/pathumman/`
- `/wards/icu/`
- `/wards/bmt/`

## วิธีลงแบบง่ายที่สุดบน GitHub (ผ่านเว็บ ไม่ต้องใช้คำสั่ง)
1. เข้า repo ของคุณบน GitHub
2. กด **Add file** > **Upload files**
3. ลากไฟล์ทั้งหมดในโฟลเดอร์นี้ขึ้นไป
4. เลื่อนลงล่าง กด **Commit changes**
5. ไปที่ **Settings** > **Pages**
6. ที่หัวข้อ **Build and deployment**
   - Source = **Deploy from a branch**
   - Branch = **main**
   - Folder = **/ (root)**
7. กด Save
8. รอ 1-3 นาที GitHub จะสร้างลิงก์เว็บไซต์ให้

## ลิงก์ที่จะได้ (ตัวอย่าง)
ถ้า repo ชื่อ `PharmaCom`
- `https://jumpon097.github.io/PharmaCom/`
- `https://jumpon097.github.io/PharmaCom/dashboard/`
- `https://jumpon097.github.io/PharmaCom/wards/sarocha/`

## ถ้าจะอัปเดตปลายทาง Apps Script ภายหลัง
ให้ค้นหาคำนี้ในไฟล์:
`https://script.google.com/macros/s/AKfycbwi1Uj2CS4SKnzxBTNFgkHCmUQvYd8wkxKR5A25_H_6xAdS-F_hOoTIqDD_D8reTY1hLA/exec`

แล้วแทนเป็น URL `/exec` ตัวใหม่ในทุกไฟล์ `index.html`

## หมายเหตุ
- ถ้า Apps Script ยังไม่เปิดให้ใช้งานแบบ Web App URL บางหน้าจะไม่ขึ้น
- ถ้าแก้ Code.gs แล้วอย่าลืม Deploy เวอร์ชันใหม่
- PWA จะติดตั้งได้ดีบน Chrome/Edge มากกว่า Safari
