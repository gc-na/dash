# [دبیان] Debian Almquist Shell (dash) rm استفاده: حذف فایل‌ها و دایرکتوری‌ها

## Overview
دستور `rm` در شل دبیان آلمکوئیست (dash) برای حذف فایل‌ها و دایرکتوری‌ها استفاده می‌شود. این دستور به شما این امکان را می‌دهد که فایل‌ها را به‌طور دائمی از سیستم خود حذف کنید.

## Usage
سینتکس پایه دستور `rm` به صورت زیر است:

```bash
rm [options] [arguments]
```

## Common Options
- `-f`: حذف فایل‌ها بدون درخواست تأیید.
- `-i`: قبل از حذف هر فایل، از کاربر تأیید می‌خواهد.
- `-r`: حذف دایرکتوری‌ها و محتوای آن‌ها به‌صورت بازگشتی.
- `-v`: نمایش نام فایل‌هایی که در حال حذف هستند.

## Common Examples
- حذف یک فایل:
  ```bash
  rm myfile.txt
  ```

- حذف چند فایل:
  ```bash
  rm file1.txt file2.txt file3.txt
  ```

- حذف یک دایرکتوری و محتوای آن به‌صورت بازگشتی:
  ```bash
  rm -r mydirectory
  ```

- حذف یک فایل با تأیید:
  ```bash
  rm -i myfile.txt
  ```

- حذف فایل‌ها با نمایش نام آن‌ها:
  ```bash
  rm -v file1.txt file2.txt
  ```

## Tips
- همیشه قبل از استفاده از `rm` با گزینه `-f`، اطمینان حاصل کنید که فایل‌های مورد نظر را به‌درستی شناسایی کرده‌اید.
- برای جلوگیری از حذف تصادفی، می‌توانید از گزینه `-i` استفاده کنید.
- اگر می‌خواهید دایرکتوری‌ها را حذف کنید، حتماً از گزینه `-r` استفاده کنید.