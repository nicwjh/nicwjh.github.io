---
name: add-research
description: Add a paper or project to the Research tab of nicwong.com from a title, abstract, coauthors, and optional PDF.
---

Add a research entry to `_publications/`.

1. Collect from the user (ask only for what is missing): title, category (`working` or `projects`), date, coauthors, supervisors or venue, abstract, and links (PDF, poster, blog post).
2. If a PDF is provided, copy it into `files/` with a short lowercase hyphenated name. If the PDF is already in `files/` (see CLAUDE.md), reuse it.
3. Create `_publications/YYYY-MM-DD-slug.md`:

   ```yaml
   ---
   title: "<Title>"
   collection: publications
   category: <working|projects>
   permalink: /publication/YYYY-MM-DD-slug
   excerpt: "<one sentence summary>"
   date: YYYY-MM-DD
   venue: "<course, institution, or 'Working paper'>"
   paperurl: "/files/<file>.pdf"
   ---
   With <coauthors>. <Supervision line if any.>

   **Abstract:** <abstract>
   ```

4. No em dashes. Do not invent details.
5. Run `bundle exec jekyll build` and confirm it succeeds, then show the user the new file and offer to commit and push.
