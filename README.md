# khyong.github.io

Personal academic homepage of Hoyong Kim, built with the [al-folio](https://github.com/alshedivat/al-folio) v1 starter (Jekyll) and deployed to GitHub Pages at https://khyong.github.io.

## Where the content lives

| What                     | File(s)                                     |
| ------------------------ | ------------------------------------------- |
| Site settings, name, URL | `_config.yml`                               |
| Bio on the front page    | `_pages/about.md`                           |
| Social links / email     | `_data/socials.yml`                         |
| News items               | `_news/announcement_*.md`                   |
| Publications             | `_bibliography/papers.bib`                  |
| Publication thumbnails   | `assets/img/publication_preview/`           |
| CV (web)                 | `_data/cv.yml`, `_pages/cv.md`              |
| CV (PDF)                 | `assets/pdf/CV_HoyongKim.pdf`               |
| Research directions      | `_projects/*.md` (rendered at `/research/`) |
| Teaching                 | `_teachings/*.md`, `_pages/teaching.md`     |
| Blog posts (optional)    | `_posts/YYYY-MM-DD-title.md`                |
| Profile photo            | `assets/img/prof_pic.jpg`                   |

## Local preview

Requires Ruby 3.3+ (for example `brew install ruby`) and ImageMagick.

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"
bundle install
bundle exec jekyll serve   # http://localhost:4000/
```

## Deployment

Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site and pushes the result to the `gh-pages` branch. One-time GitHub setup:

1. Settings → Actions → General → Workflow permissions → **Read and write permissions**.
2. After the first successful run, Settings → Pages → Source → **Deploy from a branch**, branch `gh-pages`, folder `/ (root)`.

## Updating the theme

Runtime (layouts, styles, scripts) lives in the pinned `al_*` gems in `Gemfile`. To upgrade, bump the pins in `Gemfile` and the matching entries in `_config.yml`, then run `bundle exec al-folio upgrade audit`. See `docs/` for the upstream guides.
