# Redline Discovery — site

Static site, no build step. `index.html` is the production entry point.

## Deploy (GitHub → Vercel)

```bash
git init
git add .
git commit -m "Redline Discovery site"
git remote add origin git@github.com:<user>/<repo>.git
git push -u origin main
```

Then in Vercel: New Project → import the repo → Framework preset **Other**, Build command: none, Output directory: `./` → Deploy.

## Files

- `index.html` — the site (production entry)
- `Redline Discovery Site.dc.html` — editable source; `index.html` is a copy of it
- `RLD-CTA.dc.html` — standalone CTA block
- `support.js`, `image-slot.js` — runtime scripts (must stay next to the HTML)
- `hero-magnifier-v2.png`, `spotlight-dashboard.avif`, `redline-logo.png` — images

After editing the source file, refresh the copy:

```bash
cp "Redline Discovery Site.dc.html" index.html
```

Fonts load from Google Fonts, so the deployed page needs network access.
