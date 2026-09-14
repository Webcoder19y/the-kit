# The Kit

A small free-tools website: Word Counter, QR Code Generator, Password Generator, and Case Converter. Pure HTML/CSS/JS, no build step, no backend.

## File structure

```
index.html            homepage
about.html
privacy.html           edit this if you add more data collection later
contact.html          ← put your real email in here before publishing
style.css              shared design system
tools/
  word-counter.html
  qr-generator.html
  password-generator.html
  case-converter.html
```

## 1. Publish it (GitHub Pages)

1. Create a free GitHub account if you don't have one.
2. New repository → name it (e.g. `the-kit`) → public.
3. Upload every file in this folder, **keeping the `tools/` folder structure intact**.
4. Repo → Settings → Pages → Source: `main` branch, `/ (root)` → Save.
5. Your site goes live at `https://yourusername.github.io/the-kit/` within a minute or two.

## 2. Before you tell people about it

- Open `contact.html` and replace `REPLACE-WITH-YOUR-EMAIL@example.com` with a real email.
- Skim `privacy.html` — it's already written to cover analytics + ads, but read it once so it's accurate.

## 3. Add Google Analytics (see how many people visit)

1. Go to analytics.google.com → create a property for your site.
2. Copy the tracking snippet Google gives you (starts with `<script async src="https://www.googletagmanager.com/gtag/js...`).
3. Paste it right after the `<head>` tag in **every** HTML file (index.html, about.html, privacy.html, contact.html, and all four files in `tools/`).
4. Give it a day — traffic shows up in your Analytics dashboard.

## 4. Add Google AdSense (earn money)

1. Apply at adsense.google.com once your site has been live a few weeks with real content (it already has the Privacy/About/Contact pages AdSense looks for).
2. After approval, Google gives you ad unit code snippets.
3. Every tool page already has a marked spot for this — search each file in `tools/` for:
   ```html
   <div class="ad-slot">ad slot</div>
   ```
   Replace that whole `<div>` with the ad code snippet Google gives you.
4. You can add more ad slots elsewhere on the page the same way — just avoid stacking too many, it hurts both user experience and approval odds.

## 5. Add more tools later

Copy any file in `tools/` as a starting template — it already has the header, footer, and shared styling wired up. Give the new file a `<title>`, swap the `<h1>` and the JavaScript logic, and add a matching card to the `.tool-grid` in `index.html`.
