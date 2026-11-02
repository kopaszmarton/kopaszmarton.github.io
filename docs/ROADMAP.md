# Roadmap

Each phase ends with something reviewable. Tick items as they land on `main`.

## Phase 0 — Philosophy & brief
- [x] Initial conversation: purpose, audience, structure
- [x] `CLAUDE.md`, `docs/BRIEF.md`, `docs/DECISIONS.md`, this roadmap
- [x] Owner reviews and corrects the brief

## Phase 1 — Content model
- [ ] Resolve open questions 5–8 in the brief (launch size, order, About, language)
- [ ] Define the image data format (file, alt, optional title/place/year, order)
- [ ] Define the image preparation workflow (export settings from Lightroom/Capture One etc.)

## Phase 2 — Design direction
- [x] Resolve tiling, image view, background direction (D-006 – D-010)
- [x] Prototype v1 with placeholder images (`prototypes/stream-v1.html`)
- [x] Choose field colour, tile proportion, columns (D-011)
- [x] Prototype v2: About at the end of the wall, horizon entry, phone view
- [x] Settle phone columns, About entry, mark colour (D-014)
- [x] About as a quiet colophon at the end of the wall (D-015)
- [ ] Choose series representation, colour hex, typeface
- [ ] Prototype with real photographs (deferred by owner; placeholders are fine for now)
- [ ] Choose direction; fix design tokens (type, spacing, colour, grid)

## Phase 3 — Technical skeleton
- [ ] Astro project, GitHub Actions deploy to Pages
- [ ] Design tokens, base layout, content collection
- [ ] CI checks: build, links, image size limit
- [ ] Live with placeholders, hidden from search engines

## Phase 4 — Core build
- [ ] Tiled stream (responsive, lazy-loaded, correct proportions)
- [ ] Image view (keyboard + touch)
- [ ] About page
- [ ] Responsive image generation (AVIF/WebP/JPEG)

## Phase 5 — Admin
- [ ] Connect Pages CMS or Sveltia CMS
- [ ] Test: add / reorder / remove images from laptop and phone
- [ ] Write `docs/HOW-TO-ADD-IMAGES.md`

## Phase 6 — Refinement
- [ ] Performance & accessibility audit
- [ ] Open Graph / share previews, favicon, sitemap
- [ ] Privacy-friendly analytics (optional)
- [ ] Custom domain (optional)

## Phase 7 — Launch
- [ ] Final curation of the stream
- [ ] Remove search-engine block
- [ ] Announce
