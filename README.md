# knokkeroo-squarespace

Public mirror of the content fragments behind the knokkeroo and Odderon Phi pages on
[odderonphi.com](https://www.odderonphi.com/knokkeroo). Each Squarespace page holds only a small
loader script in a Code Block; on every page load it fetches the matching fragment from this repo's
GitHub Pages URL and injects it. Squarespace still supplies the site's real header, nav, footer and
theme — only the fetched fragment fills the content area.

This repo exists only because Squarespace has no API to update page content or Code Blocks, and
GitHub Pages can't build from the main `knokker` repo (private). So the flow is: edit the source
file in the private `knokker` repo (`docs/odderonphi-com/` or `docs/legal/`), strip its leading
workflow-notes comment, mirror the one file that changed here and push — GitHub Pages redeploys in
under a minute and Squarespace itself is never touched again.

**Do not hand-edit files here directly.** The source of truth is the private `knokker` repo — this
repo is a generated/synced copy.

Fragments served (one per live page): `odderon-phi-home`, `odderon-phi-about-intro`,
`odderon-phi-about-charles`, `odderon-phi-paia`, `knokkeroo-landing`, `what-is-knokkeroo`,
`knokkeroo-terms`, `knokkeroo-account-deletion`, `knokkeroo-reviewer-access`,
`knokkeroo-internal-status`, `knokkeroo-go`, the six tester pages `knokkeroo-test*`,
`wearable-mockups`, and `archisaurus-landing` (Archisaurus Rex shares the site — not knokkeroo's
to delete). `downloads/` holds the tester test-plan `.docx` files.

The original `knokkeroo-status` page this repo was created for was retired on 2026-07-24 and
folded into `knokkeroo-internal-status`; that history is the reason the repo has this name.

Live Pages URL: https://goliontus.github.io/knokkeroo-squarespace/
