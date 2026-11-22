# Generation Dawn — Official Site

Static site for https://generationdawn.com/

## What's in here
- `index.html` — the whole site (home, releases, music, videos, tour, about, contact)
- `assets/hero.jpg` — hero image, optimized (was 500KB+ base64 inline, now a separate cached file)
- `og-image.jpg` — 1200×630 social preview image
- `favicon.svg`, `favicon.ico`, `favicon-32x32.png`, `favicon-16x16.png`, `favicon-512.png`, `apple-touch-icon.png`
- `robots.txt`, `sitemap.xml` — SEO
- `site.webmanifest` — install / home-screen info
- `404.html` — custom 404 page
- `.nojekyll` — tells GitHub Pages not to run Jekyll (important, otherwise files starting with `_` / plain HTML can break)
- `CNAME` — custom domain `generationdawn.com`. Delete this file if you are NOT using that domain yet.
- `.github/workflows/static.yml` — GitHub Actions deploy to Pages (optional)

## Deploy to GitHub Pages
1. Create a repo (e.g. `generation-dawn-site`), upload all files in this folder to the repo root, on the `main` branch.
2. GitHub repo > Settings > Pages > Build and deployment > Source: **GitHub Actions**.
3. Push — the workflow deploys automatically. Your site will be at `https://<username>.github.io/<repo>/` until the custom domain is set.
4. For the custom domain: Settings > Pages > Custom domain > enter `generationdawn.com`, save, then add the DNS records GitHub shows (A / CNAME) at your domain registrar. Keep the `CNAME` file in the repo.

## Update a release date
Edit `index.html` — the dates are in:
- the hero countdown + drop chip
- the home strip
- the Releases cards
- the About copy and footer
- the JSON-LD `MusicRelease` block in `<head>` (for Google)
- `sitemap.xml` — update `<lastmod>` when you change the page

Then commit + push. No build step.
