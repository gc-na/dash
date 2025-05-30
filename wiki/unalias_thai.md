# [ไทย] Debian Almquist Shell (dash) unalias การใช้งาน: ลบการตั้งชื่อซ้ำ

## Overview
คำสั่ง `unalias` ใช้ในการลบการตั้งชื่อซ้ำที่ถูกสร้างขึ้นโดยคำสั่ง `alias` ในเชลล์ ซึ่งช่วยให้คุณสามารถคืนค่าการทำงานเดิมของคำสั่งที่ถูกตั้งชื่อซ้ำได้

## Usage
คำสั่งพื้นฐานสำหรับ `unalias` มีรูปแบบดังนี้:

```
unalias [options] [arguments]
```

## Common Options
- `-a`: ลบการตั้งชื่อซ้ำทั้งหมดที่มีอยู่
- `-p`: แสดงรายการการตั้งชื่อซ้ำที่มีอยู่ในปัจจุบัน

## Common Examples
1. ลบการตั้งชื่อซ้ำเฉพาะคำสั่ง:
   ```sh
   unalias ll
   ```

2. ลบการตั้งชื่อซ้ำทั้งหมด:
   ```sh
   unalias -a
   ```

3. แสดงการตั้งชื่อซ้ำที่มีอยู่:
   ```sh
   unalias -p
   ```

## Tips
- ตรวจสอบการตั้งชื่อซ้ำที่มีอยู่ก่อนที่จะลบ โดยใช้คำสั่ง `alias` เพื่อดูรายการทั้งหมด
- ใช้ `unalias` ในไฟล์ `.bashrc` หรือ `.profile` เพื่อจัดการการตั้งชื่อซ้ำเมื่อเริ่มต้นเชลล์ใหม่
- ระวังการลบการตั้งชื่อซ้ำที่อาจจะใช้งานอยู่เพื่อหลีกเลี่ยงความไม่สะดวกในการทำงาน