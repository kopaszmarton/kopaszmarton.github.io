# Roadmap

Each phase ends with something reviewable. Tick items as they land on `main`.

## Phase 0 — Philosophy & brief
- [x] Initial conversation: purpose, audience, structure
- [x] `CLAUDE.md`, `docs/BRIEF.md`, `docs/DECISIONS.md`, this roadmap
- [ ] Owner reviews and corrects the brief

## Phase 1 — Content model
- [ ] Resolve open questions 5–8 in the brief (launch size, order, About, language)
- [ ] Define the image data format (file, alt, optional title/place/year, order)
- [ ] Define the image preparation workflow (export settings from Lightroom/Capture One etc.)

## Phase 2 — Design direction
- [ ] Resolve open questions 1–4 (tiling, image view, background, identity)
- [ ] 2–3 clickable prototypes with real photographs
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
