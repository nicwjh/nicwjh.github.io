# nicwong.com

Personal academic website for Nicholas Wong, built on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and hosted on GitHub Pages from `nicwjh/nicwjh.github.io` (branch `main`). Custom domain `nicwong.com` is set in `CNAME`; never delete that file.

## Where things live

| What | File(s) |
|---|---|
| Site name, sidebar bio, avatar, social links | `_config.yml` (`author:` block) |
| Header tabs | `_data/navigation.yml` |
| Home page / About | `_pages/about.md` |
| Research tab | `_pages/publications.html` (renders `_publications/*.md`, grouped by `category`) |
| Teaching tab | `_pages/teaching.html` (renders `_teaching/*.md`) |
| Blog tab | `_pages/year-archive.html` (renders `_posts/*.md`) |
| CV tab | `_pages/cv.md`, PDF at `files/cv.pdf` |
| Talks page (exists, not in nav) | `_pages/talks.html` (renders `_talks/*.md`) |
| Avatar | `images/profile.png` |
| PDFs and other downloads | `files/` (served at `https://nicwong.com/files/<name>`) |

Research categories are defined in `_config.yml` under `publication_category` (`working`, `projects`). Every `_publications` entry needs a `category:` matching one of those keys or it will not show.

## Writing style rules

- Never use em dashes in site copy. Use commas, colons, parentheses, or separate sentences.
- Keep copy concise and plain. First person for About; third person is fine for paper blurbs.
- Do not invent facts (affiliations, coauthors, dates, venues). If something is missing, leave a `TODO` comment and say so.

## Content conventions

- `_publications/YYYY-MM-DD-slug.md` front matter: `title`, `collection: publications`, `category`, `permalink: /publication/YYYY-MM-DD-slug`, `excerpt`, `date`, `venue` (optional), `paperurl` (optional, e.g. `/files/paper.pdf`), `citation` (optional). Body holds the abstract.
- `_posts/YYYY-MM-DD-slug.md` front matter: `title`, `date`, `permalink: /posts/YYYY/MM/slug/`, `tags`.
- `_teaching/YYYY-term-slug.md` front matter: `title`, `collection: teaching`, `type`, `permalink: /teaching/YYYY-term-slug`, `venue`, `date`, `location`.
- When an empty section gets its first entry, the "coming soon" placeholder disappears automatically.

## Files carried over from the old site

These PDFs are already in `files/` and can be linked from research entries:
`DDiFTS_v1.pdf` (Double Descent in Financial Time Series), `llms_equity_research.pdf` and `panagora_poster.pdf` (LLMs in Equity Research), `Portfolio_Optimization.pdf`, `nfp-forecasting.pdf`, `NLP_SVBcollapse.pdf`, `T-Rowe-Final-Report.pdf` and `T-Rowe-Final-Deck.pdf` (AI for Financial Analysis), `Wong_Nicholas_Report.pdf` (managerial training program, DiD/RD writing sample), `treasury-liquidity.pdf`, plus older course reports.

The old site (Minimal Light theme) is archived in git history before the migration commit if original wording is needed.

## Workflow

1. Make the edit.
2. Build locally to check it: `bundle exec jekyll build` (or `bundle exec jekyll serve` and open http://localhost:4000). Fix any Liquid/YAML errors before committing.
3. Commit with a short imperative message (e.g. `Add LLM equity research entry`) and push to `main`. GitHub Pages redeploys in about a minute.

Do not open pull requests against the upstream academicpages repo. Do not edit `_layouts/`, `_includes/`, or `_sass/` unless explicitly asked for a design change.
