# [ديبيان] Debian Almquist Shell (dash) time: قياس الوقت المستغرق لتنفيذ الأوامر

## نظرة عامة
أمر `time` في شل داش يُستخدم لقياس الوقت المستغرق لتنفيذ الأوامر. يوفر معلومات حول الوقت المستخدم في التنفيذ، بما في ذلك الوقت الحقيقي، ووقت المعالجة في المستخدم، ووقت المعالجة في النظام.

## الاستخدام
الصيغة الأساسية للأمر هي:

```bash
time [options] [arguments]
```

## الخيارات الشائعة
- `-p`: استخدام تنسيق POSIX للإخراج.
- `-o FILE`: كتابة الإخراج إلى ملف محدد بدلاً من الشاشة.
- `-v`: عرض معلومات مفصلة حول عملية التنفيذ.

## أمثلة شائعة
- قياس الوقت المستغرق لتنفيذ أمر `ls`:

```bash
time ls
```

- قياس الوقت المستغرق لتنفيذ سكربت:

```bash
time ./myscript.sh
```

- كتابة الإخراج إلى ملف:

```bash
time -o output.txt ls
```

- استخدام الخيار `-v` للحصول على معلومات مفصلة:

```bash
time -v ls
```

## نصائح
- استخدم الخيار `-o` لتخزين النتائج في ملف إذا كنت بحاجة إلى مراجعتها لاحقًا.
- جرب استخدام `time` مع أوامر طويلة أو معقدة للحصول على فكرة عن الأداء.
- استخدم الخيار `-p` للحصول على تنسيق إخراج بسيط وسهل القراءة.