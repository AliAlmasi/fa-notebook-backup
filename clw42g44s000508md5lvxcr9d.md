---
title: "نحوه استفاده از مجموعه V2ray تلگرام YeBeKhe"
datePublished: Sun May 12 2024 21:47:36 GMT+0000 (Coordinated Universal Time)
cuid: clw42g44s000508md5lvxcr9d
slug: telegram-v2ray-collector
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1715548896498/ace26efb-b00b-4ca5-b49b-fa5e26ada7d3.avif
tags: opensource, internet, telegram, xray, v2ray, persian, filternet, hiddify, internet-censorship

---

این پروژه همانطور که از نامش مشخص است، کانفیگ های V2ray را از بیش از 70 کانال تلگرام جمع آوری می کند. این پروژه می تواند به مردم ایران کمک کند تا سانسور و فیلترینگ اینترنت را دور بزنند.

[TelegramV2rayCollector](https://github.com/yebekhe/TelegramV2rayCollector) در بستر GitHub ارائه می شود.

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698686343248/cdbebe76-57e6-42e2-a87b-59a30b8be78f.png?auto=compress,format&format=webp align="left")](https://github.com/yebekhe/TelegramV2rayCollector)

این پروژه هر ساعت به روز می شود، بنابراین افراد می توانند از تنظیمات "تازه" استفاده کنند و سانسور را راحت تر دور بزنند. شما می توانید با افزودن لینک اشتراک آن به برنامه کلاینت V2ray/Xray از این پروژه استفاده کنید و هر ساعت آن را به روز کنید.

من قصد دارم از [***Hiddify Next***](https://github.com/hiddify/hiddify-next) استفاده کنم تا به شما نشان دهم چگونه می توانید از TelegramV2rayCollector استفاده کنید. *Hiddify Next* برای نصب در دستگاه‌های Windows، Linux و Android در دسترس است (همچنین در Google Play و Microsoft Store موجود است).

ابتدا این برنامه را نصب کنید تا بتوانید از لینک ساب‌ها استفاده کنید. می توانید *Hiddify Next* را روی هر سیستم عامل دسکتاپ نصب کنید (همچنین [در AUR](https://aur.archlinux.org/packages/hiddify-next-bin) برای کاربران Arch Linux موجود است). اگر برای نصب آن به راهنمایی نیاز دارید، می توانید [به وب سایت آنها مراجعه کنید](https://hiddify.com/app/).

شما می توانید هر برنامه کلاینت V2ray/Xray را که دوست دارید نصب و استفاده کنید (مثلا v2rayN در ویندوز یا v2rayNG در اندروید از دیگر برنامه‌های مناسب و منبع باز هستند)، زیرا همه آنها از یک [هسته V2ray](https://github.com/v2ray/v2ray-core) / [Xray](https://github.com/XTLS/Xray-core) استفاده می کنند.

پس از راه اندازی برنامه، پیوند اشتراک را از فایل readme در مخزن GitHub آنها کپی می کنیم.

![همانطور که می بینید، لینک اشتراک برای اکثر هسته های پراکسی محبوب مانند Xray، Singbox، Clash و Surfboard وجود دارد.](https://cdn.hashnode.com/res/hashnode/image/upload/v1715509127290/a0e045af-a8be-4eb0-bf4e-972911f839f4.png?auto=compress,format&format=webp align="left")

همانطور که می بینید، لینک ساب برای اکثر هسته های پراکسی محبوب مانند Xray، Singbox، Clash و Surfboard وجود دارد.

> لینک ساب‌های "Donate" برای کانفیگ هایی است که به پروژه اهدا شده اند. آنها در لینک‌ ساب‌های "Group Mix" قرار داده شده اند، بنابراین شما فقط می توانید لینک‌های "Group Mix" را کپی کنید.

![همچنین پیوندهای اشتراک متفاوتی برای انواع مختلف پروکسی ها مانند Vless، Vmess، Reality، Trojan، Shadowsocks، Tuic و Hysteria وجود دارد.](https://cdn.hashnode.com/res/hashnode/image/upload/v1715509249252/1f721988-496e-4e34-aed9-7724c6f456fe.png?auto=compress,format&format=webp align="left")

همچنین لینک‌های ساب متفاوت برای انواع مختلف پروکسی‌ها مانند Vless، Vmess، Reality، Trojan، Shadowsocks، Tuic و Hysteria در انواع مختلف هسته‌های پروکسی وجود دارد. اما ما در مورد انواع پروکسی ها حساس نیستیم، بنابراین از لینک‌های ساب ترکیبی استفاده می کنیم (آنهایی که در تصویر قبلی نمایش داده شدند - *"Group Mix Link"*).

من *Hiddify Next* را که از هسته Xray استفاده می‌کند، راه‌اندازی کرده‌ام. بنابراین باید پیوندهای اشتراک Xray را کپی کنیم. می توانید از اشتراک خام یا ساب *Base64* استفاده کنید.

تفاوت بین ساب خام *(متن ساده)* و ساب *Base64* [در این است که وقتی لینک ساب خام](https://raw.githubusercontent.com/yebekhe/TelegramV2rayCollector/main/sub/normal/mix) را باز می‌کنید، می‌توانید اطلاعاتی را که پیوند موجود است ببینید، اما اطلاعات لینک ساب *Base64* کدگذاری شده است. *Base64* ممکن است در شبکه‌هایی که ترافیک دائماً بررسی و شنود می‌شود، مفید باشد.

من شخصاً از ساب *Base64* استفاده می کنم، بنابراین لینک با عنوان **Xray (Base64)Group Mix** را کپی می کنیم**.** *(می توانید لینک را با کلیک راست روی* [*اینجا*](https://raw.githubusercontent.com/yebekhe/TelegramV2rayCollector/main/sub/base64/mix) *و بعد "Copy link" کپی کنید)*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1715513142406/e163392a-3c11-4334-9771-6c7da13ddafc.png?auto=compress,format&format=webp align="left")

---

پس از کپی کردن لینک ساب، باید آن را به برنامه وارد کنیم. در *Hiddify Next* به راحتی این عمل انجام میشود. فقط برنامه را شروع کرده و روی "نمایه جدید" در صفحه "خانه" کلیک کنید.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1715549972347/4c20dfec-3e1c-4df7-bf9c-71d619b4cae7.png align="center")

سپس "افزودن از کلیپ بورد" را انتخاب می کنید و سپس منتظر می مانید تا برنامه لینکی که کپی کرده اید را بخواند و وارد کند. در پایان، چنین چیزی را باید مشاهده کنید.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1715550026780/30f6b735-7c26-4f02-8785-3cbd3cf1ae4d.png align="center")

اکنون می توانید به راحتی از این سرویس استفاده کنید و هر زمان که بخواهید کانفیگ های V2ray "تازه" داشته باشید تا بتوانید راحت تر سانسور را دور بزنید. به‌روزرسانی کانفیگ‌ها نیز بسیار آسان است. شما فقط روی این دکمه در اینجا کلیک کنید و سپس کانفیگ‌های جدیدی خواهید داشت. به یاد داشته باشید، این سرویس هر ساعت به روز می شود.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1715550175074/82b2fe18-cc32-4946-b254-5d09034b746f.png align="center")

---

دستورالعمل های نسخه اندروید *Hiddify Next* نیز مانند نسخه دسکتاپ است، زیرا هر دو دارای ظاهر یکسان هستند.

*اگر در* مورد *Hiddify Next* سؤالی دارید، می‌توانید در [بخش بحث مخزن GitHub](https://github.com/hiddify/hiddify-next/discussions) بپرسید. اگر مشکلی یا باگی در برنامه پیدا کردید، می‌توانید با ثبت یک issue در [بخش مشکلات مخزن GitHub](https://github.com/hiddify/hiddify-next/issues) را به تیم توسعه هیدیفای اطلاع دهید.