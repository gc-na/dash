# [ديبيان] Debian Almquist Shell (dash) ping الاستخدام: اختبار الاتصال بالشبكة

## Overview
أمر `ping` هو أداة تستخدم لاختبار الاتصال بين جهازين على الشبكة. يقوم بإرسال حزم بيانات إلى عنوان IP محدد ويقيس الوقت المستغرق للحصول على استجابة، مما يساعد في تحديد ما إذا كان الجهاز الآخر متصلًا بالشبكة أم لا.

## Usage
يمكن استخدام الأمر `ping` بالشكل التالي:

```bash
ping [options] [arguments]
```

## Common Options
- `-c <count>`: يحدد عدد حزم البيانات التي سيتم إرسالها.
- `-i <interval>`: يحدد الفاصل الزمني بين إرسال الحزم.
- `-t <ttl>`: يحدد قيمة TTL (Time To Live) للحزم.
- `-s <size>`: يحدد حجم الحزمة المرسلة.

## Common Examples
- **اختبار الاتصال بجهاز معين:**
```bash
ping 8.8.8.8
```

- **إرسال 4 حزم فقط:**
```bash
ping -c 4 8.8.8.8
```

- **تحديد حجم الحزمة:**
```bash
ping -s 64 8.8.8.8
```

- **تحديد الفاصل الزمني بين الحزم:**
```bash
ping -i 2 8.8.8.8
```

## Tips
- استخدم الخيار `-c` لتحديد عدد الحزم المرسلة لتجنب إرسال الحزم بشكل غير محدود.
- تحقق من استجابة الشبكة باستخدام `ping` قبل محاولة الاتصال بخدمات أخرى.
- يمكنك استخدام `ping` مع أسماء النطاقات بدلاً من عناوين IP، مثل `ping google.com`.