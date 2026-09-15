نسخه آماده Firebase برای «دختر بغلیم» ❤️

این نسخه طوری تنظیم شده که برای چت و گنجینه به Storage نیاز نداشته باشد؛ بنابراین روی Spark و بدون وارد کردن کشور/کارت بانکی هم قابل استفاده است.
عکس گنج‌ها قبل از ذخیره در مرورگر فشرده می‌شوند و داخل Firestore ذخیره می‌شوند (حداکثر حدود 600KB فایل فشرده).

تنظیمات Firebase:
1. Authentication > Sign-in method > Anonymous باید Enabled باشد.
2. Firestore Database > Rules: محتوای firestore.rules این بسته را جایگزین کن و Publish بزن.
3. Storage را فعلاً لازم نیست راه‌اندازی کنی.
4. firebase-config.js از قبل با پروژه فعلی تنظیم شده است.

انتشار:
فایل‌های این بسته را در GitHub Pages یا هاست خودت قرار بده:
index.html
chat.html
treasure.html
firebase-config.js
firestore.rules
storage.rules
.nojekyll

بعد از انتشار، دامنه سایت را در Authentication > Settings > Authorized domains اضافه کن.

تست:
- chat.html را باز کن و دو مرورگر/دستگاه را امتحان کن.
- treasure.html را باز کن و یک گنج Shared با عکس کوچک اضافه کن.
- از مرورگر دیگر همان گنج را ببین.
- یک گنج Private بساز و مطمئن شو فقط سازنده آن را می‌بیند.
- برای گنج قفل‌شده تاریخ آینده بگذار.

نکته: کلید apiKey در Firebase config برای اپ وب شناسه عمومی است؛ امنیت اصلی با Authentication و Firestore Rules انجام می‌شود.
