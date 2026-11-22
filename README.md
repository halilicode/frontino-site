<div align="center">

# Frontino — Frontend Education

**A free, interactive front-end course with a built-in live code editor.**
HTML · CSS · JavaScript · React — in English and Persian.

[**Live demo**](https://YOUR_USERNAME.github.io/frontino/) · [Report a bug](https://github.com/YOUR_USERNAME/frontino/issues) · [فارسی](#-فرانتینو)

![License](https://img.shields.io/badge/license-MIT-blue)
![No build step](https://img.shields.io/badge/build-none-brightgreen)
![Languages](https://img.shields.io/badge/languages-EN%20%7C%20FA-orange)

</div>

<!-- Add a screenshot or GIF here, e.g. ![Frontino](docs/screenshot.png) -->

## Features

- **Live code editor** — edit and run HTML, CSS, JavaScript and React right on the page, with syntax highlighting, line numbers, bracket and tag auto-close, a problems panel (unclosed tags, stray text, CSS brace errors, JS/React runtime and syntax errors) and optional auto-run.
- **309 lessons in 4 tracks** — HTML (85), CSS (122), JavaScript (49) and React (53), each with a runnable example.
- **Bilingual** — English (default) and Persian with a proper right-to-left layout. Choice is remembered.
- **Quizzes and progress** — 3-question quizzes with *Next*, per-track progress bars, "mark as complete", and a completion certificate preview.
- **Scroll-driven landing page** — parallax hero, infinite marquee, a laptop/tablet/phone mockup that opens as you scroll, sticky "how it works" story, bento feature grid, sideways-scrolling gallery, count-up stats, and a scroll progress bar. All artwork is inline SVG/CSS (no image files).
- **4 themes** — Black (default), Aurora, Cyber and Light, switchable from the palette button; choice is remembered.
- **Interactive UI** — particle network, cursor comet trail and spotlight grid that follow the mouse, mouse-parallax layers, 3D-tilting cards with glare, magnetic buttons, cursor labels, click sparks. All motion respects `prefers-reduced-motion`; custom cursor effects are off on touch devices.
- **Responsive** — phones, tablets and desktops (Windows, macOS, Linux): off-canvas lesson menu on small screens, stacked editor on tablets, larger touch targets and 16px editor text on touch devices (avoids iOS zoom), wider layout on big monitors.
- **Private** — no accounts, no analytics. Progress is stored only in `localStorage`.
- **Zero build** — the whole site is one `index.html`.

## Content coverage

| Track | Lessons |
|---|---|
| HTML | 85 |
| CSS | 122 |
| JavaScript | 49 |
| React | 53 |

Persian translations exist for lesson text and menu titles of every written lesson. Code examples are in English.

## Quick start

```bash
git clone https://github.com/YOUR_USERNAME/frontino.git
cd frontino
# open index.html in a browser, or serve it locally:
python3 -m http.server 8080
```

## Deploy on GitHub Pages

1. Push the repo to GitHub.
2. **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Choose `main` and `/ (root)`, then save.
4. Your site appears at `https://YOUR_USERNAME.github.io/frontino/`.

Optional: open `index.html`, find `const GH="";` and set it to your repo URL to show a **★ GitHub** button in the footer.

## How it works

- Single-page app in vanilla HTML, CSS and JavaScript. Routes use the URL hash (`#html-3`).
- Lessons are plain data. Helper functions register a title, Persian title, English text, Persian text and example code, for example:

  ```js
  C("CSS Variables", "متغیرها", "English explanation.", "توضیح فارسی.", '<style>…</style>');
  ```

  Helpers: `H` (HTML), `C` (CSS), `J` (JavaScript), `R` (React). Menus live in the `MENU` object.
- The editor is a transparent `<textarea>` over a syntax-highlighted `<pre>`. Code runs in a sandboxed `<iframe srcdoc>`; errors are sent back with `postMessage`.
- React lessons load React 18 and Babel Standalone from **cdnjs** inside the sandbox. Fonts load from **Google Fonts**. Nothing else leaves the browser.

## Editor shortcuts

| Key | Action |
|---|---|
| `Ctrl/Cmd + Enter` | Run |
| `Tab` | Insert two spaces |
| `Enter` | Keep indentation |

## Browser support

Current Chrome, Edge, Firefox and Safari. Uses `color-mix()`, `:is()` and CSS `inset`; older browsers fall back to plainer styling.

## Roadmap

- [ ] One page per lesson for better SEO
- [ ] Longer explanations for the shorter lessons
- [ ] More quizzes (JavaScript, forms, Flexbox)
- [ ] Search across all lessons

## Contributing

Issues and pull requests are welcome. For a new lesson, add one helper call to the matching track and include both languages.

## License

[MIT](LICENSE) — the Frontino name and logo remain the property of the Frontino team.

---

# 🇮🇷 فرانتینو

**فرانتینو** یک دورهٔ رایگان و تعاملی فرانت‌اند با ویرایشگر زندهٔ کد است: HTML، CSS، جاوااسکریپت و React، به دو زبان فارسی و انگلیسی.

- ویرایشگر زنده با رنگ‌آمیزی کد، شمارهٔ خط، بستن خودکار تگ و پرانتز و نمایش خطا
- ۳۰۹ درس در ۴ مسیر، هر درس با مثال قابل‌اجرا
- آزمون، پیگیری پیشرفت و گواهی پایان دوره
- تم تیره (پیش‌فرض) و روشن، با انیمیشن‌های تعاملی همراه موس
- بدون ثبت‌نام و بدون آنالیتیکس؛ پیشرفت فقط در مرورگر خود کاربر ذخیره می‌شود
- کل سایت یک فایل `index.html` است؛ بدون نیاز به بیلد

برای اجرا فایل `index.html` را باز کنید یا با GitHub Pages منتشر کنید (مراحل بالا).
