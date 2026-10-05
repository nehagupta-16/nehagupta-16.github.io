# nehagupta-16.github.io

Personal academic + professional website for **Neha Gupta** — PhD candidate in Bioinformatics
at the University of Georgia.

Live at 👉 **https://nehagupta-16.github.io**

Built with plain [Jekyll](https://jekyllrb.com/) (custom layout, no external theme) and hosted
free on GitHub Pages.

## How to change things

| I want to… | Edit this file |
| --- | --- |
| **Update résumé facts** (education, job titles & dates, skills, publications, awards, presentations, leadership) | `_data/cv.yml` — the Research & CV and Publications pages read from it |
| Edit what I did in each role / research descriptions | `research.html` (the "What I work on" section) |
| Replace the downloadable résumé | `assets/files/Neha_Gupta_Resume.pdf` (keep the filename) |
| Change my name, tagline, email, social links | `_config.yml` |
| Change the homepage photo | replace `assets/images/neha.jpg` (portrait, roughly 4:5) |
| Add / rename / reorder tabs in the top menu | `_data/navigation.yml` |
| Add photos to **Beyond the Lab** | drop images in `assets/images/beyond/`, then list them in `_data/gallery.yml` |
| Fill in the optional "Currently" list | `_data/currently.yml` (hidden until an entry is uncommented) |
| Add blog posts, articles or features | `_data/writing.yml` (hidden while empty) |
| Edit the homepage story | `index.html` |
| Edit the personal page | `beyond.html` |
| Change colours, fonts, spacing | `assets/css/style.css` — every colour is in the `:root` block at the top |

### The science drawings on Research & CV

The faint brain, kinase and UMAP drawings live in `assets/images/research/`.
The kinase is traced from the AlphaFold model of DCLK3 (credited at the bottom of
the page, as its CC BY 4.0 licence requires). To make all three stronger or
fainter, change `--art-opacity` near the top of `assets/css/style.css`
(e.g. `.15` → `.25`).

### The mandala borders and backgrounds

The blue band at the top of every page and the green band at the bottom are built in
`assets/css/style.css` (`.mandala-top`, `.mandala-bottom`) from three images:
`assets/images/mandala-ornate-blue.svg`, `mandala-ornate-green.svg` and the faint
`mandala-ghosts.svg`. The same ornate mandalas form the very faint page background on
Beyond the Lab (`body.page-beyond::before` — change its `opacity` to make it stronger
or fainter).

## Running it locally (optional)

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000. You don't need this to publish — pushing to `main` is enough.
