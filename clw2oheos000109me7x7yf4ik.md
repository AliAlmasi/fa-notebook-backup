---
title: "رفع خطای کارت وای‌فای Rtl8821ce در لینوکس دبیان/اوبونتو (و سایر توزیع‌های مبتنی بر دبیان/اوبونتو)"
seoTitle: "رفع خطای کارت وای‌فای RTL8821CE در لینوکس"
seoDescription: "رفع خطای کارت وای‌فای RTL8821CE در لینوکس دبیان/اوبونتو (و سایر توزیع‌های مبتنی بر دبیان/اوبونتو) "
datePublished: Sat May 11 2024 22:28:56 GMT+0000 (Coordinated Universal Time)
cuid: clw2oheos000109me7x7yf4ik
slug: rtl8821ce-wireless-card-fix-on-ubuntu
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1715466403812/212049da-3fd4-4bb1-9e4f-c6e30f1cc2d2.avif
tags: ubuntu, linux, debian, foss, wireless-network, persian

---

### [English version link is here](https://note.al1almasi.ir/rtl8821ce-wireless-card-fix-on-ubuntu)

به دلایلی، سخت افزار وای‌فای rtl8821ce در اکثر توزیع های لینوکس ضعیف عمل می کند یا اصلاً کار نمی کند. درایور استفاده شده در هسته لینوکس برای این سخت افزار قدیمی است یا به دلایل دیگری که من نمی دانم درست کار نمی کند. راه حل این مشکل درایوری است که توسط [یکی از دوستان پرتغالی](https://github.com/tomaspinho) توسعه یافته و در GitHub قرار داده شده است.

**در این راهنما، ما می‌خواهیم این درایور را روی اوبونتو خود بسازیم و نصب کنیم.**

> هشدار: قبل از ادامه، یک snapshot از سیستم خود برای احتیاط بگیرید.

یک ترمینال را باز کنید و دنبال کنید:

1. APT خود را به روز کنید: `sudo apt update`
    
2. ابزارهای لازم را نصب کنید: `sudo apt install bc module-assistant build-essential dkms git`
    
3. را حذف کنید `rtl8821ce-dkms`در صورت وجود: `sudo apt remove rtl8821ce-dkms`
    
4. درایور را از گیتهاب دریافت کنید و وارد دایرکتوری دریافت شده شوید: `git clone` [`https://github.com/tomaspinho/rtl8821ce.git`](https://github.com/tomaspinho/rtl8821ce.git) `&& cd rtl8821ce`
    
5. آماده کردن/ساخت درایور: `sudo m-a prepare`
    
6. اگر خروجی `Couldn't create the /usr/src/linux symlink!` بود، دوباره امتحان کنید.
    
7. درایور را نصب کنید: `sudo ./`[`dkms-install.sh`](http://dkms-install.sh)
    
8. یک ترمینال جدید باز کنید و این دستور را اجرا کنید: `sudo nano /etc/modprobe.d/blacklist.conf`
    
9. اضافه کردن `blacklist rtw88_8821ce` تا انتها و فایل را ذخیره کنید
    
10. ریبوت سیستم و ... تمام!