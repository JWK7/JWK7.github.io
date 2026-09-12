# Bellman Meets Kolmogorov — project page

Static project website for *Bellman Meets Kolmogorov: Unsupervised Reinforcement Learning Through Mastering Chaos*.

## Layout

```
index.html               the whole site (single page, no build step)
assets/paper.pdf         the paper
assets/figures/          Figure 1 strips, Figure 2 (gibbon), Figure 3 (method, SVG), Figure 4 (Lorenz)
assets/videos/           hopper_cip, walker_cip (hero), hopper_6way, walker_6way (Q3 comparison)
```

Fonts come from Google Fonts and equations are rendered by MathJax 3 from cdnjs, so the page needs
network access for those two things; everything else is local.

## Preview locally

```
python3 -m http.server 8000
```

then open <http://localhost:8000>. Opening `index.html` directly from Finder also works.

## Deploy

Any static host works. For GitHub Pages: push this folder to a repository, then in
*Settings → Pages* choose the `main` branch, root folder.

## Before publishing

Two hero buttons are placeholders until the links exist. Search `index.html` for `TODO`:

- `arXiv` button — set `href` to the arXiv abstract URL.
- `Code` button — set `href` to the code repository.

The BibTeX entry in the *Cite* section uses the venue from the paper's copyright line (AAAI 2027);
update pages, volume, and DOI once assigned.
