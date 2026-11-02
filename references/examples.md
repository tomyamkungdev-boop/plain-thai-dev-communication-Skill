# Examples

Use these examples to calibrate tone and wording.

## Implementation Summary

Avoid:

```text
ผม implement feature ใหม่และ update validation logic ใน form component แล้ว
```

Prefer:

```text
ผมเพิ่มฟีเจอร์ใหม่และแก้ logic ตรวจข้อมูลใน `Form` แล้ว
```

## Debugging

Avoid:

```text
Error นี้เกิดจาก dependency missing ทำให้ runtime load module ไม่ได้
```

Prefer:

```text
ข้อผิดพลาดนี้เกิดจากแพ็กเกจที่โค้ดต้องใช้ยังไม่ได้ติดตั้ง ทำให้ระบบโหลด module ไม่ได้ตอนรัน
```

## Architecture

Avoid:

```text
เราควร split service layer ออกมาเพื่อ improve maintainability และ testability
```

Prefer:

```text
ควรแยกชั้น service ออกมา เพื่อให้ดูแลโค้ดและเขียน test ได้ง่ายขึ้น
```

## Terminal Output

Avoid:

```text
Command fail เพราะ permission denied ตอน write file
```

Prefer:

```text
คำสั่งล้มเหลวเพราะไม่มีสิทธิ์เขียนไฟล์ ต้นเหตุคือข้อความ `permission denied`
```

## Code Review

Avoid:

```text
Finding: This can cause race condition when multiple requests update same resource.
```

Prefer:

```text
จุดที่ควรแก้: โค้ดนี้อาจเกิดปัญหาการเขียนข้อมูลชนกัน เมื่อมีหลายคำขอแก้ resource เดียวกันพร้อมกัน
```
