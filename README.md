# Redline Discovery — site

Static site, no build step. All files sit in this one folder; keep them together.

## Deploy

1. Create a GitHub repo and upload every file in this folder to the repo root.
2. Vercel → New Project → import the repo.
3. Framework preset: **Other**. Build command: none. Output directory: `./`.
4. Deploy.

## Files

- `index.html` — the site
- `RLD-CTA.dc.html` — contact / demo block, loaded by index.html
- `support.js`, `image-slot.js`, `articles.js` — scripts
- `redline-logo.png`, `hero-magnifier-v2.png`, `spotlight-dashboard.avif` — images
- `image-slots.state.json` — photos placed in the page's image slots (keep it)
- `vercel.json` — caching headers

Fonts load from Google Fonts.
