# Plain Thai Dev Communication

Skill / Custom Instruction สำหรับบังคับให้ AI ตอบกลับ Developer เป็นภาษาไทยที่อ่านง่าย เป็นธรรมชาติ และไม่แปลคำศัพท์ Technical (ลดปัญหา AI ตอบแบบไทยคำอังกฤษคำ)

## วิธีนำไปใช้งาน

คุณสามารถคัดลอกเนื้อหาทั้งหมดในไฟล์ `SKILL.md` ไปตั้งค่าตามเครื่องมือ AI ที่คุณใช้งานได้ดังนี้:

- **Cursor IDE:** นำไปวางในไฟล์ `.cursorrules` ที่ Root directory ของโปรเจกต์
- **ChatGPT:** นำเนื้อหาไปวางใน Settings -> Personalization -> Custom instructions (ช่อง How would you like ChatGPT to respond?)
- **Claude:** นำไปตั้งค่าในช่อง Project instructions (สำหรับแผน Pro) หรือใช้เป็น System Prompt ใน API

## ทำไมถึงควรใช้คำสั่งนี้?

- ช่วยลดความหงุดหงิดจากการที่ AI พยายามแปลคำศัพท์เฉพาะทาง (เช่น แปล deployment เป็น การนำระบบขึ้นใช้งานในบริบทที่ไม่เหมาะสม)
- โครงสร้างการตอบกลับจะถูกปรับให้เหมาะกับบริบทของ Developer ทั้งงาน Implementation, Debugging และ Code Review

## ตัวอย่างผลลัพธ์ (Before / After)

**Bad Pattern:**
เราจะ implement middleware เพื่อ handle auth flow ก่อน redirect user ไป dashboard

**Good Pattern:**
เราจะเพิ่ม `middleware` เพื่อตรวจสิทธิ์ผู้ใช้ก่อนพาไปหน้า dashboard