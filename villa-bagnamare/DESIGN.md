---
name: Villa Bagnamare e MorfeoCentro42
description: Holiday flats on Lipari, let directly by the owners; white pumice ground, black obsidian slabs, pumice-water turquoise.
colors:
  pumice: "#efeee9"
  pumice-shade: "#e6e4dd"
  pumice-stone: "#cfccc2"
  pumice-thread: "#bdb9ae"
  turquoise: "#21a3a3"
  turquoise-deep: "#0b5f63"
  turquoise-light: "#8fd6d1"
  turquoise-ink: "#032628"
  obsidian: "#0e1012"
  obsidian-raised: "#191d21"
  obsidian-sheen: "#20262b"
  obsidian-core: "#050607"
  ink: "#121416"
  ink-muted: "#4f4d47"
  slab-text: "#e9ecee"
  slab-muted: "#9aa5ad"
  slab-stroke: "#3c454c"
typography:
  display:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "clamp(34px, 7.4vw, 112px)"
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "clamp(38px, 5.4vw, 76px)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "clamp(30px, 3.4vw, 50px)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  title-small:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "28px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "-0.01em"
  numeral:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "44px"
    fontWeight: 700
    lineHeight: 0.9
    fontFeature: "tnum"
  body:
    fontFamily: "Hanken Grotesk, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Hanken Grotesk, sans-serif"
    fontSize: "13px"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "0.04em"
  label-cut:
    fontFamily: "Chakra Petch, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.04em"
  button:
    fontFamily: "Hanken Grotesk, sans-serif"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1
  caption:
    fontFamily: "Hanken Grotesk, sans-serif"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.4
rounded:
  control: "2px"
spacing:
  gutter: "16px"
  stack: "32px"
  column-gap: "56px"
  column-gap-wide: "64px"
  band: "72px"
  section: "112px"
components:
  button-primary:
    backgroundColor: "{colors.turquoise}"
    textColor: "{colors.obsidian}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 20px"
  button-primary-hover:
    backgroundColor: "{colors.turquoise-light}"
    textColor: "{colors.obsidian}"
  button-ghost-on-obsidian:
    backgroundColor: "transparent"
    textColor: "#ffffff"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 20px"
  button-ask:
    backgroundColor: "transparent"
    textColor: "{colors.obsidian}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "13px 16px"
  button-ask-hover:
    backgroundColor: "{colors.obsidian}"
    textColor: "#ffffff"
  input-slab:
    backgroundColor: "rgb(255 255 255 / .06)"
    textColor: "#ffffff"
    rounded: "{rounded.control}"
    padding: "12px"
  chip-distance:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "6px 10px"
  slab-form:
    backgroundColor: "{colors.obsidian}"
    textColor: "{colors.slab-text}"
    padding: "28px 30px 24px"
    width: "min(500px, 100%)"
  band-sea:
    backgroundColor: "{colors.turquoise}"
    textColor: "{colors.obsidian}"
    padding: "72px 0 88px"
  band-obsidian:
    backgroundColor: "{colors.obsidian}"
    textColor: "{colors.slab-text}"
    padding: "104px 0"
---

# Design System: Villa Bagnamare e MorfeoCentro42

## Overview

**Creative North Star: "Pumice and Obsidian"**

The system is built from Lipari's own two stones and the water between them. The ground is pumice: a chalky, warm off-white carrying a faint porous grain (an SVG fractal-noise tile at 16% opacity over the page background). Against it sit obsidian slabs: near-black, glossy, with a cold diagonal sheen and edges cut like conchoidal fracture instead of rounded. Turquoise, the colour of the sea over the pumice beds, never decorates. It either owns a whole band (the house on the sea) or marks the one action that sends a request.

Structure comes from one long horizontal line. A 1px obsidian rule runs edge to edge under the masthead, again between the two houses, and across the hero photograph, where it is measured to sit exactly on the sea horizon. Headings are cut, chamfered capitals (Chakra Petch); everything people read or type is a quiet grotesque (Hanken Grotesk). Photographs are shown untinted as plates on a 12-column grid, each with a caption line underneath naming the place and the flat.

Density is generous and editorial: large uppercase headings, wide bands (72 to 120px vertical), apartments laid out as ruled rows rather than cards. The form is a working instrument, not a teaser, and it lives in the first viewport.

