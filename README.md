# nehagupta-16.github.io

Personal academic + professional website for **Neha Gupta** — PhD candidate in Bioinformatics
at the University of Georgia.

Live at 👉 **https://nehagupta-16.github.io**

Built with plain [Jekyll](https://jekyllrb.com/) (custom layout, no external theme) and hosted
free on GitHub Pages.

## How to change things

| I want to… | Edit this file |
| --- | --- |
| Change my name, tagline, email, social links, résumé path | `_config.yml` |
| Add / rename / reorder the tabs in the top menu | `_data/navigation.yml` |
| Add photos to the **Beyond the Lab** gallery | `_data/gallery.yml` + drop images in `assets/images/beyond/` |
| Add blog posts, articles or features | `_data/writing.yml` |
| Edit homepage text | `index.html` |
| Edit research interests, skills, timeline | `research.html` |
| Add a publication | `publications.html` |
| Update CV content | `cv.html` |
| Edit the fun / personal page | `beyond.html` |
| Change colours, fonts, spacing | `assets/css/style.css` (the `:root` block at the top holds every colour) |

### Adding a profile photo

1. Save a headshot as `assets/images/neha.jpg`
2. In `_config.yml`, uncomment the `avatar:` line under `author:`

Until then the site shows a colourful "NG" monogram, so nothing looks broken.

### Updating the résumé

Replace `assets/files/Neha_Gupta_Resume.pdf` with the new PDF, keeping the same filename —
every download button will pick it up automatically.

## Running it locally (optional)

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000. You don't need this to publish — pushing to `main` is enough.
