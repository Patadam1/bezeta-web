---
name: BEZETA Barberstudio
description: Street technique, classic finish. A head of hair being designed, in pure black and pure white.
colors:
  ink: "#000000"
  paper: "#ffffff"
typography:
  display:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.5rem, 5.2vw, 5.4rem)"
    fontWeight: 850
    lineHeight: 0.92
    letterSpacing: "-0.035em"
    fontVariation: "'wdth' 125"
  headline:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.6rem, 7vw, 6rem)"
    fontWeight: 850
    lineHeight: 0.92
    letterSpacing: "-0.035em"
    fontVariation: "'wdth' 125"
  title:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.7rem, 3.4vw, 3rem)"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.03em"
    fontVariation: "'wdth' 118"
  serif-echo:
    fontFamily: "Bodoni Moda, Didot, Bodoni 72, serif"
    fontSize: "1.04em"
    fontWeight: 500
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
    fontVariation: "'wdth' 100"
  button:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.02em"
    fontVariation: "'wdth' 112"
  label:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "13px"
    fontWeight: 600
    letterSpacing: "0.18em"
    fontVariation: "'wdth' 70"
rounded:
  none: "0px"
spacing:
  gutter: "clamp(16px, 4vw, 56px)"
  container: "1360px"
  section-top: "clamp(96px, 13vw, 190px)"
  section-bottom: "clamp(72px, 9vw, 140px)"
  head-gap: "clamp(40px, 6vw, 80px)"
  action-gap: "14px"
components:
  button-solid:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "54px"
  button-solid-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
  button-ghost:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    typography: "{typography.button}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "54px"
  button-ghost-hover:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
  button-nav:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0 18px"
    height: "44px"
  button-close:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0 34px"
    height: "64px"
  social-tile:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    size: "52px"
  hours-row-today:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    padding: "16px 14px"
---

# Design System: BEZETA Barberstudio

## Overview

**Creative North Star: "Las Rayas"**

The site is a head of hair being designed. Every surface is a dense field of fine white hair strokes on black, and every section is opened by a raya: a crisp white channel cut through the hair at the logo's slash angle (-39.3deg). Tone comes only from stroke density, the way a fade thins toward the neckline: thick on top, sparse below. Contrast is made optically by line frequency, never by mixing greys.

The type carries the monogram. Archivo set heavy and expanded (850, width 125) speaks with the weight of the B/Z mark; Archivo condensed caps do the small talk of labels and nav; Bodoni Moda appears only as a rare serif echo of the BEZETA wordmark, one word per statement at most. Surfaces are flat, square-cornered and outlined in 1.5px white. Motion is a cut: sequenced, numbered, timed in a fixed order, never scattered. On load the slash carves across the hero and the logo opens along it; on scroll each section's raya scrubs in; under the pointer the visitor carves temporary rayas that grow back.

The world refuses the category default of black-and-gold luxe photography plus three service cards.

**Key Characteristics:**
- Two colors only: pure black ink and pure white paper.
- Hair-stroke texture as the only source of tone.
- Rayas at -39.3deg, the logo's slash, open every section.
- Heavy expanded Archivo display; condensed caps labels; Bodoni as a single-word echo.
- Square corners, 1.5px white strokes, no shadows.
- Every cut is sequenced: one order, one ease.

## Colors

A strict two-ink world: everything is black or white, and grey exists only as an optical effect of hair density.

### Primary
- **Razor White** (`paper`): text, strokes, hair, rayas, solid button fill, the inverted "today" hours row, focus rings, selection, scrollbar thumb. White is the cut and the hair at once.

### Neutral
- **Chair Black** (`ink`): page ground, nav when solid, mobile booking bar, the black gutter (16px) that sits under each white raya channel, and ghost-button fills at rest.

### Named Rules
**The Two Inks Rule.** Every fill, text, border and stroke is either `#000` or `#fff`. No greys, no tints, no reduced-opacity text for hierarchy; hierarchy comes from size, width and weight. Transient opacity during motion (fade-ins, rayas growing back) is permitted because it resolves to one of the two inks.