**Key Characteristics:**
- Pumice ground with porous grain; obsidian slabs with a gradient sheen; turquoise in whole bands or on the primary action only.
- One long 1px horizon line as the page's structural rule.
- Faceted clip-path corners on obsidian panels; 2px corners on controls; nothing pill-shaped or soft.
- Chakra Petch uppercase for names, headings and numerals; Hanken Grotesk for body, labels and controls.
- Untinted photo plates with a caption line below.
- Apartments as ruled rows with a large guest-count numeral, never a grid of equal cards.

## Colors

Two stones and one water: a warm mineral white, a cold glassy black, and a single saturated turquoise with a deep and a light step.

### Primary
- **Pumice-Water Turquoise** (`turquoise`): the field of the Villa Bagnamare band and the fill of the primary "Invia su WhatsApp" / "Chiedi per tutti e due" buttons. It is also the text accent inside obsidian ("Chiedici tutto.") and the selection colour. Obsidian text sits on it, never white.
- **Deep Lagoon** (`turquoise-deep`): links and focus outlines on pumice, and the Morfeo subtitle under the main title. This is the turquoise that is legible as text on the light ground.
- **Shallow Water** (`turquoise-light`): hover fill for the primary button, focus border on obsidian fields, and the live summary line inside the slab.
- **Lagoon Ink** (`turquoise-ink`): body text, list text and captions inside the turquoise band, where pure obsidian would be too heavy for running copy.

### Neutral
- **Pumice** (`pumice`): page ground, always with the porous grain.
- **Pumice Shade** (`pumice-shade`): footer ground.
- **Pumice Stone** (`pumice-stone`): row rules and chip borders on pumice.
- **Pumice Thread** (`pumice-thread`): the hairline above the footer's registration codes.
- **Obsidian** (`obsidian`): the horizon line, row rules, slab mid-tone, the "Siamo eoliani" band, the outline of the per-flat ask button.
- **Obsidian Raised** (`obsidian-raised`): photo placeholder behind plates and the option list inside slab selects.
- **Obsidian Sheen / Obsidian Core** (`obsidian-sheen`, `obsidian-core`): the two ends of the 160deg slab gradient (sheen at 0%, obsidian at 46 to 50%, core at 100%).
- **Ink** (`ink`): body text on pumice. **Ink Muted** (`ink-muted`): secondary copy, captions and footer text on pumice.
- **Slab Text / Slab Muted / Slab Stroke** (`slab-text`, `slab-muted`, `slab-stroke`): text, secondary text and 1px field borders on obsidian surfaces.

### Named Rules
**The Whole-Band Rule.** Turquoise appears as a full-width band or as the fill of the single primary action. It is never used for small decorative accents, borders or icons on pumice.

**The Deep-on-Light Rule.** On pumice, turquoise text is always `turquoise-deep`. Plain `turquoise` as text appears only on obsidian.

**The Untinted Plate Rule.** Photographs are never colour-graded, duotoned or overlaid with brand colour. The only overlays permitted are the horizon line and a caption with a soft text-shadow.

## Typography

**Display Font:** Chakra Petch (with sans-serif fallback), weights 500 to 700
**Body Font:** Hanken Grotesk (with system-ui, sans-serif), weights 400 to 700

**Character:** Chakra Petch's chamfered corners and cut terminals echo the faceted slabs, and set in uppercase they read as stone that has been cut. Hanken Grotesk stays out of the way, warm and humanist enough for hospitality copy.

### Hierarchy
- **Display** (700, clamp(34px, 7.4vw, 112px), 0.9, uppercase): the property name in the masthead only. Held on one line above 640px.
- **Headline** (700, clamp(38px, 5.4vw, 76px), 0.95, uppercase): section headings ("Siamo eoliani", "Come arrivare"). The houses intro runs one step larger (clamp(40px, 6vw, 84px)). Below 640px, clamp(30px, 9.4vw, 44px).
- **Title** (700, clamp(30px, 3.4vw, 50px), uppercase): house names inside their bands. **Title small** (700, 28px, uppercase): flat names in rows. The slab heading is 30px, 700, mixed case.
- **Numeral** (700, 44px, 0.9, tabular): guest capacity per flat. The owners' phone numbers use the same face at 24px.
- **Body** (400, 17px, 1.6; 16px below 640px): running copy, held to 32 to 38em.
- **Label** (600, 13px, 0.04em): form labels in the slab. **Label cut** (Chakra Petch 700, 14 to 15px, 0.04 to 0.06em, uppercase): row labels in the travel list and footer column heads.
- **Button** (Hanken Grotesk 700, 15 to 16px, line-height 1): all buttons.
- **Caption** (400, 13px): plate captions and the hero credit.

