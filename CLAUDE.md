# CLAUDE.md

Personal academic site of Hoyong Kim (https://khyong.github.io), built on the al-folio v1 starter. Runtime (layouts, includes, Sass, JS) lives in the pinned `al_*` gems listed in `Gemfile` and `_config.yml`; this repo holds only configuration and content.

## Working here

- Content map: see `README.md`. Bio in `_pages/about.md`, papers in `_bibliography/papers.bib`, CV data in `_data/cv.yml`, news in `_news/`, research cards in `_projects/`, courses in `_teachings/`.
- `baseurl` is empty (site is served at the domain root). Do not pass `--baseurl /al-folio`.
- Adding or removing a plugin requires editing both `Gemfile` and the `plugins:` list in `_config.yml`.
- Local overrides of gem-owned files (`_layouts/`, `_includes/`, `_sass/`) are allowed for this site but should be the last resort; prefer `_config.yml` and `_data/`.
- `new/` holds the original handoff notes from the first design pass and is excluded from the build.

## Commands

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"   # Homebrew Ruby 3.x
bundle install
bundle exec jekyll serve          # http://localhost:4000/
bundle exec jekyll build          # output in _site/
npx prettier . --check            # formatting (CI runs this)
```

## Deployment

`.github/workflows/deploy.yml` builds on push to `master` and publishes to the `gh-pages` branch; GitHub Pages serves that branch.
