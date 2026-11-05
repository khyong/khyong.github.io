# khyong.github.io: handoff for Claude Code

Paste this into Claude Code from inside the `khyong.github.io` repo, together with the files below.

## Task

1. Set up the repo with the al-folio template (https://github.com/alshedivat/al-folio).
   If the repo is empty, recreate it from the template ("Use this template") or merge al-folio into it.
2. Configure `_config.yml`: first_name Hoyong, last_name Kim, url https://khyong.github.io, baseurl empty.
3. Place the content files:
   - `papers.bib` → `_bibliography/papers.bib`
   - `about.md` → `_pages/about.md` (adapt front matter keys to the installed al-folio version, e.g. `news` vs `announcements`)
   - `socials.yml` → `_data/socials.yml` (or the matching keys in `_config.yml` for older versions)
   - `news.md` → split into `_news/announcement_1.md` … `announcement_6.md`
4. Remove the template's sample news, projects, blog posts, and example bib entries.
5. Profile photo → `assets/img/prof_pic.jpg`.
   Publication thumbnails → `assets/img/publication_preview/` using the `preview` filenames in `papers.bib`
   (the current Google Sites page has a thumbnail for each paper that can be reused).
6. Enable deployment: Settings → Actions → General → Workflow permissions = Read and write;
   after the first successful build, Settings → Pages → Deploy from branch `gh-pages`.
7. Run a local preview (`docker compose up`), check every page, then commit and push.

## Still to confirm (search for TODO in the files)

- Final title and authors of the NeurIPS 2026 paper, plus its OpenReview link
- Current position title and lab URL in `about.md`
- Public email in `socials.yml`
- News dates marked TODO

## Later additions

- CV page (`_data/cv.yml` or a PDF in `assets/pdf/`)
- Projects page for VLA interpretability and world model work
- Honors and academic service (reviewer for ICLR 2025, NeurIPS 2025, ICLR 2026)
