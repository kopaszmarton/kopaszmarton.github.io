# CLAUDE.md — project memory

Read this file first in every session. It is the single source of truth for
*what* this site is and *how* we work on it. If a request conflicts with this
file, raise it with the owner before acting — then update this file.

## What this is

The photographic portfolio of Márton Kopasz, published at
`https://kopaszmarton.github.io` via GitHub Pages.
Photography only — no graphic or visual design work appears here.

Full brief: `docs/BRIEF.md` · Decisions: `docs/DECISIONS.md` · Plan: `docs/ROADMAP.md`

## Philosophy (design follows this, never the reverse)

- **The images are the site.** Everything else exists to get out of their way.
- **A single stream.** One continuous tiled field of photographs — not
  categories, not projects, not a blog.
- **No text on or around the images.** Words live on the About page only.
- **Serious, restrained, wild.** The interface is quiet and exact so the
  atmosphere of the photographs can be loud.
- **No effects for their own sake.** No parallax, no hover gimmicks, no
  loading spinners, no autoplay. Motion only when it aids viewing.

## Hard constraints (GitHub Pages)

- Static output only: HTML, CSS, minimal JS. No PHP, no server, no database.
- Published site ≤ 1 GB; repo should stay < 1 GB. Git history keeps every
  file ever committed — deleting an image does NOT free space.
- The repo is public: every committed file is downloadable.
  **Never commit original/full-resolution files.** Commit web masters only
  (see image rules below).
- No server-side forms. Contact = email link (or an external form service).

## Conventions

- **Content is separate from design.** Image order and metadata live in data
  files under `src/content/`; layout lives in templates/components. Adding a
  photo must never require touching layout code, and vice versa.
- **Design tokens in one place** (type, spacing, colours, grid). No magic
  numbers scattered through components.
- **Small, reviewable changes.** One concern per branch / pull request.
  `main` is always the live site.
- **Record decisions.** Any choice that shapes the site gets an entry in
  `docs/DECISIONS.md` (what, why, date). Change a decision by superseding it,
  not by quietly working around it.
- **Accessibility is not optional.** Every image has meaningful `alt` text in
  its data file, even though no text is shown visually. Keyboard navigation
  must work everywhere.

## Image rules

- Web master: long edge 3000 px max, sRGB, high-quality JPEG, metadata
  stripped except copyright.
- Target ≤ ~1.5 MB per master; responsive sizes/formats are generated at
  build time, not committed.
- Filenames: lowercase, hyphenated, no spaces (e.g. `2024-pilis-fog.jpg`).
- Curate before committing — the repo is not a scratch space.

## Stack (planned — see DECISIONS.md)

Astro static site, built and deployed by a GitHub Actions workflow.
Content editing initially by editing data files; a git-based CMS
(Pages CMS or Sveltia CMS) to be added once the structure settles.
