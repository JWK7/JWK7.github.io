# Bellman Meets Lyapunov — project page

Static project website for *Bellman Meets Lyapunov: Unsupervised Reinforcement Learning via Mastering Chaos*
(under review at ICLR 2027; [arXiv:2610.02012](https://arxiv.org/abs/2610.02012)).

## Layout

```
index.html               the whole site (single page, no build step)
assets/paper.pdf         earlier (AAAI) version of the paper; the page links to arXiv instead
assets/figures/          Figure 1 strips, Figure 2 (method, SVG), Figure 3 (Lorenz), Figure 4 (gibbon)
assets/videos/           hopper_cip, walker_cip (hero), hopper_6way, walker_6way (Q3 comparison)
```

Figure and equation numbers follow the ICLR submission.

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

## Citation

The BibTeX entry in the *Cite* section points to the arXiv preprint. Update it to the
ICLR proceedings entry if the paper is accepted.
