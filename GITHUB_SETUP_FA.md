# راهنمای گذاشتن فرانتینو روی GitHub (به‌عنوان نمونه‌کار)

## ۱) ساخت ریپو
- در GitHub روی **New repository** بزن.
- نام پیشنهادی: `frontino`
- Description (کپی کن):
  `Free interactive front-end course with a live code editor — HTML, CSS, JavaScript & React in English and Persian.`
- Public را انتخاب کن. تیک «Add a README» را **نزن** (README آماده است).

## ۲) آپلود فایل‌ها
از پوشهٔ همین بسته این فایل‌ها را آپلود کن: `index.html`، `README.md`، `LICENSE` و `.nojekyll`.
- روش ساده: در صفحهٔ ریپو **Add file → Upload files**، فایل‌ها را بکش و **Commit changes** بزن.
- روش گیت:
```bash
git init
git add .
git commit -m "feat: Frontino v1.0 - bilingual front-end course with live editor"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/frontino.git
git push -u origin main
```

## ۳) فعال‌سازی سایت (GitHub Pages)
**Settings → Pages → Deploy from a branch → main / (root) → Save.**
بعد از ۱ تا ۲ دقیقه آدرس سایت این است: `https://YOUR_USERNAME.github.io/frontino/`

## ۴) جایگزین کردن YOUR_USERNAME
در `README.md` همهٔ `YOUR_USERNAME` را با نام کاربری خودت عوض کن.
اختیاری: در `index.html` عبارت `const GH="";` را پیدا کن و آدرس ریپو را بین گیومه‌ها بگذار تا دکمهٔ «★ GitHub» پایین سایت دیده شود.

## ۵) تنظیمات صفحهٔ ریپو
- بالا سمت راست (About) → Description را بگذار و آدرس سایت را در Website وارد کن.
- Topics پیشنهادی:
  `html` `css` `javascript` `react` `education` `tutorial` `live-editor` `learn-to-code` `frontend` `persian` `farsi` `rtl` `github-pages`
- **Settings → General → Social preview**: یک تصویر ۱۲۸۰×۶۴۰ بگذار (اسکرین‌شات صفحهٔ اصلی با لوگو).
- ریپو را در پروفایلت **Pin** کن.

## ۶) چیزهایی که باعث دیده شدن می‌شود (راه‌های درست)
- یک اسکرین‌شات یا GIF کوتاه از ویرایشگر و انیمیشن موس در ابتدای README بگذار؛ مهم‌ترین عامل است.
- یک **Release** با عنوان `v1.0` بساز و تغییرات را بنویس.
- لینک را در کانال تلگرام، لینکدین، ویرگول، Dev.to و Reddit (مثلاً r/webdev، روزهای Showoff) به اشتراک بگذار و از بقیه بازخورد بخواه.
- چند Issue با برچسب `good first issue` باز کن تا دیگران مشارکت کنند.
- ستاره یا بازدید **نخر**؛ GitHub حساب‌های متقلب را حذف می‌کند و به اعتبار نمونه‌کارت ضرر می‌زند.

## ۷) قبل از انتشار
- چند درس از هر مسیر را بخوان و اگر نکته‌ای را اصلاح کردی همان‌جا در `index.html` بنویس. برای نمونه‌کار، دقت محتوا مهم است.
- همهٔ مثال‌ها را یک بار در مرورگر اجرا کن و اگر مورد خراب دیدی ریپو را Issue بزن یا درستش کن.
