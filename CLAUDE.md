# lulinsong.com — Claude Code notes

Personal academic site for Lulin Song. Jekyll on GitHub Pages, custom domain https://lulinsong.com, default branch `master`. Every push to `master` deploys (about a minute).

## Where things live
- `_config.yml` — name, email, office, links (SSRN, Scholar, LinkedIn, UofA profile), CV path, nav order, Cloudflare analytics token.
- `index.md` — bio, research-area tags, education list, paper cards (short form).
- `research.md` — paper cards with one-line summary, collapsible abstract, funding, committee, presentations, coauthor links.
- `teaching.md` — courses (name/term/description rows).
- `cv.md` — embeds `files/LulinSong_CV.pdf`; to update the CV just replace that file.
- `personal.md` — hobbies and Ski (the husky; image files are `images/seven-*.jpg`).
- `_layouts/default.html`, `_includes/sidebar.html`, `assets/css/site.css` — layout and styles. Accent is UofA green `#007C41`; gold only on the active-nav underline.

## Conventions (decided by Lulin — keep them)
- Official title wording: Assistant Professor / Department of Accounting and Business Analytics / Alberta School of Business. Bio leads with affiliation, then research.
- Paper cards: title (linked to the paper's SSRN abstract page when it exists) → one-line plain-language summary → coauthors · grant → buttons. No SSRN button if the paper isn't on SSRN.
- External links use `target="_blank" rel="noopener"`, including the CV PDF.
- Teaching: no teaching interests, no evaluation scores, no TA courses, no prerequisites.
- Do not trim presentation lists; no UofA logo; footer shows institution only; no phone number.
- To add a paper or course, copy an existing `<li>` block.

## Verifying
- No local Jekyll (system Ruby 2.6); rely on the GitHub Pages build.
- On the UofA campus network, `lulinsong.com` may be blocked by Cisco Umbrella DNS; test with
  `curl --resolve lulinsong.com:443:185.199.108.153 https://lulinsong.com/`.
