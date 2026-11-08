Shine Chen — portfolio site
===========================

Files
  index.html          the whole site (both languages, all interactions, no build step)
  Shine_Chen_CV.pdf   linked from the "Download CV" buttons — keep it next to index.html

Hosting (any of these works; all are free)
  Netlify Drop   https://app.netlify.com/drop  — drag this folder onto the page, done.
  GitHub Pages   new repo → upload both files → Settings → Pages → deploy from main.
  Cloudflare Pages / Vercel — same idea: upload the folder.
  Your own domain: point it at whichever of the above you used.

Notes
  - Default language follows the visitor's browser (Chinese browsers get 中文); the
    toggle in the nav overrides it and is remembered. ?lang=zh or ?lang=en in the URL
    forces a language, e.g. for a link in a Chinese email.
  - Fonts load from Google Fonts (Inter + Noto Sans TC). If you'd rather have zero
    external requests, delete the <link ... fonts.googleapis.com ...> line in index.html;
    the page falls back to the system font.
  - To change copy: open index.html, find "var COPY = {" — all text for both languages
    lives there, en: and zh:, in reading order.
