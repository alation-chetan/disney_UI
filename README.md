# Enterprise Data Marketplace — UI Prototype

A self-contained UI prototype for reviewing the marketplace design with the customer.
It models three marketplaces — **Enterprise Data Marketplace (EDM)**, **Segment Marketplace A**,
and **Segment Marketplace B** — that share one layout, where data products published in a
segment can be **pushed up** to the top-level EDM for company-wide discovery.

## Highlights
- **App shell**: marketplace rail (EDM / Segment A / Segment B) + a collapsible *Data Products App* menu (The Marketplace, My Bookmarks, Manage Authentication, My Data Products, Manage).
- **The Marketplace**: Home / Browse / Bookmarks content tabs.
  - *Home* — branded hero, welcome, Domains, Recently Used, Most Popular.
  - *Browse* — AI "How can I help you today?" insights hero + full catalog with sort / filter / search.
- **Push-to-EDM** flow with a distinct **enterprise domain** taxonomy (choose which enterprise domain a product maps into).
- **Manage** — full customization (logo upload, background gradients / images / upload, all text, section visibility, domains-shown count, hero alignment) with a live preview, plus data-product curation and a *Create data product* flow (segments only).
- Clean inline SVG icon set, editorial serif headings, light/refined palette.

No build step, no dependencies — everything is inline in `index.html`.

## Run locally
Just open the file:
```bash
open index.html
```
Or serve it:
```bash
python3 -m http.server 8777
# then visit http://localhost:8777/index.html
```

## Deploy (Vercel)
This is a static site — Vercel serves `index.html` directly, no build needed.
Import this repo at https://vercel.com/new (Framework Preset: **Other**), or run `vercel` from this folder.

> The "Disney" branding is a placeholder logo/wordmark for design review, not the real Disney logo.
