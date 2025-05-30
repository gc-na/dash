# [ডেবিয়ান] Debian Almquist Shell (dash) du ব্যবহার: ফাইল সাইজ পরিমাপ করা

## Overview
`du` কমান্ডটি Unix-ভিত্তিক অপারেটিং সিস্টেমে ব্যবহৃত হয়, যা ফাইল এবং ডিরেক্টরির ডিস্ক ব্যবহারের পরিমাণ পরিমাপ করে। এটি ব্যবহারকারীদের তাদের সিস্টেমে স্থান খরচের বিশ্লেষণ করতে সাহায্য করে।

## Usage
`du` কমান্ডের মৌলিক সিনট্যাক্স হলো:

```bash
du [options] [arguments]
```

## Common Options
- `-h`: মানব-পঠনযোগ্য ফরম্যাটে আউটপুট দেখায় (যেমন KB, MB)।
- `-s`: শুধুমাত্র সারসংক্ষেপ আউটপুট করে, অর্থাৎ নির্দিষ্ট ডিরেক্টরির মোট সাইজ দেখায়।
- `-a`: সমস্ত ফাইল এবং ডিরেক্টরির সাইজ দেখায়, ডিরেক্টরি ছাড়া।
- `-c`: মোট সাইজের একটি সারসংক্ষেপ যোগ করে।

## Common Examples
1. একটি ডিরেক্টরির সাইজ দেখানোর জন্য:
   ```bash
   du -h /path/to/directory
   ```

2. শুধুমাত্র একটি ডিরেক্টরির মোট সাইজ দেখানোর জন্য:
   ```bash
   du -sh /path/to/directory
   ```

3. সমস্ত ফাইল এবং ডিরেক্টরির সাইজ দেখানোর জন্য:
   ```bash
   du -ah /path/to/directory
   ```

4. একাধিক ডিরেক্টরির মোট সাইজ দেখানোর জন্য:
   ```bash
   du -sh /path/to/directory1 /path/to/directory2
   ```

5. মোট সাইজের সারসংক্ষেপ সহ:
   ```bash
   du -ch /path/to/directory
   ```

## Tips
- `du` কমান্ডটি ব্যবহার করার সময়, `-h` অপশনটি ব্যবহার করা সর্বদা ভাল, কারণ এটি আউটপুটকে আরও সহজে বোঝার যোগ্য করে।
- যদি আপনি একটি বৃহৎ ডিরেক্টরির সাইজ বিশ্লেষণ করতে চান, তবে `-s` অপশনটি ব্যবহার করুন যাতে আপনি দ্রুত সারসংক্ষেপ পেতে পারেন।
- `du` কমান্ডের আউটপুটকে `sort` কমান্ডের সাথে যুক্ত করে সাইজ অনুযায়ী সাজানো যেতে পারে:
  ```bash
  du -h /path/to/directory | sort -h
  ```