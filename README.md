# nehagupta-16.github.io

Personal academic + professional website for **Neha Gupta** — PhD candidate in Bioinformatics
at the University of Georgia.

Live at 👉 **https://nehagupta-16.github.io**

Built with plain [Jekyll](https://jekyllrb.com/) (custom layout, no external theme) and hosted
free on GitHub Pages.

## Pages

| Tab | File |
| --- | --- |
| Home | `index.html` |
| Research & Résumé (research, publications, presentations, experience, education, skills, awards) | `research.html` |
| Beyond the Lab | `beyond.html` |
| Let's get in touch | `contact.html` |

`cv.html` and `publications.html` are redirects, so older links to `/cv/` and
`/publications/` still land in the right place on Research & Résumé.

## How to change things

| I want to… | Edit this file |
| --- | --- |
| **Update résumé facts** (education, job titles & dates, skills, publications, awards, presentations, leadership) | `_data/cv.yml` |
| Edit what I did in each role / research descriptions | `research.html` ("What I work on") |
| Replace the downloadable résumé | `assets/files/Neha_Gupta_Resume.pdf` (keep the filename). Download links carry a `?v=` stamp that changes on every rebuild, so visitors always get the newest copy |
| Change my name, tagline, email, social links | `_config.yml` |
| Change the homepage photo | replace `assets/images/neha.jpg` (portrait, roughly 4:5) |
| Add / rename / reorder tabs in the top menu | `_data/navigation.yml` |
| Add photos to **Beyond the Lab** | drop images in `assets/images/beyond/`, then add `image:` lines in `_data/gallery.yml`. The Photographs section appears automatically once at least one photo is listed |
| Fill in the optional "Currently" list | `_data/currently.yml` (hidden until an entry is uncommented) |
| Add blog posts, articles or features | `_data/writing.yml` (hidden while empty) |
| Change colours, fonts, spacing | `assets/css/style.css`. Every colour is in the `:root` block at the top |

### Mandala artwork

- **Top and bottom bands** (every page): `.mandala-top` / `.mandala-bottom` in the CSS,
  built from `mandala-ornate-blue.svg`, `mandala-ornate-green.svg` and `mandala-ghosts.svg`.
- **Page backgrounds** (every page): a faint seamless wallpaper, `pattern-tile.svg`
  (`body::before`), plus one large blue-to-green line mandala, `mandala-line.svg`
  (`body::after`), placed on a different edge for each page. Beyond the Lab uses the two
  layered mandalas in its corners instead. Change the `opacity` values on those two rules
  to make the backgrounds stronger or fainter.

### Science drawings on Research & Résumé

The brain and kinase drawings live in `assets/images/research/`. Their strength is
`--art-opacity` near the top of the CSS.

## Credits

The kinase drawing is adapted from the AlphaFold model of human DCLK3,
[AF-Q9C098-F1](https://alphafold.ebi.ac.uk/entry/Q9C098) (AlphaFold Protein Structure
Database, DeepMind / EMBL-EBI), licensed
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Changes: the Cα trace of
residues 342–618 was redrawn as a 2D cartoon. The same credit is embedded in the image file.

## Running it locally (optional)

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000. You don't need this to publish — pushing to `main` is enough.
