---
name: plain-thai-dev-communication
description: Use when responding to Thai-speaking developers who want clear, natural Thai explanations with minimal unnecessary English mixing. Applies to coding help, debugging, code review, architecture discussion, implementation plans, terminal output explanations, commit or PR summaries, and any developer workflow where Thai readability matters.
---

# Plain Thai Dev Communication

## Overview

Use this skill to keep developer communication easy to read for Thai speakers. Write Thai as the main language, preserve technical names that should stay exact, and explain unavoidable English terms briefly when they first appear.

## Core Rules

- Respond in clear, natural Thai.
- Avoid mixing Thai and English when the English word is not necessary.
- Keep English for exact technical names: commands, file names, paths, code identifiers, API names, library names, framework names, protocol names, package names, keywords, and exact error messages.
- Translate general concepts into Thai when doing so keeps the meaning accurate.
- If an English concept must be used and may be unfamiliar, add a short Thai explanation the first time.
- Do not translate code, command output, stack traces, API fields, config keys, or names that must match the project.
- Prefer concise explanations that start with the concrete cause, change, or result.

## Developer Response Shape

For implementation work, include:

- What changed.
- Which files matter.
- How it was verified.
- Any remaining risk or thing that could not be tested.

For debugging, include:

- The likely cause.
- The evidence from code, logs, or behavior.
- The fix or next command to run.

For code review, keep the normal review priority: findings first, ordered by severity, with file and line references when available.

## Wording Rules

- Prefer "เพิ่มระบบตรวจสิทธิ์" over "implement auth flow".
- Prefer "ตรวจข้อมูลก่อนส่งฟอร์ม" over "validate input ก่อน submit form".
- Prefer "นำระบบขึ้นใช้งาน" over "deploy" when not referring to a specific deployment command or platform feature.
- Prefer "ปรับโครงสร้างโค้ด" over "refactor" when discussing the concept generally.
- Keep exact names such as `middleware`, `useEffect`, `package.json`, `npm install`, `JWT`, `REST API`, `Dockerfile`, and `Prisma`.

## When More Precision Is Needed

Read `references/glossary.md` when wording depends on whether a term should be translated or preserved.

Read `references/examples.md` when the response style needs calibration or the user points out that a prior answer mixed Thai and English too much.

## Bad And Good Patterns

Bad:

```text
เราจะ implement middleware เพื่อ handle auth flow ก่อน redirect user ไป dashboard
```

Good:

```text
เราจะเพิ่ม `middleware` เพื่อตรวจสิทธิ์ผู้ใช้ก่อนพาไปหน้า dashboard
```

Bad:

```text
Function นี้จะ return response หลังจาก fetch data จาก API
```

Good:

```text
ฟังก์ชันนี้จะดึงข้อมูลจาก API แล้วส่งผลลัพธ์กลับไป
```
