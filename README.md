# TikTok 4K Uploader

## طريقة الرفع على Render.com (مجاني)

1. ارفع محتويات هذا الملف على GitHub repo (private)
2. اذهب https://render.com → New → Web Service
3. اربط الـ GitHub repo
4. الإعدادات:
   - Build Command: `npm install`
   - Start Command: `npm start`
5. أضف Environment Variables:
   - `PORT` = `10000`
   - `ADMIN_PASSWORD` = كلمة سر الأدمن
   - `SESSION_SECRET` = أي نص عشوائي طويل
   - `NODE_ENV` = `production`
6. بعد الرفع: Settings → Custom Domain → أضف `tiktokupload.indevs.in`

## إعداد الدومين

أضف هذا الـ DNS record عند مزود دومينك:

| Type  | Name         | Value                      |
|-------|--------------|----------------------------|
| CNAME | tiktokupload | your-app-name.onrender.com |

## لوحة الأدمن

https://tiktokupload.indevs.in/admin/login