**The Density Not Grey Rule.** When a surface needs tone, add or thin hair strokes (0.35 to 0.65px white curves, 4 to 12px long); never lay down a grey fill. The antialiased shimmer of fine strokes is the world's only grey.

**The Monochrome Photo Rule.** Photographs render in grayscale with a slight contrast lift (`grayscale(1) contrast(1.08)`) so they sit inside the two-ink world.

## Typography

**Display Font:** Archivo variable (with Helvetica Neue, Arial)
**Body Font:** Archivo variable at normal width
**Label Font:** Archivo condensed (width 70 to 80), uppercase
**Serif Echo:** Bodoni Moda (with Didot, Bodoni 72)

**Character:** One family stretched across its width axis does all the work: expanded and heavy it reads as the B/Z monogram, condensed and tracked it reads as the "BARBERSTUDIO" line. Bodoni is the wordmark's ghost, used for one word that names the classic half of the story.

### Hierarchy
- **Display** (850, width 125, clamp(2.5rem, 5.2vw, 5.4rem), 0.92): the hero headline; balanced wrapping. On mobile clamp(2.3rem, 10vw, 3.4rem).
- **Headline** (850, width 125, clamp(2.6rem, 7vw, 6rem), 0.92): section titles; sliced statements use clamp(2.4rem, 6.4vw, 6rem), the close clamp(3rem, 9vw, 6rem).
- **Title** (800, width 118, clamp(1.7rem, 3.4vw, 3rem), 1): service names in the menu list. The address uses the same voice at 800, width 115, clamp(1.6rem, 3vw, 2.5rem), 1.08.
- **Body** (400, 17px, 1.55): running copy at 34 to 46ch. Section intros and service descriptions narrow to width 90; studio paragraphs 18px; lede clamp(17px, 1.3vw, 19px).
- **Button** (700, width 112, 15px, 0.02em, uppercase): all button labels (13px in the nav, 16px in the close).
- **Label** (600, width 70 to 80, 13px, 0.14 to 0.18em, uppercase): nav links, inline "Reservar" links, hours day names (14px), figcaptions, the hero hint.

### Named Rules
**The One Serif Word Rule.** Bodoni Moda (500) sets a single word inside an Archivo statement, the word for the classic side ("Acabado", "clásico"). Never a whole line, never a heading on its own.

**The Width Axis Rule.** Hierarchy is set by Archivo's width axis as much as by size: expanded for statements, normal for reading, condensed for labels. Don't swap in a second sans.

## Layout

A single centred container (max 1360px) with a fluid gutter (clamp(16px, 4vw, 56px)). Sections breathe with large vertical padding (top clamp(96px, 13vw, 190px), bottom clamp(72px, 9vw, 140px)). Each banded section opens with a hair band (clamp(130px, 15vw, 210px) tall) carrying one to three parallel rayas, offset 13px apart, then a section head: headline left, a short intro paragraph aligned to its baseline on the right.

The hero is full-bleed and at least one small-viewport height: logo left at large scale (up to 560px), headline, lede and actions in the right column. Services are a ruled list (name, description, link) with a thin carved rule above each row, not cards. The gallery is a five-column staggered reel (even items drop clamp(40px, 7vw, 110px)) of 4:5 frames.

At 960px and below: one column, hero actions go full width, nav links and the nav button hide, the reel becomes a horizontal scroll-snap strip (items 72% wide), and a fixed bottom booking bar slides up after 60% of a viewport of scroll. Hair density and stroke length drop below 700px.

## Elevation & Depth

Completely flat. There are no shadows anywhere. Depth is made by the hair: text sits in a cleared parting where strokes thin out around the actual glyph boxes (a 64px soft falloff, 28px on mobile), and a raya reads as cut into the hair because each white channel rides on a 16px black gutter that erases the strokes beneath it. Layering is only ink over hair over ink.

### Named Rules
**The Cut Not Lift Rule.** Nothing floats. To separate an element, part the hair around it or carve beside it; never add a shadow, glow or blur at rest.

## Shapes

