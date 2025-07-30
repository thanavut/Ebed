# หน้า Report (รายงานกิจกรรมผู้ใช้)

## วัตถุประสงค์:
ให้แอดมินตรวจสอบกิจกรรมของผู้ใช้ ย้อนหลังตามช่วงเวลาและประเภทกิจกรรม

## Fields & Logic:
- `startDate`, `endDate` → กรองวันที่เพื่อดูเฉพาะช่วงที่สนใจ
- `actionType` → กรองประเภท เช่น login, update, reset
- ตารางแสดงผลดึงจาก action logs โดยใช้ role-based access

## Audit Standard:
- ทุกข้อมูลมาจาก ActionLogs, ไม่มี manual entry
- ไม่มีปุ่ม export เพื่อหลีกเลี่ยงการเก็บข้อมูลซ้ำซ้อน
- CSS คงโทน beige/gray/blue และใช้ฟอนต์ Kanit ตามระบบหลัก

## ข้อจำกัด:
- ไม่แสดงข้อมูลที่ละเอียดเกินความจำเป็น เช่น IP หรือ device (เพื่อ Lean design)
