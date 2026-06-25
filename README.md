# Thomas R Vargas - Personal Website

This repository contains the source code for my personal academic website, hosted at [thomasrvargas.com](https://www.thomasrvargas.com).

### Tech Stack
* **Framework:** [Quarto](https://quarto.org/) (R)
* **Hosting:** Netlify via GitHub
* **Design:** Custom editorial theme using Bootstrap 5 & CSS

### Reproducibility
This site is built using RStudio.

### File naming convention
PDFs in `files/` and figures in `images/` follow a standardized
`YYYY-keyword.pdf` / `YYYY-keyword.png` scheme (lowercase, kebab-case), so each
paper's PDF and figure share the same stem and the list sorts chronologically —
e.g. `2026-homeowners.pdf` ↔ `images/2026-homeowners.png`. The shared
`images/dissertation-graph.png` (used on the home page) is the one exception.

To add a new paper: drop the PDF in `files/` and its figure in `images/` using
this scheme, then copy a `<div class="paper" data-tags="…">` block in
`research.qmd`. If you introduce a new tag, add a matching
`<button class="filter-chip" data-tag="…">` to the filter bar.
