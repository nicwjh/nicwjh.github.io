---
name: preview
description: Build nicwong.com locally and check for errors, broken internal links, and leftover template text before pushing.
---

1. Run `bundle install` if `vendor/` or gems are missing, then `bundle exec jekyll build`.
2. Report any build errors with the file and line and fix them.
3. Check `_site/` for leftover template placeholders: `grep -rIl "Your Name\|academicpages\|example.org" _site --include=*.html`.
4. Check that every `/files/...` link in `_site` points to a file that exists in `files/`.
5. Summarize what changed since the last commit (`git status`, `git diff --stat`) and whether it is ready to push.
