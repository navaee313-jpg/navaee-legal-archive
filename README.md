<p align="center">
  <img src="assets/logo-emblem.png" width="140" alt="Mohammad Navaee Attorney logo">
</p>

<h1 align="center">بایگانی حقوقی نوائی</h1>
<p align="center">سامانه آفلاین ثبت و مدیریت پرونده‌های موکلین دفتر وکالت</p>

---

## درباره پروژه

یک اپ تک‌فایلی (Single-file PWA) برای مدیریت روزمره دفتر وکالت — کاملاً آفلاین و بدون نیاز به سرور یا بک‌اند. تمام داده‌ها با `localStorage` روی همان مرورگر/دستگاه ذخیره می‌شوند.

### امکانات

- 👤 مدیریت موکلین
- 📁 مدیریت پرونده‌ها (مرتبط با موکل)
- ⏰ مواعید و یادآوری‌ها
- 🗓 تقویم جلالی
- 💰 مدیریت مالی (درآمد/هزینه و مانده)
- 📄 اسناد و مدارک (آپلود تا ۱.۵ مگابایت هر فایل)
- 🔍 جستجوی سراسری/پیشرفته
- ⚙️ تنظیمات، پشتیبان‌گیری/بازیابی JSON، پاک‌سازی کامل داده‌ها
- 📲 قابل نصب به‌صورت PWA (زمانی که روی HTTPS میزبانی شود)

<p align="center">
  <img src="assets/screenshot-dashboard.png" width="700" alt="داشبورد">
</p>
<p align="center">
  <img src="assets/screenshot-add-client.png" width="700" alt="ثبت موکل جدید">
</p>

## استفاده

فقط فایل `index.html` را در مرورگر باز کنید — نیازی به نصب یا سرور نیست.

برای نصب PWA (آیکن روی صفحه اصلی، اجرای آفلاین کامل)، پروژه باید روی یک آدرس HTTPS میزبانی شود (مثلاً GitHub Pages).

### راه‌اندازی روی GitHub Pages

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <آدرس ریپازیتوری شما>
git push -u origin main
```

سپس در تنظیمات ریپازیتوری، بخش **Settings → Pages** را باز کرده و شاخه `main` را به‌عنوان منبع انتخاب کنید.

## ساختار پروژه

```
├── index.html              # کل اپلیکیشن (HTML+CSS+JS)
├── manifest.json            # مشخصات PWA
├── sw.js                     # service worker (کش آفلاین)
├── favicon.ico
├── icon-16.png / icon-32.png / icon-192.png / icon-512.png
├── icon-512-maskable.png
├── apple-touch-icon.png
└── assets/                   # لوگوها و اسکرین‌شات‌ها (فقط مستندات)
```

## نکته درباره داده‌ها

داده‌ها فقط در مرورگر همان دستگاه ذخیره می‌شوند. به‌صورت دوره‌ای از بخش تنظیمات، پشتیبان‌گیری (Export) بگیرید.

---
<p align="center">محمد نوائی — وکیل دادگستری</p>
