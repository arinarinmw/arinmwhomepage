---
name: arinmw.com homepage (The Warm Room)
description: Arin's profile as one small isometric room, in warm beige and brown: quiet, mature, minimal.
colors:
  ground: "#f4ede3"
  panel: "#fcf9f3"
  edge: "#e4d8c6"
  sand: "#d8c7ad"
  ink: "#3a2a20"
  ink-soft: "#6a5646"
  line: "#7b6150"
  accent: "#7a4d32"
  accent-deep: "#5e3822"
  accent-hover: "#66402a"
  clay: "#ecd8c9"
  clay-deep: "#d9b9a2"
  oat: "#e9e0d1"
  oat-deep: "#d5c5ab"
  tan: "#f1e0c0"
  tan-deep: "#e4c999"
  sage: "#b4c4a0"
typography:
  display:
    fontFamily: "IBM Plex Sans Thai, Inter, sans-serif"
    fontSize: "clamp(28px, 3.5vw, 42px)"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.015em"
  body:
    fontFamily: "Inter, IBM Plex Sans Thai, Noto Sans Thai, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Inter, IBM Plex Sans Thai, Noto Sans Thai, sans-serif"
    fontSize: "14.5px"
    fontWeight: 400
    lineHeight: 1.3
rounded:
  chip: "12px"
  panel: "18px"
  card: "16px"
spacing:
  part-padding: "56px"
  chip-gap: "8px"
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.panel}"
    rounded: "{rounded.chip}"
  button-primary-hover:
    backgroundColor: "{colors.accent-hover}"
  chip:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.chip}"
  panel:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.panel}"
---

# Design System: arinmw.com homepage (The Warm Room)

Scope: `index.html` and `home.css`. The four course-student pages still use `site.css`. Earlier versions are kept in `.impeccable/versions/minihompy/` (pastel) and `.impeccable/versions/monument/` (name as a monument).

## Overview

**Creative North Star: "The Warm Room"**

The homepage is still Arin's profile as one tiny isometric room where every object is a section and a piece of real proof, now in a quiet, adult palette: oat walls, a sand-and-cream checker floor, walnut furniture with soft brown outlines. Around it the page is calm: a warm oat ground, cream panels, IBM Plex Sans Thai Medium for headings (a stand-in for Asangha Medium, which is a Canva font) and Inter Regular for everything else.

It keeps the charm of the room and drops the candy: no saturated pastels, no heavy outlines, no tile bands, no coloured icon bubbles.

**Key Characteristics:**
- One authored isometric SVG room as the hero; each object links to its section.
- Beige, cream, clay and brown only; sage appears just in the plant.
- IBM Plex Sans Thai Medium for headings (stand-in for Asangha Medium) and Inter Regular for text and controls.
- Hairline borders (1px), small radii, light shadows.
- Bilingual EN default, TH toggle; every text node exists in both languages.

## Colors

- **Oat Ground** (#f4ede3): page. **Cream Panel** (#fcf9f3): panels and chips. **Edge Sand** (#e4d8c6): borders. **Sand** (#d8c7ad): TV frames, scrollbar.
- **Espresso Ink** (#3a2a20): text and headings. **Soft Brown** (#6a5646): secondary text. **Outline Brown** (#7b6150): room outlines.
- **Walnut Action** (#7a4d32; hover #66402a; deep #5e3822 for text on light): the one action colour (email button, active toggle, focus).
- **Clay** (#ecd8c9 / #d9b9a2), **Oat** (#e9e0d1 / #d5c5ab), **Tan** (#f1e0c0 / #e4c999): object and note tints, never actions. **Sage** (#b4c4a0): the plant.

**The One Action Rule.** Walnut means "do something". Clay, oat and tan decorate objects.

## Typography

- **Display:** IBM Plex Sans Thai 500 (Latin and Thai; stand-in for Asangha Medium, a Canva font), tracking -0.015em: hero tagline, part headings, note titles.
- **Body and UI:** Inter 400 (IBM Plex Sans Thai for Thai glyphs): paragraphs, chips, buttons, captions. Body 17px, leading 1.65 (Thai 1.8).
- Thai tagline breaks only between phrases.

## Layout

Hero grid `minmax(0,1fr) minmax(0,560px) 262px`: profile and tagline, room, three small panels. At 1180px two columns; at 900px notes and shelf go single-column; at 760px one column and the room chips become icon-only. Parts are cream panels on the oat ground (56px padding stepping down at 1180/900/760/480). A floating "Back to the room" chip appears after the hero.

## Elevation & Depth

Barely there: `0 10px 24px rgba(58,42,32,.07), 0 1px 3px rgba(58,42,32,.05)` on panels; a smaller version on chips; the primary button carries `0 10px 20px rgba(122,77,50,.18)`. Objects in the room lift on hover.

## Shapes

Small radii: chips and buttons 12px, cards 16px, panels 18-20px. Sticky notes keep a folded corner; polaroids 2px with a sand tape strip; round shapes only for icon bubbles and the avatar.

## Components

- **Button:** walnut fill, cream text, 12px radius, soft shadow; secondary is a cream chip with a walnut outline.
- **Chips:** cream, 1px edge, 12px radius, Inter 14.5px.
- **Sticky notes:** tan, clay and oat-deep, folded corner, expandable.
- **Video frames:** sand TV frame around a photo thumbnail, click to load YouTube.
- **Plaques:** certificates in framed cream tiles with an inset sand border.
- **Language toggle:** two-segment, EN default, remembered, `?lang=` overrides.

## Do's and Don'ts

### Do:
- **Do** keep every object in the room linked to a real section and labelled.
- **Do** keep every text in both languages and the Thai name อรินจ์ หมวดทอง untranslated.
- **Do** state only true facts; counts come from content on the page.
- **Do** keep colour to beige, cream, clay and brown with one walnut action.

### Don't:
- **Don't** bring back violet, candy pastels, heavy 2-3px outlines or the checker tile bands.
- **Don't** add eyebrows, section numbers, hard shadows, bevels or cards inside cards.
- **Don't** invent numbers, testimonials, logos or counters.
