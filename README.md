# knokkeroo-squarespace

Public mirror of the content behind [odderonphi.com/knokkeroo-status](https://www.odderonphi.com/knokkeroo-status).

This repo exists only because Squarespace has no API to update page content or Code Blocks, and
GitHub Pages can't build from the main `knokker` repo (private, and this account isn't on a paid
GitHub plan). So the flow is: edit the page in the private `knokker` repo as usual, then mirror the
one file that changed here and push — GitHub Pages redeploys automatically, and a tiny loader
script already pasted into the Squarespace page's Code Block fetches the live version of
`knokkeroo-status.html` from this repo's Pages URL on every page load. Squarespace still supplies
the site's real header, nav, footer and theme — only the fetched fragment fills the content area.

**Do not hand-edit files here directly.** The source of truth is
`docs/odderonphi-com/knokkeroo-status.html` in the private `knokker` repo — this repo is a
generated/synced copy (the leading `<!-- ... -->` workflow-notes comment is stripped since it's
internal-only).

- `knokkeroo-status.html` — the bare content fragment the Squarespace Code Block's loader script
  fetches at runtime.
- `index.html` — a standalone preview that fetches and renders the same fragment, so the content
  can be checked without touching the live Squarespace page (won't have Squarespace's real
  header/nav/footer/theme around it — those only apply on the real site).

Live Pages URL: https://goliontus.github.io/knokkeroo-squarespace/
