# Decision log

Newest first. To change a decision, add a new entry that supersedes the old
one — do not edit history.

---

### D-004 · Curated selection, not the archive — 2026-11-02
The site shows a selected stream from a large archive. Reasons: a stronger
portfolio for an institutional audience, and GitHub Pages' ~1 GB limit (with
git history counting every image ever committed).

### D-003 · Single tiled stream, no text on images — 2026-11-02
The portfolio is one continuous tiled field of photographs. Words appear only
on the About page. Reason: the owner's philosophy — the images carry the site.

### D-002 · Astro static site, deployed with GitHub Actions — 2026-11-02 _(proposed)_
GitHub Pages can only serve static files. Astro outputs plain HTML/CSS with
no JS by default and generates responsive image sizes/formats at build time,
so only one web master per photo is committed. Content lives in data files,
separated from layout.

### D-001 · Host on GitHub Pages at kopaszmarton.github.io — 2026-11-02
Free hosting with HTTPS, custom-domain support, and version history of every
change. Accepted constraints: static only, ~1 GB, public repository.
