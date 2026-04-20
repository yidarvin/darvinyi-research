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

## Add figures

See [FIGURES_NEEDED.md](./FIGURES_NEEDED.md) for which papers still need figures.

Quick process:
1. Save image to `/public/figures/{slug}-fig.png`
2. In `index.html`, find `<!-- FIGURE: {slug} -->`
3. Replace the `.figure-placeholder` div with `<img src="/figures/{slug}-fig.png" class="paper-figure" alt="...">`

## Update IOVS/TVST placeholder entries

Three papers returned 403 on fetch. Once you have institutional access:
- `iovs-2024` → https://iovs.arvojournals.org/article.aspx?articleid=2805488
- `iovs-2023` → https://iovs.arvojournals.org/article.aspx?articleid=2794403

In `index.html`, find the accordion items with slugs `paper-iovs-2024` and `paper-iovs-2023` and fill in the title and contribution text.
