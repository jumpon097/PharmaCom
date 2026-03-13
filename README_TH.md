# PharmaCom GitHub Pages (index เดิมเป็นหลัก)

ชุดนี้ออกแบบตามที่ต้องการ:
- เก็บ `index.html` เดิมเป็นหน้าหลัก
- เพิ่มปุ่ม **รวมลิงก์ Dashboard / วอร์ด** ที่หน้าแรก
- มีหน้า `links/` สำหรับรวมลิงก์ทั้งหมด
- หน้า `dashboard/` และ `wards/.../` เป็น PWA wrapper แยกหน้า
- ทุกหน้าชี้ไปที่ Apps Script URL แบบ `/exec`

## URL GAS ที่ใช้อยู่
https://script.google.com/macros/s/AKfycbwi1Uj2CS4SKnzxBTNFgkHCmUQvYd8wkxKR5A25_H_6xAdS-F_hOoTIqDD_D8reTY1hLA/exec

## วิธีลงแบบง่าย
1. แตก zip
2. เข้า repo `PharmaCom`
3. อัปโหลด **ไฟล์และโฟลเดอร์ข้างในชุดนี้** ไปที่ root ของ repo
4. อย่าอัปโหลดเป็นโฟลเดอร์ครอบอีกชั้น
5. ที่ root ของ repo ควรเห็นประมาณนี้:
   - index.html
   - manifest.json
   - sw.js
   - links/
   - dashboard/
   - wards/
6. ไปที่ GitHub > Settings > Pages
7. เลือก Deploy from a branch
8. Branch = main, Folder = / (root)
9. Save

## ลิงก์ตัวอย่างหลังขึ้น GitHub Pages
- หน้าเดิมหลัก: `/PharmaCom/`
- หน้ารวมลิงก์: `/PharmaCom/links/`
- Dashboard: `/PharmaCom/dashboard/`
- ICU: `/PharmaCom/wards/icu/`

## หมายเหตุสำคัญ
ถ้า Apps Script ของคุณยังไม่รองรับ `?view=dashboard` และ `?view=ward&id=...`
ใน `doGet(e)` หน้าใน iframe อาจยังเด้งกลับหน้าแรก
อันนี้ต้องแก้ฝั่ง GAS เพิ่ม
