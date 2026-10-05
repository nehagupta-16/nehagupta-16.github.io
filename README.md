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

### The mandala borders

The blue band at the top of every page and the green band at the bottom are
`assets/images/mandala-top.svg` and `assets/images/mandala-bottom.svg`. They are
generated vector art, so they stay crisp at any size. To make them taller or
shorter, change `.mandala { height: … }` in `assets/css/style.css`.

## Running it locally (optional)

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000. You don't need this to publish — pushing to `main` is enough.