Square corners everywhere (0px). Edges are 1.5px white strokes on buttons and social tiles, 1px white rules for nav, footer, booking bar and hours rows. The signature shape is the raya: a straight line at -39.3deg, 2.5px white (1.5px when it carves a hairline rule) over a 16px black gutter, butt caps, led by a small white blade tip (12 x 4px) while it is cutting. Sliced statements are clipped along the same line and their halves part by 5px along the blade.

### Named Rules
**The Logo Angle Rule.** Every diagonal in the system is -39.3deg, the logo's slash: rayas, the button blade sweep, the hero hint tick. No other angle.

## Components

### Buttons
Blunt, uppercase, square; they cut rather than glow.
- **Shape:** square (0px), 1.5px white border, 54px tall, 26px side padding, 14px gap before an optional 18px arrow icon.
- **Solid:** white fill, black text. Primary action, always "Reservar".
- **Ghost:** transparent on black, white text. Secondary action.
- **Hover / Focus:** ghost buttons fill with a white blade that sweeps in along the slash angle (0.55s, ease-out) and the text turns black; solid buttons invert to black with white text. The arrow nudges 4px right. Active presses scale to 0.97. Focus is a 2px white outline offset 4px.
- **Sizes:** nav 44px / 18px padding / 13px; close 64px / 34px padding / 16px.
- **Pending:** when a link is not yet known, a dashed white border on black, no blade, default cursor, aria-disabled.

### Navigation
Fixed strip, 72px tall: B/Z mark (44 x 42px) left, condensed caps links (13px, 0.16em) right, solid Reservar button at the end. Transparent over the hero; turns solid black with a 1px white bottom rule after 40px of scroll. Link hover draws a 1.5px white underline from left. Below 960px links and button hide and the bottom booking bar takes over.

### Service List
Ruled rows (34px vertical padding): Title name, short description, condensed "Reservar" link with arrow. A 1.5px raya carves each row's top rule on scroll. Hovering a row slides its name 14px right.

### Hours Table
Tabular numerals, 1px white row rules, day names in condensed caps (14px), times right-aligned at 18px width 110. Today's row inverts to white with black text.

### Social Tiles
52px square, 1.5px white border, 22px stroked SVG icon; hover inverts to white.

### Gallery Frame
4:5, black ground, hair field placeholder with its own rayas that re-carve on hover; label-style caption bottom left.

### Mobile Booking Bar
Fixed bottom, black with a 1px white top rule, full-width solid button, respects the safe-area inset.

### Hair Field and Raya (signature)
Canvas fields of seeded white strokes whose density follows a profile per context (hero thins like a fade toward the neckline; bands swell in the middle). Rayas are SVG lines scrubbed by scroll; the hero cut draws on load in 1.1s, then the logo, headline, lede, actions and hint enter in fixed numbered order. In the hero the pointer carves black-and-white rayas that fade back over 2.6s. Reduced motion shows every cut complete and skips the sequence.

## Do's and Don'ts

### Do:
- **Do** use only `#000` and `#fff`; make tone with hair-stroke density.
- **Do** cut every diagonal at -39.3deg and seat every white raya on a 16px black gutter.
- **Do** open each new section with a hair band and a raya that scrubs in on scroll.
- **Do** sequence motion in a fixed numbered order with the one ease-out curve (`cubic-bezier(.16, 1, .3, 1)`).
- **Do** keep a solid "Reservar" within one tap on every viewport (nav button on desktop, bottom bar on mobile).
- **Do** clear the hair around real text lines so copy always reads on pure black.
- **Do** mark missing owner information visibly with the dashed pending treatment.

### Don't:
- **Don't** introduce greys, tints, gold or any third color, including semi-transparent white text for secondary copy.
- **Don't** round corners or add shadows, glows or blurs at rest.
- **Don't** set more than one Bodoni word in a statement, or use Bodoni for headings, labels or body.
- **Don't** use any diagonal angle other than the logo's slash.
- **Don't** scatter motion: no independent looping animations, parallax drift or random reveals.
- **Don't** fall back to the black-and-gold luxe hero photo plus three service cards.
