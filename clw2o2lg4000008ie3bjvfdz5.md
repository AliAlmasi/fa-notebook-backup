---
title: "ساخت آسان کانفیگ وی‌لس با ورکر کلاودفلر"
seoTitle: "ساخت آسان کانفیگ وی‌لس با ورکر کلاودفلر"
datePublished: Sat May 11 2024 22:17:25 GMT+0000 (Coordinated Universal Time)
cuid: clw2o2lg4000008ie3bjvfdz5
slug: easy-vless-config-with-cf-worker
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1715465025529/d553e396-cbb5-488d-9a46-4c78c8f41bb9.avif
tags: cloudflare, websockets, iran, persian, cloudflare-worker, filternet

---

### [English Version of this article is here.](https://note.al1almasi.ir/easy-vless-config-with-cf-worker)

این بسیار آسان است (شما به هیچ سروری نیاز ندارید). فقط یک ورکر کلاودفلر ایجاد کنید و سپس تمام [محتوای فایل worker.js](https://raw.githubusercontent.com/AliAlmasi/vless-cf-worker/main/worker.js) را به عنوان اسکریپت ورکر کپی و paste کنید، سپس همه این کارها را انجام دهید:

1. یک [UUID](https://fa.wikipedia.org/wiki/%D8%B4%D9%86%D8%A7%D8%B3%D9%87_%D9%85%D9%86%D8%AD%D8%B5%D8%B1%D8%A8%D9%87%E2%80%8C%D9%81%D8%B1%D8%AF_%D8%AC%D9%87%D8%A7%D9%86%DB%8C) ایجاد کنید و پس از چسباندن آن، آن را در پیکربندی کارگر جایگزین کنید ( [خط 201](https://github.com/AliAlmasi/vless-cf-worker/blob/main/worker.js#L201) )
    
2. ورکر خود را ذخیره و deploy کنید.
    
3. اختیاری: اگر دامنه ای در کلاودفلر خود دارید، یک دامنه سفارشی برای ورکر خود اضافه کنید.
    
4. روی هر برنامه وی‌توری/ایکس‌ری که استفاده می کنید یک پیکربندی وی‌لس ایجاد کنید (شخصا [v2rayN](https://github.com/2dust/v2rayN)
    
5. روی ویندوز و [v2rayng](https://github.com/2dust/v2rayNG) روی اندروید را ترجیح می دهم)
    
6. گزینه TLS را **TLS** مقداردهی کنید و دامنه ورکر خود را به عنوان SNI تنظیم کنید.
    
7. گزینه transport را روی **ws** تنظیم کنید .
    
8. دامنه ورکر خود را به عنوان میزبان ws تنظیم کنید.
    
9. هر *آی‌پی کلاودفلر تمیزی* که دارید را به عنوان آدرس مقصد تنظیم کنید. می توانید از [IRCF.space](http://IRCF.space) استفاده کنید. *(بروزرسانی: دامنه های ircf.space در ایران فیلتر شده)*
    
10. پورت را **443** تنظیم کنید.
    
11. و در نهایت، UUID تولید شده خود را به عنوان UUID کافیگ‌تون تنظیم کنید.
    

اکنون همه چیز تمام شده است. کانفیگ وی‌لس خود را تست کنید.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1715465608139/215ef837-d596-48ec-ac4d-592a39125e71.jpeg align="center")