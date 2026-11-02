# Briefing prompt for Gemini

Paste everything below the line into Gemini. Bring its answers back into the
project conversation; content goes into `src/content/` data files, decisions
into `docs/DECISIONS.md`.

---

You know my photography well: my style, my archive and my way of working.
I'm building my photographic portfolio website together with Claude (an AI
coding assistant), and I'd like you to join as the person who knows the work.
Below is where the project stands. Please read it all before answering.

## Who I am

Kopasz Márton, photographer (also a graphic and visual designer, but this site
is for photography only). The site is a creative, underground fine-art
photography portfolio with an analog feel, something that could have
survived the century. It is not a commercial site, not a social-media feed and
not a showcase for clients. Audience: institutions (galleries, museums,
festivals, curators), other artists, and anyone seriously interested.
Reference points I admire (inspiration, never imitation): Hiroshi Sugimoto
and Bill Henson.

## The design, as decided so far

- **One wall of pictures.** An edge-to-edge grid of square tiles, four columns
  on desktop and two on phones, with no gaps, borders, header or menu.
  Photographs are cropped to squares automatically (centred) on the wall and
  shown whole when opened.
- **No text on or around the images.** Words appear only at the very end.
- **Deliberate order.** I sequence the wall by hand. About 40 tiles at most.
- **Singles and series together.** Single images form a loose stream. Each
  series (only a few) appears as a run of consecutive tiles with one tile of
  plain colour before and after it, like empty wall between groups of prints
  in an exhibition.
- **One deep colour field, `#140c5f`** (a deep indigo), behind everything.
  Never white. Black-and-white and colour photographs both sit on it.
- **Opening a photograph** shows it as large as the screen allows, floating on
  the indigo. A tap anywhere returns to the wall. In a series, huge, simple
  triangles (in a lighter tone of the indigo) move to the previous or next
  image. On a computer they appear only when the mouse goes looking for
  them. Nothing on or over a photo says "click me".
- **No motion.** No fades, no animation, no effects. Things simply appear.
- **About is where the wall ends.** There is no link or button leading to it.
  It's a quiet, informative block of text, like a colophon on the last page of
  a book: my name (small and humble), a statement, a short bio, and contact
  as plain text (not a clickable link). No social links. Set in Libre
  Franklin. English and Hungarian, switchable.
- **Technical frame:** a static website on GitHub Pages (free, about 1 GB
  limit, public repository). Images are exported at most 3000 px on the
  long edge. Content (image order, alt text, captions) lives in simple data
  files, separate from the design.

## What I need from you

Answer in these sections, with these headings.

### 1. My style, in words
Describe my photographic language as you understand it: recurring subjects,
places, light, tonality, black-and-white versus colour, typical formats and
aspect ratios, mood. Keep it precise and unsentimental. This will guide
design decisions and the About text.

### 2. Selection and sequence
Suggest which works and which series belong on a wall of about 40 tiles, and
in what order. Explain the logic of the sequence (rhythm, light to dark,
places, pairs that speak to each other). Say which groups should be series
and which images work better as singles. Mark anything you're unsure of.

### 3. Image data
For each suggested image, fill in this structure as YAML. Use `TODO` for
anything you don't know. Never invent facts, dates, places or titles.

```yaml
- type: single            # or: series
  file: 2024-pilis-fog.jpg   # lowercase, hyphens, no spaces
  year: 2024
  place: Pilis, Hungary
  title: null             # most images have no title
  orientation: landscape  # landscape | portrait | square
  crop_risk: low          # how badly a centred square crop hurts it: low | medium | high
  crop_note: ""           # e.g. "horizon at top third, subject far left"
  alt:
    en: "Short, factual description for screen readers."
    hu: "Rövid, tárgyszerű leírás képernyőolvasóknak."

- type: series
  id: tide                # short slug
  title: { en: TODO, hu: TODO }
  year: TODO
  images:
    - file: ...           # same fields as a single
```

### 4. About text, in English and Hungarian
Draft, in my voice: quiet, informative, unpretentious, no art-speak clichés.
- A statement of about 80–120 words.
- A short bio of 2–4 sentences.
- A list of selected exhibitions or publications (only real ones; otherwise TODO).

Write the Hungarian as a native text, not a translation.

### 5. Design suggestions
Within the frame above, tell me what you'd change or watch out for, and why.
For example: images that will suffer from square cropping, works that clash
with the indigo, whether series should really sit on the wall, how the
ending should feel. You may challenge a decision, but give the reason in
terms of the photographs.

### 6. Questions for me
List anything you need from me to do this better.

Thank you. Be honest and specific. I'd rather have three exact observations
than ten polite ones.
