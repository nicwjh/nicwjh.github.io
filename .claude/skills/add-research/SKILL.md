---
name: add-research
description: Add a paper or project to the Research tab of nicwong.com from a title, abstract, coauthors, and optional PDF.
---

Add a research entry to `_publications/`.

1. Collect from the user (ask only for what is missing): title, category, date, coauthors (with links if any), status line, abstract, and PDF.
   - `working`: Working Papers. The draft is public, so there is a `paperurl`.
   - `wip`: Work in Progress. No public draft, so no `paperurl`; usually a status line such as "Draft coming soon".
   - `projects`: Selected Projects.
2. If a PDF is provided, copy it into `files/` with a short lowercase hyphenated name. If the PDF is already in `files/` (see CLAUDE.md), reuse it.
3. Create `_publications/YYYY-MM-DD-slug.md`:

   ```yaml
   ---
   title: "<Title>"
   collection: publications
   category: <working|wip|projects>
   date: YYYY-MM-DD
   coauthors: '[<Name>](<url>) and [<Name>](<url>)'   # optional, markdown
   status: "<e.g. Draft coming soon>"                  # optional
   paperurl: "/files/<file>.pdf"                       # optional, links the title
   ---
   <optional abstract; leave the body empty for none>
   ```

   Omit any optional field that does not apply. Do not add `permalink`, `excerpt`, `venue`, or `citation`; the Research page does not use them and papers have no standalone pages.
4. Moving a paper from `wip` to `working` happens only when the draft is made public: change `category` to `working`, add `paperurl`, and remove `status`.
5. No em dashes. Do not invent details.
6. Run `bundle exec jekyll build` and confirm it succeeds, then show the user the new file and offer to commit and push.