### Named Rules
**The Cut Caps Rule.** Chakra Petch carries names, headings, numerals and short row labels, almost always in uppercase with tight negative tracking at large sizes. It never sets paragraphs, form fields or button labels.

**The Quiet Reader Rule.** Everything that is read in sentences or typed into is Hanken Grotesk.

## Layout

A single centred container (`min(1240px, 100% - 32px)`) holds content. Bands break out of it to full bleed: the turquoise sea band, the obsidian band, the footer. The horizon rule always runs full width.

The masthead is a two-column grid: the property name (auto width) and a short location statement aligned to the baseline. Below the horizon, the hero photograph runs full bleed (clamp(560px, 74vh, 780px) high; 52vh with a 320px minimum on mobile). Above 1000px the obsidian slab is absolutely placed over the photograph's top-right, aligned to the container edge. At 1000px and below it overlaps the photo's bottom edge by 140px (72px on mobile) and takes full width on phones.

House sections use a 5/7 split (name and address beside description and distance chips), then a 12-column plate grid with 16px gaps. Plates span 7+5, 6+6, 4+8 or 5+7, with aspect ratios set per span (4:3, 5:6, 3:2, 4:5, 16:10, 5:4). Flats are ruled rows on a four-column grid (name and type, numeral, features list, ask button). Each row is separated by a 1px rule and the list is topped by an obsidian rule.

Spacing rhythm: a 16px gutter and plate gap, 32px stack gaps, 56 to 64px column gaps, 72/88px band padding (56/64px on mobile), and 104 to 120px between major sections (72 to 80px on mobile). Breakpoints are 1000px (multi-column splits collapse to one column; plates go full span except the narrow 4-span, which becomes 6) and 640px (single column throughout, buttons full width).

## Elevation & Depth

Depth is material rather than layered UI. Pumice is flat, and its only texture is the grain. Obsidian conveys depth through its own gloss: a 160deg linear gradient from sheen to core, plus, on the form slab, a radial highlight (420 x 260px, `rgb(170 190 205 / .16)`) that follows the pointer through `--x`/`--y`. Shadows are soft, long and dark, and only used where an obsidian object physically overlaps something.

### Shadow Vocabulary
- **Slab drop** (`box-shadow: 0 30px 60px -30px rgb(0 0 0 / .6)`): the form slab where it sits over the photograph.
- **Notice lift** (`box-shadow: 0 12px 30px -10px rgb(0 0 0 / .5)`): the fixed bottom notice.
- **Caption lift** (`text-shadow: 0 1px 6px rgb(0 0 0 / .55)`): white captions laid on photographs.
- **Horizon glint** (`box-shadow: 0 1px 0 rgb(255 255 255 / .25)`): the 1px light edge under the horizon line on the photo.

### Named Rules
**The Gloss-Not-Lift Rule.** Obsidian surfaces read as deep because of their gradient sheen, not because they float. Only the overlapping slab and the transient notice cast shadows.

## Shapes

Two corner languages, one for each stone. Obsidian panels are cut, never rounded: clip-path polygons take one or two chamfers off opposite corners. The form slab loses its top-left (7% x 3.5%) and bottom-right (5% x 12%) corners; on mobile only a shallow top-left facet remains. The "Siete in tanti?" panel loses its bottom-left. The owner phone tiles lose their bottom-right. Controls, chips, the notice and buttons get a near-square 2px radius. Rules are 1px hairlines. Feature lists use a 7px x 1px dash as a bullet, not a dot.

**The Conchoidal Edge Rule.** Any obsidian panel gets at least one chamfered corner via clip-path and no border-radius. Anything on pumice or turquoise stays rectilinear at 2px.

## Components

