<!-- ©︎ BBQ大好き All Rights Reserved. -->

# BBQ Daisuki Privacy

Static GitHub Pages site for privacy and legal notices published at `privacy.bbqdaisuki.moe`.

## Public routes

- `/` — legal-document index
- `/crash-reporting/privacy/` — BBQ Daisuki Applications Crash Reporting Notice
- `/crash-reporting/terms/` — Terms of Crash Report Submission

## Publishing

GitHub Pages serves the repository's `main` branch from `/` (root). `CNAME` owns the custom-domain declaration. Cloudflare DNS must point `privacy.bbqdaisuki.moe` to the GitHub Pages host before GitHub can provision HTTPS.

The site is intentionally dependency-free: static HTML and CSS only, with no JavaScript, analytics, cookies, remote fonts, or third-party page resources.

## Local preview

```powershell
python -m http.server 4173
```

Open `http://127.0.0.1:4173/`.

## Maintenance

When data handling changes, update the relevant notice and the `lastmod` values in `sitemap.xml`. Legal text should be reviewed for the actual products, users, infrastructure, and jurisdictions before material changes are published.
