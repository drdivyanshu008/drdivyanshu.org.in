# drdivyanshupatel.org.in — Static Site (Auto Deploy)

This repository contains the **ready-to-use** website for **Dr. Divyanshu Patel**.
- GitHub Pages auto-deploy via **GitHub Actions** (file: `.github/workflows/pages.yml`)
- SEO: `sitemap.xml`, `robots.txt`, OG/Twitter meta, PWA manifest
- Legal: `privacy.html`, `terms.html`
- 404 page and `CNAME` for custom domain

## 1) Create repo & push
```bash
git init
git branch -m main
git add .
git commit -m "Initial publish"
git remote add origin https://github.com/<YOUR_USERNAME>/drdivyanshu-patel-site.git
git push -u origin main
```

## 2) Enable Pages
Repo → **Settings → Pages** → Source: **GitHub Actions** (already configured).

The workflow will publish to Pages automatically on each push.

## 3) Custom domain
- Settings → Pages → Custom domain: `drdivyanshupatel.org.in`
- DNS records at your registrar:
  - A (apex @): 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
  - CNAME (www): `<YOUR_USERNAME>.github.io`
- Enable **Enforce HTTPS** (after certificate is issued).

> GA4: Replace `G-XXXX` in `index.html` if you want analytics.

---

© 2025 Dr. Divyanshu Patel
