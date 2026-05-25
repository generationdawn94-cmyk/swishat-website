# Swisha T — Official Website

Official artist website for Swisha T. Built as a single-file static site.

## Structure

```
/
├── index.html    # Full site — all 7 pages
└── README.md
```

## Pages

- **Home** — Hero, stats, song marquee
- **Music** — Live Spotify embed + catalog
- **Videos** — Music video + content grid
- **Tour** — Live dates + booking CTA
- **Shop** — Merch store with Stripe checkout modal
- **About / Press** — Bio, EPK, press downloads
- **Contact** — Management, booking, press, sync contacts + form

## Deployment

Deployed via [Vercel](https://vercel.com) — auto-deploys on every push to `main`.

## Stripe Setup

To activate payments in the Shop:

1. Create a [Stripe account](https://stripe.com)
2. Either use **Stripe Payment Links** (recommended — zero code) or integrate Stripe.js
3. Replace the `handleStripeCheckout()` function in `index.html` with your Stripe publishable key and checkout session logic

## Domain

Connect via Vercel → Project Settings → Domains.
Add the Vercel-provided A record and CNAME to your DNS registrar.

## Updating Content

All content lives in `index.html`. Search for the relevant section comment:

- `<!-- HOME -->` — hero text, stats
- `<!-- MUSIC -->` — releases grid, Spotify embed
- `<!-- VIDEOS -->` — video grid
- `<!-- TOUR -->` — show dates table
- `<!-- MERCH -->` — products, prices
- `<!-- ABOUT -->` — bio text, facts
- `<!-- CONTACT -->` — email addresses, form

## To Do Before Launch

- [ ] Replace placeholder press photo
- [ ] Add real email addresses (management, booking, press, sync)
- [ ] Add real social media URLs (Instagram, TikTok, YouTube)
- [ ] Connect Stripe for live payments
- [ ] Upload actual merch designs to replace placeholders
- [ ] Add music video YouTube embed URL
- [ ] Confirm tour dates and update table
- [ ] Add EPK PDF download links

---

© 2026 Swisha T. All Rights Reserved.
