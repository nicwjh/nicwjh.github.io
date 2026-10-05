---
name: add-post
description: Draft and add a blog post to the Blog tab of nicwong.com.
---

1. Get the topic, title, and any draft text or notes from the user.
2. Create `_posts/YYYY-MM-DD-slug.md` (today's date unless told otherwise):

   ```yaml
   ---
   title: "<Title>"
   date: YYYY-MM-DD
   permalink: /posts/YYYY/MM/slug/
   tags:
     - <tag>
   ---
   ```

3. Write in Nick's voice: direct, concise, no em dashes. Math can use `$...$` (MathJax is enabled). Images go in `images/` and are referenced as `/images/<file>`.
4. Build with `bundle exec jekyll build`, then show the draft and wait for approval before committing and pushing.
