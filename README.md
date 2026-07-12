# research.darvinyi.com

Static research portfolio for Darvin Yi. Single-page site showcasing 18 papers across two threads: datasets/benchmarks and foundational AIML methods.

## Run locally

Open `index.html` directly in a browser, or serve with:

```bash
npx serve .
```

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → **Add New Project** → import the repo
3. Vercel auto-detects a static site — no build settings needed
4. After deploy, go to **Project Settings → Domains** → add `research.darvinyi.com`
5. In Namecheap DNS for `darvinyi.com`, add a CNAME record:
   - **Host:** `research`
   - **Value:** `cname.vercel-dns.com`
6. Pushing to `main` auto-deploys via Vercel webhook

## Figures

All figures are stored locally in `figures/` at the repo root and referenced as `/figures/{slug}-fig.png`. No external image hosts are used. See [FIGURES_NEEDED.md](./FIGURES_NEEDED.md) for the source of each figure.

To add or replace a figure:
1. Save the image to `figures/{slug}-fig.png` (repo root — **not** `public/`; this is a no-build static deploy, so the path on disk is the served path).
2. In `index.html`, find `<!-- FIGURE: {slug} -->`.
3. Point the `<img class="paper-figure">` at `/figures/{slug}-fig.png` and update its `alt` text.

The two `iovs-*` entries are ARVO Annual Meeting abstracts with no scientific figure (results table only), so they intentionally have no `<img>`.
