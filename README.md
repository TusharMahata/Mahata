# Tushar Kumar Mahata — Résumé

A black-and-white, print-ready A4 résumé built as a single static HTML file. No build step, no dependencies.

**Live content:** WordPress & Shopify development, the remote developer role at [Continental Restaurant Equipment](https://continentalrestaurantequipment.ca/) (March 2025 — present, WordPress → Shopify migration, 300% sales growth), freelance work on Fiverr since 2020, plus selected machine-learning work.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole résumé — markup, styles and print rules in one file |
| `Tushar_Mahata_Resume.pdf` | Two-page A4 PDF export of the same document |

## Run locally

Open `index.html` directly, or serve the folder:

```bash
python -m http.server 8080
# http://localhost:8080
```

## Print / export a PDF

Open the page and use the **Print / Save as PDF** button (bottom right), or `Ctrl/Cmd + P`.

Settings: **A4**, margins **None**, **Background graphics** on. The stylesheet sets `@page { size: A4; margin: 0 }`, so it exports as exactly two pages.

## Deploy

It is a static file — any host works:

- **GitHub Pages** — push this folder, enable Pages on the branch root
- **Netlify / Vercel / Cloudflare Pages** — point at this directory, no build command, no output directory
- **Firebase / S3 / any static host** — upload `index.html`

## Design notes

- Strictly monochrome: black `#0a0a0a`, white, and greys — no accent colours
- Two A4 pages: page 1 is header, profile and experience; page 2 is skills, machine-learning work and education
- Type: **Inter** for text, **IBM Plex Mono** for labels, dates and tags
- Collapses to a single readable column on phones