### Buttons
Firm and plain: square-ish blocks with a label and, where it names a channel, a 20px inline SVG icon.
- **Shape:** near-square corners (2px).
- **Primary (turquoise):** turquoise fill, obsidian label, 15px 20px padding, 16px/700 Hanken Grotesk. It grows to fill the row in the slab. Hover moves the fill to Shallow Water over 0.2s.
- **Ghost on obsidian:** transparent with a 1px `#56616a` border and white label. Hover turns the border white.
- **Ask per flat ("Chiedi per ..."):** transparent, 1px obsidian border, obsidian label, 13px 16px padding. Hover fills it with obsidian and turns the label white. Clicking selects that flat in the slab, scrolls the slab into view, plays a 0.7s settle (6px lift and return), and moves focus to the next empty field.
- **Focus:** 2px `turquoise-deep` outline offset 3px, site-wide.

### Chips
- **Style (distance chips):** 1px border in currentColor at reduced strength (`pumice-stone` on pumice, obsidian at 45% on turquoise), 2px corners, 6px 10px padding, 14px/600 text. Informational only, never interactive.

### Cards / Containers
There are no generic cards. Containers are either full-width bands (turquoise, obsidian, pumice shade) or obsidian slabs.
- **Corner Style:** chamfered by clip-path (see Shapes).
- **Background:** the 160deg obsidian gradient.
- **Shadow Strategy:** slab drop only when overlapping (see Elevation & Depth).
- **Internal Padding:** 28px 30px 24px for the form slab (28px 20px 24px on mobile), 40px for the group panel, 14px 22px for phone tiles.

### Inputs / Fields
- **Style:** on obsidian only. 6% white fill, 1px `slab-stroke` border, 2px corners, 12px padding, 16px/500 white text, `color-scheme: dark` for native pickers. Labels are 13px/600 above the field.
- **Hover:** border lightens to `#5d6870`.
- **Focus:** border becomes Shallow Water and the fill rises to 9% white. No outline ring.
- **Error:** border `#f08c7a`. The summary line under the fields switches to `#ffb4a6` for errors and `#ffd29a` for capacity warnings.
- **Stepper:** guests are set with a bordered stepper: 42 x 44px minus/plus buttons with 18px SVG strokes around a centred 18px/700 tabular count. A disabled step dims to `#56606a`.

### Navigation
- **Style:** a single masthead row. A cut-caps mark line ("Affitti diretti", 15px/700, 0.08em) sits over a Hanken owners line, with a flat list of four anchors on the right (15px/600, ink).
- **Hover:** a 1px obsidian underline via bottom border.
- **Mobile:** the list wraps under the mark at full width with an 18px gap. There is no hamburger.

### Availability Slab (signature)
The obsidian form panel that holds the whole request: arrival and departure dates, adult and child steppers, flat select (grouped by house), a live summary line ("n notti · n persone", plus a suggested flat or a capacity warning), primary WhatsApp and ghost email buttons, and the owners' direct phone numbers. The sheen follows the pointer. Every "Chiedi per ..." on the page fills it.

### Flat Row (signature)
A ruled row: the flat name in title-small caps with its type and size below; the guest-capacity numeral with a small qualifier; a dashed-bullet features list; and the ask button. At 1000px and below it becomes name plus numeral on one line, with the list and button stacked under them.

### Photo Plate (signature)
An untinted image in a fixed-aspect frame on the obsidian-raised placeholder, with a 13px caption line underneath. Place or flat sits left and a credit (e.g. "Ripresa con drone") sits right. Plates sit on the 12-column grid.

## Do's and Don'ts

### Do:
- **Do** keep the page ground pumice with its grain, and let turquoise own a whole band or the one primary action.
- **Do** run the 1px obsidian horizon line full width between major zones, and register it to the real horizon when it crosses a sea photograph.
- **Do** cut every obsidian panel with a clip-path chamfer and give it the 160deg sheen-to-core gradient.
- **Do** set names, headings and capacity numerals in Chakra Petch caps; set copy, labels and controls in Hanken Grotesk.
- **Do** present photographs untinted on the 12-column plate grid with a caption line naming the place or flat.
- **Do** list flats as ruled rows with the guest numeral prominent and an ask button that fills the slab.

### Don't:
- **Don't** set plain `turquoise` as text on pumice; use `turquoise-deep`.
- **Don't** round obsidian panels or soften controls beyond 2px.
- **Don't** tint, duotone or colour-overlay the photographs.
- **Don't** set paragraphs, field text or button labels in Chakra Petch.
- **Don't** add shadows to flat pumice or turquoise surfaces; depth belongs to obsidian.
