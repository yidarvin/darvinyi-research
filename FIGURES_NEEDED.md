# Figures Needed — darvinyi-research

Papers below had no auto-fetchable figure. Save the image and update index.html.

## How to add a figure
1. Save image to `/public/figures/{slug}-fig.png` (or `.jpg`, `.webp`)
2. In `index.html`, find the comment `<!-- FIGURE: {slug} -->`
3. Replace the `.figure-placeholder` div with:
   ```html
   <img src="/figures/{slug}-fig.png" class="paper-figure" alt="[description]">
   ```

---

## Successfully retrieved figures

| Slug | Source URL |
|---|---|
| `upbench` | https://arxiv.org/html/2511.12306/figures/headline.png |
| `mammogram-dream` | https://cdn.ncbi.nlm.nih.gov/pmc/blobs/bfb3/7052735/d9ba5ec55bdf/jamanetwopen-e200265-g003.jpg |
| `brainmetshare` | https://www.frontiersin.org/files/Articles/1056068/xml-images/fninf-16-1056068-g0006.webp |
| `chest-radiograph` | https://cdn.ncbi.nlm.nih.gov/pmc/blobs/0fd1/6358056/776c2c2dd976/radiol.2018181422.fig2.jpg |
| `jamia-distributed` | https://cdn.ncbi.nlm.nih.gov/pmc/blobs/6912/5977656/30ec5cd8399c/2730723f1.jpg |

**Note on `jamia-distributed`:** PMC5977656 figures show data augmentation examples from the training pipeline. If a clearer distributed-learning performance figure is preferred, extract Figure 3 or 4 from the JAMIA paper PDF directly.

---

## Papers requiring manual figure extraction

### ct-org
- Journal URL: https://www.nature.com/articles/s41597-020-00715-8
- PMC URL: N/A (open access but Nature returned 303 redirect — requires browser session)
- Target figure: **Figure 2** — CT cross-section with color-coded simultaneous segmentation overlaid for all 6 organ classes (liver, lungs, bladder, kidney, bones, brain)
- Save as: `/public/figures/ct-org-fig.png`

### federated-npj
- Journal URL: https://www.nature.com/articles/s41746-021-00398-4
- PMC URL: N/A (Nature returned 303 redirect — requires browser session)
- Target figure: **Figure 2 or 3** — Performance convergence curves comparing federated vs. centralized training across 2, 4, and 6+ institutions
- Save as: `/public/figures/federated-npj-fig.png`

### periorbital-seg
- Journal URL: https://www.sciencedirect.com/science/article/pii/S2666914525000557
- PMC URL: N/A
- Target figure: Main segmentation figure — overlay on periorbital photographs showing eyelid boundary annotations
- Save as: `/public/figures/periorbital-seg-fig.png`

### intraop-guidance
- Journal URL (JAMA): https://jamanetwork.com/journals/jamaophthalmology/fullarticle/2787889
- Journal URL (TVST): https://tvst.arvojournals.org/article.aspx?articleid=2792985
- Target figure: Performance evaluation figure or surgical workflow diagram showing real-time AI guidance integration
- Save as: `/public/figures/intraop-guidance-fig.png`

### i-oda
- arXiv URL: https://arxiv.org/abs/2104.02609 (no HTML version, PDF only)
- Target figure: **Figure 1** — Dataset overview showing 12 imaging modalities, disease categories, and data volume distribution
- Save as: `/public/figures/i-oda-fig.png`

### mri-pulse-seq
- arXiv URL: https://arxiv.org/abs/1912.08775 (no HTML version, PDF only)
- Target figure: Architecture comparison diagram (early fusion / late fusion / parallel-branch), plus the input-level dropout training schema showing the 15 possible sequence subsets
- Save as: `/public/figures/mri-pulse-seq-fig.png`

### robust-false-neg
- arXiv URL: https://arxiv.org/abs/2001.09501 (no HTML version, PDF only)
- Target figure: Sensitivity/performance comparison between naive training and lopsided-bootstrap-loss training on size-censored annotation sets
- Save as: `/public/figures/robust-false-neg-fig.png`

### gan-dr
- CVPR PDF: https://openaccess.thecvf.com/content/CVPR2024W/DCAMI/papers/Poles_Repurposing_the_Image_Generative_Potential_Exploiting_GANs_to_Grade_Diabetic_CVPRW_2024_paper.pdf
- Target figure: Side-by-side real vs. GAN-generated retinal fundus images, plus grading performance comparison with and without synthetic augmentation
- Save as: `/public/figures/gan-dr-fig.png`

### iovs-2024
- Journal URL: https://iovs.arvojournals.org/article.aspx?articleid=2805488
- Note: Page returned 403 — likely requires ARVO member login or institutional access. Title and contribution also need updating in index.html once accessible.
- Target figure: Main results figure from the paper
- Save as: `/public/figures/iovs-2024-fig.png`

### tvst-foundational
- Journal URL: https://tvst.arvojournals.org/article.aspx?articleid=2803053
- Note: Page returned 403 — requires institutional access. Title filled from PubMed.
- Target figure: Main results or methods figure from the TVST 2023 generalizability paper
- Save as: `/public/figures/tvst-foundational-fig.png`

### iovs-2023
- Journal URL: https://iovs.arvojournals.org/article.aspx?articleid=2794403
- Note: Page returned 403 — likely requires ARVO member login. Title and contribution need updating in index.html once accessible.
- Target figure: Main results figure from the paper
- Save as: `/public/figures/iovs-2023-fig.png`

### arxiv-2111
- arXiv URL: https://arxiv.org/abs/2111.00042 (no HTML version, PDF only)
- Target figure: CvS architecture diagram and/or classification accuracy comparison vs. baseline methods on small ophthalmic datasets
- Save as: `/public/figures/arxiv-2111-fig.png`

### arxiv-1904
- arXiv URL: https://arxiv.org/abs/1904.11595 (no HTML version, PDF only)
- Target figure: Pipeline diagram or perimeter estimation results on indoor scenes from ScanNet/FloorNet benchmarks
- Save as: `/public/figures/arxiv-1904-fig.png`
