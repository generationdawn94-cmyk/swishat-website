# Swisha T — Official Site

Static site for https://swishamusic.com/

## What's in here
- `index.html` — the whole site (home, music, videos, tour, shop, about, contact)
- `banner.jpg` — new hero photo (sepia portrait), optimized. Was a 754KB base64 image inline in the HTML — now a separate cached file, so `index.html` is much smaller and faster.
- `about.jpg` — same photo, used as the About / press photo (was a "Coming Soon" placeholder)
- `og-image.jpg` — 1200x630 social preview, linked in og:image / twitter:image (the old `banner.png` reference didn't exist as a file)
- `favicon.ico`, `favicon-32x32.png`, `favicon-48x48.png`, `favicon-192x192.png`, `apple-touch-icon.png`, `icon-512.png` — black & gold ST logo
- `robots.txt`, `sitemap.xml` (lastmod 2026-11-19), `site.webmanifest`, `404.html`

## Aesthetic revamp
The old teal accent clashed with the new sepia photo, so teal is gone — replaced with warm sepia tan (#A67C52 / #C9A86A) and a light sepia filter on the hero. Gold (#C8952A) stays. Hero object-position is now centre 18% so his face stays in frame on desktop and mobile.

## Releases — updated Nov 19, 2026
- Pray — out now, July 3, 2026, Left Lane Music, 1:45, written by Taleb Mansour. Featured on Chymamusique MUSIQUE compiled vol 1 (Sept 23, 2026). Official music video on YouTube.
- One Of One — Dillin Hoox, Swisha T, Lil Durk — Sept 5, 2025
- Downfall — Jstn Dmnd, Swisha T — Aug 1, 2025
- Handout — Dillin Hoox, Swisha T — Mar 7, 2025
- The Truth — Feb 21, 2025
- Plus No Love, Sober, Chapo, Fallen Soul, Legends in the Music grid, all linked to Spotify.

Streaming: the Music page has a featured Pray block with Spotify / Apple Music / YouTube / SoundCloud / Deezer buttons, plus the Spotify artist embed. No per-track URLs were invented — cards link to the Spotify artist page unless a track URL was already on the old site.

## Deploy (Vercel)
Upload the *contents* of this folder to the project root — `index.html` must be at the root, not inside a subfolder. If the files are inside a folder (e.g. `swisha-t-website/`), set Settings > General > Root Directory to that folder, then Redeploy. Same lesson as the Generation Dawn site: a nested folder + a misnamed index file = Vercel 404.
