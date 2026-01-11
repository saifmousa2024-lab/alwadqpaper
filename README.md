# Deployment Notes

## Before deployment
1. Replace company contact details in:
   - `site/index.html`
   - `site/about.html`
   - `site/contact.html`
2. Update:
   - `site/robots.txt` (set your domain in Sitemap line)
   - `site/sitemap.xml` (replace YOUR-DOMAIN.com with your real domain or Netlify URL)

## Netlify
- Drag & drop the `site/` folder in Netlify manual deploy.

## GitHub Pages (Recommended approach)
- Either:
  - Move all files inside `site/` to the repository root, OR
  - Configure Pages to publish from `/site` (if your instructor allows).
