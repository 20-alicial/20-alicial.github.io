# 20-alicial.github.io

Personal website of Alicia Liu, built with [Jekyll](https://jekyllrb.com/) and the
[al-folio](https://github.com/alshedivat/al-folio) theme.

## Editing content

| What | Where |
| --- | --- |
| Bio / homepage | `_pages/about.md` |
| News items | `_news/` (one Markdown file per item) |
| Publications | `_bibliography/papers.bib` |
| Ongoing research & talks | `_pages/research.md` |
| Essays | `_pages/essays.md` |
| Photography | `_pages/photography.md` (images in `assets/img/photos/`) |
| Site title, URL, socials | `_config.yml`, `_data/socials.yml` |
| PDFs | `files/` (legacy links) and `assets/pdf/` |

## Deployment

Pushes to `master` trigger `.github/workflows/deploy.yml`, which builds the site and
pushes the result to the `gh-pages` branch. GitHub Pages must be configured to serve
from `gh-pages` (Settings → Pages → Source: Deploy from a branch → `gh-pages` / root).

## Local preview

Requires Ruby 3.x and ImageMagick:

```bash
bundle install
bundle exec jekyll serve
```

Or with Docker: `docker compose up`.
