# Figures — darvinyi-research

All paper figures are resolved and stored locally in `figures/` (referenced as `/figures/{slug}-fig.png`). No external image hosts are used. This file records where each figure came from.

## How to replace a figure
1. Save image to `figures/{slug}-fig.png` (or `.jpg`, `.webp`) — repo root, **not** `public/`.
2. In `index.html`, find `<!-- FIGURE: {slug} -->` and point its `<img class="paper-figure">` at `/figures/{slug}-fig.png`.

---

## Retrieved figures (16)

| Slug | Figure | Source |
|---|---|---|
| `upbench` | task completion-rate bar chart | arXiv 2511.12306 (headline figure) |
| `mammogram-dream` | ROC curves, AI vs radiologist benchmarks | JAMA Network Open, PMC7052735 |
| `brainmetshare` | brain-metastasis segmentation overlays | Frontiers Neuroinformatics 2022 |
| `ct-org` | tri-planar CT + 3D render, organ segmentation (Fig 2) | Nature Sci Data s41597-020-00715-8 |
| `chest-radiograph` | ROC curves by training-set size | Radiology 2019, PMC6358056 |
| `periorbital-seg` | periorbital segmentation grid (CFD + Celeb) | ScienceDirect S2666914525000557 (fig CDN `ars.els-cdn.com`) |
| `intraop-guidance` | AI intraoperative-guidance workflow (Fig 1) | JAMA Ophthalmology 2021, PMC8855235 |
| `i-oda` | 6-modality dataset sample grid (Fig 3) | arXiv 2104.02609v1 (PDF render) |
| `jamia-distributed` | augmentation examples | JAMIA 2018, PMC5977656 |
| `federated-npj` | ROC detection curves, DeepLab v3 vs ILD (Fig 2) | npj Digital Medicine s41746-021-00398-4 |
| `mri-pulse-seq` | multi-sequence fusion architecture | arXiv 1912.08775 (ar5iv) |
| `robust-false-neg` | segmentation across lesion sizes (Fig 4) | arXiv 2001.09501 (ar5iv) |
| `gan-dr` | real vs GAN-generated fundus grid (Fig 4) | CVPR 2024W DCAMI (PDF extract) |
| `tvst-foundational` | segmentation→classification pipeline (Fig 3) | TVST 2023, PMC10629532 |
| `arxiv-2111` | CvS architecture overview (Fig 1) | arXiv 2111.00042 (PDF render) |
| `arxiv-1904` | DeepPerimeter pipeline (Fig 2) | arXiv 1904.11595 (ar5iv) |

## No-figure entries (2)

`iovs-2024` and `iovs-2023` are ARVO Annual Meeting abstracts (Rashidisabet, Chan, Vajaranant, Yi — UIC) published in *Investigative Ophthalmology & Visual Science*. They contain only a results table, not a scientific figure, so they intentionally have no `<img>`. Titles and contributions were recovered from the ARVO abstracts (the arvojournals.org pages are behind a Cloudflare human-verification wall):
- `iovs-2024` (id 2805488) — "Adversarial Domain Adaptation for Robust Glaucoma Classification"
- `iovs-2023` (id 2794403) — "Out-of-Distribution Detection via Uncertainty Learning for Robust Glaucoma Prediction"

## Notes
- Nature/Springer figures are served at 685px max by the CDN (`/full/` returns a broken placeholder), so `ct-org` and `federated-npj` are 685px wide.
- `federated-npj` (npj s41746-021-00398-4) is the "missing MRI sequences / multicenter" study; its Fig 2 shows detection ROC curves (not federated-vs-centralized convergence), and the `alt` text describes it accordingly.
