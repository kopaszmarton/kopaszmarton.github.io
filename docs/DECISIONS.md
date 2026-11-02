# Decision log

Newest first. To change a decision, add a new entry that supersedes the old
one — do not edit history.

---

### D-010 · Geometric controls — 2026-11-02 _(proposed, see prototype v1)_
No icons or small UI. Three gestures only: a circle tile opens About (the circle
returns from it); huge triangles move through a series; tapping anywhere else
in the viewer, Esc, or swiping down returns to the wall. Marks are drawn in a
tone of the field colour so they stay bold without competing with the photos.

### D-009 · English and Hungarian — 2026-11-02
The site is bilingual. Since the wall has no text, this mainly affects the
About page, page titles, alt text and metadata.

### D-008 · Viewer: screen-size image on the colour field — 2026-11-02
Opening a tile shows the full, uncropped photograph as large as the screen
allows, floating on the colour field. Single images: tap to return. Series:
triangles (or swipe / arrow keys) move through the series.

### D-007 · Bold single-colour field, never white — 2026-11-02
White is too prosaic for artistic imagery. One saturated colour carries the
whole site; black-and-white and colour photographs both sit on it. Direction:
deep/harsh blue (Klein blue, indigo, ocean); pink kept as an alternative.
Exact hue to be chosen from the prototype.

### D-006 · Equal tiles, no gaps — supersedes the tiling options in BRIEF — 2026-11-02
The wall is a grid of equal-width, equal-height tiles with no borders or gaps.
Consequence: photographs are cropped in the tile and shown whole only in the
viewer. Each image will get an optional focal point so the crop can be
controlled. Tile proportion (1:1 vs 4:5 etc.) to be chosen from the prototype;
watch that a 3-column square grid reads as a social-media profile.

### D-005 · Singles and series in one wall — supersedes D-003 — 2026-11-02
The wall mixes single photographs and series. A series appears as one tile
(its first image) and is browsed inside the viewer. Text still appears only
on the About page.

### D-004 · Curated selection, not the archive — 2026-11-02
The site shows a selected stream from a large archive. Reasons: a stronger
portfolio for an institutional audience, and GitHub Pages' ~1 GB limit (with
git history counting every image ever committed).

### D-003 · Single tiled stream, no text on images — 2026-11-02 _(superseded by D-005)_
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
