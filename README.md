# JHIDE — Animated Leather Goods Website

A front-end prototype for a handmade leather goods brand. Built as a single
self-contained HTML file: no build step, no dependencies, no server required.
Open `index.html` in any browser.

**Live demo:** https://jhide10.github.io/jhide-leather-website/

---

## What it demonstrates

Four scroll-driven moments, built with plain CSS and the Intersection Observer
API — no animation library:

1. **Preloader → hero** — wordmark and progress bar, then headline lines rise
   into place under an overflow mask, floating product cards, and a rotating
   circular badge drawn with SVG `textPath`.
2. **Marquee band** — seamless infinite scroll of craft terms; pauses on hover.
3. **The Making** — a scroll-pinned section. The viewport locks while four
   production stages advance: each stage cross-fades its own photograph, the
   copy slides in, and a progress rail fills. Driven by scroll ratio against a
   `400svh` container with a `position: sticky` inner panel.
4. **Featured collection** — horizontal scroller with scroll-snap, arrow
   buttons, pointer-drag, and a progress rail.

Plus: header inverts automatically over dark sections, numbers count up on
first view, section reveals stagger on scroll, reading-progress bar.

## Design

Monochrome interface — near-black `#0A0A0A`, white, greys. No accent colour and
no gradients anywhere; texture comes from flat fills and dashed stitch borders.

Photography carries the colour instead of the UI:

| Class  | Behaviour |
|--------|-----------|
| `tint` | Full colour, always — hero pair and the material close-up |
| `mono` | Black and white; turns full colour on hover, and automatically on the active process step while scrolling |

Swapping one class for the other on any `<img>` changes that photo's treatment.

## Structure

```
index.html                            the whole site
images/                               photography + swap instructions
versions/index-v1.1-monochrome.html   earlier fully black-and-white version
```

## Technical notes

- Single file, ~40 KB before images. Works offline; webfonts (Fraunces, Inter)
  load from Google Fonts with full system fallbacks.
- Responsive from 390px up. Below 1000px the pinned section unpins into a
  stacked layout and the photos light up per step via Intersection Observer.
- `prefers-reduced-motion` is honoured: pinning, reveals and marquees are
  disabled and the page renders as static content.
- No horizontal overflow at any tested width.

## Status

Prototype for client presentation. Photography is placeholder/reference
imagery, not final product photography, and the copy is illustrative.

## Licence

Code is free to reference. The photographs are placeholders and are not
licensed for redistribution.
