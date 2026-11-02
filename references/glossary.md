# Glossary

Use this glossary as a living reference. Prefer the Thai wording for general explanations, but keep the English term when it is an exact name in code, a command, a library, a framework, an API field, or an error message.

## Prefer Thai For General Concepts

| English | Preferred Thai |
| --- | --- |
| state | สถานะ |
| render | แสดงผล |
| request | คำขอ |
| response | คำตอบกลับ |
| dependency | แพ็กเกจที่โค้ดต้องใช้ |
| deploy | นำระบบขึ้นใช้งาน |
| refactor | ปรับโครงสร้างโค้ด |
| validate | ตรวจข้อมูล |
| authentication | การยืนยันตัวตน |
| authorization | การตรวจสิทธิ์ |
| cache | แคช |
| configuration | การตั้งค่า |
| environment variable | ตัวแปรสภาพแวดล้อม |
| database migration | การปรับโครงสร้างฐานข้อมูล |
| schema | โครงสร้างข้อมูล |
| payload | ข้อมูลที่ส่งไปกับคำขอ |
| endpoint | จุดเรียก API |
| handler | ส่วนจัดการคำขอ |
| fallback | ทางสำรอง |
| timeout | หมดเวลารอ |
| retry | ลองใหม่ |

## Preserve English For Exact Technical Names

- Commands: `npm install`, `git status`, `docker compose up`
- Files and paths: `package.json`, `src/app/page.tsx`, `.env`
- Code identifiers: `useEffect`, `handleSubmit`, `UserService`
- Protocols and formats: HTTP, JSON, YAML, SQL
- Libraries and frameworks: React, Next.js, Express, Prisma, Tailwind CSS
- Platform or product names: GitHub Actions, Vercel, Docker, PostgreSQL
- Exact errors: keep the original error text, then explain it in Thai.

## First-Mention Pattern

When preserving an English term that may be unclear, explain it once:

```text
ปัญหาอยู่ที่ `middleware` ซึ่งเป็นส่วนที่ทำงานก่อนคำขอจะไปถึงหน้าเว็บจริง
```

After that, use the exact term without repeating the explanation if the context is clear.
