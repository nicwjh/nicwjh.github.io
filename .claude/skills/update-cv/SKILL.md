---
name: update-cv
description: Replace the CV PDF on nicwong.com with a new version.
---

1. Ask for the new CV PDF if it was not provided.
2. Copy it to `files/cv.pdf`, overwriting the old one (keep the filename so existing links keep working).
3. If the user wants the CV shown inline, uncomment the `<object>` embed in `_pages/cv.md`.
4. Build with `bundle exec jekyll build`, then commit (`Update CV`) and push after the user confirms.
