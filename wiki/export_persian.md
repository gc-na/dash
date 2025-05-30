# [دبیان] Debian Almquist Shell (dash) export استفاده: متغیرهای محیطی را تنظیم می‌کند

## Overview
دستور `export` در شل دبیان آلمکوئیست (dash) برای تعیین متغیرهای محیطی استفاده می‌شود. با استفاده از این دستور، می‌توانید متغیرهایی را تعریف کنید که در تمام زیرشِل‌ها و فرآیندهای فرزند قابل دسترسی باشند.

## Usage
سینتکس پایه دستور `export` به صورت زیر است:

```sh
export [options] [arguments]
```

## Common Options
- `-n`: این گزینه متغیر را از لیست متغیرهای صادر شده حذف می‌کند.
- `-p`: این گزینه لیست متغیرهای صادر شده را نمایش می‌دهد.

## Common Examples
### مثال ۱: صادر کردن یک متغیر
برای صادر کردن یک متغیر به نام `MY_VAR`، می‌توانید از دستور زیر استفاده کنید:

```sh
MY_VAR="Hello, World!" 
export MY_VAR
```

### مثال ۲: صادر کردن چندین متغیر
شما می‌توانید چندین متغیر را به صورت همزمان صادر کنید:

```sh
export VAR1="Value1" VAR2="Value2"
```

### مثال ۳: نمایش متغیرهای صادر شده
برای نمایش متغیرهای صادر شده، می‌توانید از گزینه `-p` استفاده کنید:

```sh
export -p
```

### مثال ۴: حذف یک متغیر صادر شده
برای حذف یک متغیر از لیست متغیرهای صادر شده، از گزینه `-n` استفاده کنید:

```sh
export -n MY_VAR
```

## Tips
- همیشه قبل از استفاده از متغیرهای صادر شده، مطمئن شوید که آنها به درستی تعریف شده‌اند.
- برای جلوگیری از تداخل نام متغیرها، از نام‌های منحصر به فرد استفاده کنید.
- می‌توانید متغیرهای صادر شده را در فایل‌های اسکریپت ذخیره کنید تا در زمان‌های بعدی به راحتی از آنها استفاده کنید.