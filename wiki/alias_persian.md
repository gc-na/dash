# [دبیان] Debian Almquist Shell (dash) alias: ایجاد نام‌های مستعار برای دستورات

## Overview
دستور `alias` در شل دبیان آلمکوئیست (dash) به شما این امکان را می‌دهد که نام‌های مستعار برای دستورات طولانی یا پیچیده ایجاد کنید. این کار باعث می‌شود که استفاده از این دستورات ساده‌تر و سریع‌تر شود.

## Usage
سینتکس پایه دستور `alias` به شکل زیر است:

```bash
alias [options] [arguments]
```

## Common Options
- `-p`: نمایش تمام نام‌های مستعار تعریف‌شده در حال حاضر.
- `name=value`: ایجاد یا تغییر یک نام مستعار. 

## Common Examples
در اینجا چند مثال عملی از استفاده از دستور `alias` آورده شده است:

1. ایجاد یک نام مستعار برای دستور `ls -la`:
   ```bash
   alias ll='ls -la'
   ```

2. ایجاد یک نام مستعار برای پاک کردن صفحه نمایش:
   ```bash
   alias cls='clear'
   ```

3. نمایش تمام نام‌های مستعار موجود:
   ```bash
   alias -p
   ```

4. تغییر یک نام مستعار موجود:
   ```bash
   alias ll='ls -l --color=auto'
   ```

## Tips
- برای حفظ نام‌های مستعار خود، می‌توانید آن‌ها را در فایل `~/.bashrc` یا `~/.profile` اضافه کنید.
- از نام‌های مستعار کوتاه و معنادار استفاده کنید تا به راحتی به خاطر سپرده شوند.
- برای بررسی نام‌های مستعار موجود، از دستور `alias` بدون هیچ آرگومانی استفاده کنید.