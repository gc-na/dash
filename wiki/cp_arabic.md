# [ديبيان] Debian Almquist Shell (dash) cp الاستخدام: [نسخ الملفات والمجلدات]

## Overview
أمر `cp` يُستخدم في نظام التشغيل لنسخ الملفات والمجلدات من موقع إلى آخر. يُعتبر هذا الأمر من الأوامر الأساسية في نظام لينكس، ويتيح للمستخدمين إدارة الملفات بكفاءة.

## Usage
الصيغة الأساسية للأمر هي:

```bash
cp [options] [arguments]
```

## Common Options
- `-r`: يُستخدم لنسخ المجلدات بشكل متكرر (بما في ذلك المحتويات).
- `-i`: يُطلب تأكيد قبل الكتابة فوق الملفات الموجودة.
- `-u`: يُنسخ الملفات فقط إذا كانت المصدر أحدث من الهدف أو إذا لم يكن الهدف موجودًا.
- `-v`: يُظهر تفاصيل العمليات أثناء النسخ.

## Common Examples
- لنسخ ملف من مكان إلى آخر:

```bash
cp file.txt /path/to/destination/
```

- لنسخ مجلد وكل محتوياته:

```bash
cp -r /path/to/source_directory /path/to/destination_directory
```

- لنسخ ملف مع طلب تأكيد قبل الكتابة فوق الملف الموجود:

```bash
cp -i file.txt /path/to/destination/
```

- لنسخ ملف مع عرض تفاصيل النسخ:

```bash
cp -v file.txt /path/to/destination/
```

## Tips
- تأكد دائمًا من أنك في الدليل الصحيح قبل تنفيذ الأمر `cp` لتجنب الأخطاء.
- استخدم الخيار `-i` لتجنب الكتابة فوق الملفات المهمة عن طريق الخطأ.
- عند نسخ المجلدات، تأكد من استخدام الخيار `-r` لضمان نسخ جميع المحتويات.