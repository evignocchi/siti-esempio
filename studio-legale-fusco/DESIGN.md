---
name: Studio Legale Fusco
description: A sheet of carta uso bollo; ruled lines, a red double margin, one violet stamp.
colors:
  carta: "#f8f8f4"
  desk: "#e9ebe6"
  riga: "#c9d4e0"
  margine: "#cf4a3f"
  inchiostro: "#172030"
  testo-2: "#465065"
  grafite: "#626b7d"
  numerale: "#9aa4b3"
  viola: "#56399a"
  viola-deep: "#432a7d"
  viola-velo: "rgb(86 57 154 / .09)"
  marca-carta: "#fbf4e6"
  marca-verde: "#3d7a5c"
  marca-rosa: "#c96d86"
typography:
  display:
    fontFamily: "Libre Caslon Display, Georgia, serif"
    fontSize: "clamp(40px, 4.6vw, 66px)"
    fontWeight: 400
    lineHeight: "68px"
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Libre Caslon Display, Georgia, serif"
    fontSize: "clamp(36px, 4.2vw, 58px)"
    fontWeight: 400
    lineHeight: "68px"
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "Libre Caslon Text, Georgia, serif"
    fontSize: "clamp(26px, 2.7vw, 36px)"
    fontWeight: 400
    lineHeight: "68px"
  title:
    fontFamily: "Libre Caslon Text, Georgia, serif"
    fontSize: "21px"
    fontWeight: 700
    lineHeight: "34px"
  body:
    fontFamily: "Libre Caslon Text, Georgia, serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: "34px"
  label:
    fontFamily: "Archivo Narrow, sans-serif"
    fontSize: "13px"
    fontWeight: 600
    lineHeight: "34px"
    letterSpacing: "0.1em"
  nav:
    fontFamily: "Archivo Narrow, sans-serif"
    fontSize: "16px"
    fontWeight: 600
    letterSpacing: "0.04em"
  numeral:
    fontFamily: "Archivo Narrow, sans-serif"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: "34px"
    fontFeature: "\"tnum\""
rounded:
  none: "0px"
  hairline: "2px"
spacing:
  riga: "34px"
  riga-mobile: "32px"
  margine: "104px"
  margine-tablet: "64px"
  margine-mobile: "40px"
  gutter: "56px"
  sheet-inset: "48px"
components:
  button-primary:
    backgroundColor: "{colors.viola}"
    textColor: "{colors.carta}"
    typography: "{typography.nav}"
    rounded: "{rounded.hairline}"
    padding: "13px 20px"
  button-primary-hover:
    backgroundColor: "{colors.viola-deep}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.inchiostro}"
    typography: "{typography.nav}"
    rounded: "{rounded.hairline}"
    padding: "13px 20px"
  marca-da-bollo:
    backgroundColor: "{colors.marca-carta}"
    textColor: "{colors.marca-verde}"
    rounded: "{rounded.none}"
    padding: "16px"
    width: "236px"
  sheet:
    backgroundColor: "{colors.carta}"
    textColor: "{colors.inchiostro}"
    rounded: "{rounded.none}"
    padding: "75px 48px 61px 136px"
  form-panel:
    backgroundColor: "rgb(255 255 255 / .55)"
    textColor: "{colors.inchiostro}"
    rounded: "{rounded.none}"
    padding: "32.5px 28px"
  field-ruled:
    backgroundColor: "transparent"
    textColor: "{colors.inchiostro}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    height: "34px"
---

# Design System: Studio Legale Fusco

## Overview

**Creative North Star: "Il Foglio Uso Bollo"**

Every surface is a sheet of Italian protocol paper: off-white, ruled in faint blue at a fixed pitch, with a double red margin line on the left and small line numerals counted down the margin. Text is written onto the rules in a legal book serif, never floated over them. Sheets sit on a grey-green desk, one after another, each with its own folio in the top right corner. The single active colour is a violet stamp ink; everything that can be pressed, hovered or focused speaks in it, and nothing decorative does.

Density is calm and document-like: generous left margin, a two-column reading layout inside each sheet, plain words. Objects from the world of legal paperwork carry the interactive weight: the call control is a perforated marca da bollo with guilloche ground, the address is a round rubber stamp overlapping it, the portrait is clipped to the sheet with a paperclip. These objects are slightly rotated, as if placed by hand; the sheet itself is never rotated.

The confirmed visual rejection is the navy courtroom-photo hero with columns and scales of justice. The world answers sobriety with stationery, not with institutional iconography.

**Key Characteristics:**
- Ruled paper at a 34px pitch (32px on phones); every line of text lands on that rhythm.
- A double red margin line and right-aligned line numerals in the margin.
- One active ink, violet, for actions, focus, selection and highlights.
- Paperwork objects (marca da bollo, rubber stamp, paperclip) as the expressive components, slightly rotated.
- Book serif for reading, a narrow grotesque for labels, numerals and controls.

## Colors

Paper, ink and one violet stamp; the marca da bollo carries its own small multi-tint print palette.

### Primary
- **Timbro Violet** (viola): the stamp ink. Rubber stamp, primary button, focus outline, text selection, the lit margin numeral, and (as Violet Veil, viola-velo) the wash behind a hovered problem line or practice area.
- **Pressed Violet** (viola-deep): hover state of the filled button only.

### Secondary
- **Margin Red** (margine): the two vertical margin lines of every sheet. Structural, never used for text or controls.

### Tertiary
- **Marca Paper** (marca-carta): ground of the revenue-stamp control.
- **Marca Green** (marca-verde): the stamp's frame, value line and horizontal guilloche.
- **Marca Rose** (marca-rosa): the stamp's vertical guilloche. Both tints live only inside the marca da bollo.

### Neutral
- **Protocol Paper** (carta): sheet ground and the colour of the perforation holes.
- **Desk** (desk): page background between sheets.
- **Rule Blue** (riga): the horizontal rules, also drawn inside the textarea.
- **Blue-Black Ink** (inchiostro): headings, body, links, outline button border, underlined fields.
- **Second Ink** (testo-2): supporting paragraphs, captions, label text, icon strokes.
- **Graphite** (grafite): sheet folio and problem-line keys.
- **Margin Numeral** (numerale): line numbers in the margin; ornamental and hidden from assistive tech.

### Named Rules
**The One Stamp Rule.** Violet is the only active ink. If an element does not act, respond to a pointer, or show focus, it is not violet. There is exactly one rubber stamp per page.

**The Marca Palette Stays in the Marca Rule.** Green and rose exist only inside the marca da bollo; they never leak into buttons, links or headings.

**The Numeral Is Ornament Rule.** Margin Numeral is too faint for words; use it only for the aria-hidden line numbers. Any readable label uses Graphite or Second Ink.

## Typography

**Display Font:** Libre Caslon Display (with Georgia, serif)
**Body Font:** Libre Caslon Text (with Georgia, serif)
**Label/Mono Font:** Archivo Narrow (500/600/700)

**Character:** A legal book serif written on the rules, paired with a narrow grotesque that reads like a printed form field: the serif speaks to the client, the grotesque labels, counts and controls.

### Hierarchy
- **Display** (400, clamp(40px, 4.6vw, 66px), two rules tall): the studio name on line 1 of the first sheet only.
- **Headline** (400, clamp(36px, 4.2vw, 58px), two rules tall): one section title per sheet.
- **Lead** (Caslon Text 400, clamp(26px, 2.7vw, 36px), two rules per line, balanced wrap, max 21em): the opening statement; italic for the plain-words phrase. One rule per line on phones at 24px.
- **Title** (Caslon Text 700, 21–22px, one rule): practice-area and form headings.
- **Body** (Caslon Text 400, 18px, one rule; 17px on phones): all reading text. Italic for notes, captions and the deontological line.
- **Label** (Archivo Narrow 600, 13px, 0.06–0.1em tracking, uppercase for field and term labels): definition terms, form labels, timeline keys, the sheet folio.
- **Nav / Control** (Archivo Narrow 600–700, 16px, 0.04–0.06em): menu links and buttons; buttons uppercase.
- **Numeral** (Archivo Narrow 500, 12px, tabular): margin line numbers; 10px on phones.

### Named Rules
**The On-the-Rule Rule.** Every line-height is the rule pitch or a whole multiple of it (34px, 68px, 102px). Display sizes take two rules; nothing sits between lines.

**The Serif Speaks, the Narrow Labels Rule.** Sentences addressed to the client are always Caslon; Archivo Narrow never carries a full sentence.

## Layout

Each section is a full sheet: a centred column min(1180px, 100% − 32px) wide on the desk, separated from the next sheet by one rule (34px). The sheet's rules start two rules down; content is padded to begin on a rule, with a 104px margin column plus 32px before the text and 48px on the right. The margin numerals are counted by script to match the sheet height.

Inside a sheet the grid is two columns with a 56px gutter: opening statement and problem list beside a 300px contact column; section heading beside its intro; practice areas as a two-column legend; contacts beside the form. The biography uses three columns (200px portrait, story, credentials) with a 48px gutter.

Vertical spacing is only ever in rules: margins of one, one and a half, two or three rules. Horizontal spacing uses 12, 14, 16, 24, 28, 32, 48 and 56px.

Responsive: at 980px the margin narrows to 64px and every grid collapses to one column, with the marca da bollo moving below the problem list. At 560px the margin is 40px, the rule pitch drops to 32px, body to 17px, and the problem-line keys hide.

## Elevation & Depth

Mostly flat paper. Depth comes from stacked physical objects, each with a soft, low, downward-bleeding shadow as if lying on the desk; there are no hard or offset shadows and no shadow on hover except the marca lifting 3px.

### Shadow Vocabulary
- **Sheet on desk** (`box-shadow: 0 1px 0 rgb(0 0 0 / .04), 0 24px 40px -32px rgb(20 30 40 / .35)`): every sheet.
- **Object on sheet** (`box-shadow: 0 8px 14px -10px rgb(30 30 40 / .35)`): the marca da bollo; the portrait print uses the same shape at 16px / .5.

### Named Rules
**The Placed-by-Hand Rule.** Objects on the sheet (stamp, revenue stamp, portrait) may rotate between −12° and +2.2°; the sheet, its text and its controls never rotate.

## Shapes

Square paper geometry. Sheets, panels, fields and the marca are square-cornered (0); buttons and highlight washes take a hairline 2px. Curvature belongs to the world's objects: the round stamp with circular text, the perforated marca edge (4.5px holes at a 12px pitch, punched in paper colour), the paperclip. Borders are 1–1.5px solid ink or violet; fields are a single bottom rule rather than a box.

## Components

### Buttons
Printed-form controls: narrow uppercase, hairline corners, clear outline.
- **Shape:** near-square (2px), 1.5px border.
- **Primary:** violet fill, white text, 13px 20px, inline 18px SVG icon at 10px gap.
- **Hover / Focus:** fill deepens to Pressed Violet over .2s; focus is a 2px violet outline at 3px offset.
- **Outline:** transparent with an ink border and ink text; hover adds a 6% ink wash.

### Marca da Bollo (signature component)
The primary call control is a revenue stamp: Marca Paper ground with punched perforations on all four edges, an inner green-framed vignette with fine green and rose guilloche, the value line ("Prima consulenza") in tracked green caps, the phone number at 30px bold tabular, the action in caps, and the address in Caslon italic. Rotated +1.6° at rest; on hover it straightens and lifts 3px (.35s, cubic-bezier(.16,1,.3,1)).

### Timbro (signature component)
The round violet rubber stamp: three concentric rings, the studio name and address set on a circular path in Archivo Narrow caps, the lawyer's name in Caslon at the centre, roughened by an SVG turbulence filter, multiplied onto the paper at .86 opacity and rotated −12°. It overlaps the marca. When the marca is hovered or focused it presses: scale down to .95, ink fully opaque with a slight blur, then settles at 1.02 (.55s).

### Problem Lines and Legend
Problems are plain-words links, one per rule, each keyed by a short Graphite label. Hovering or focusing a line washes it in Violet Veil, lights its margin numeral in bold violet, and lights the matching practice area in the legend. Practice areas are title, paragraph and a dot-separated row of narrow sub-topics; hovering one lights it and its numeral the same way.

### Inputs / Fields
- **Style:** no box; select is underlined by a 1px ink rule; textarea is transparent and ruled with Rule Blue at the pitch, so the client writes on lines.
- **Focus:** 2px violet outline at 2px offset.
- **Labels:** uppercase Label style, Second Ink.

### Cards / Containers
- **Form panel:** square, 1px ink border, translucent white over the rules, padded to keep its text on the rule.
- **Sheet:** see Layout; carries its folio ("Foglio n di N") top right in Graphite caps.

### Navigation
Three Archivo Narrow links on line 1 of the first sheet, ink colour, no underline at rest; hover draws a 1px ink underline as a bottom border. Wraps beneath the studio name on narrow screens.

## Do's and Don'ts

### Do:
- **Do** set every line on the rule pitch (34px, 32px under 560px) and give display type exactly two rules.
- **Do** keep violet for what acts: buttons, focus, selection, lit numerals, hover veils, the one stamp.
- **Do** express new interactive emphasis as a paperwork object (stamp, marca, clip, tab) before reaching for a generic card.
- **Do** keep icons as inline stroked SVG at 18px, coloured in Second Ink or inheriting the control colour.
- **Do** honour reduced motion: transitions and the stamp press both stop.

### Don't:
- **Don't** use the navy courtroom-photo hero, classical columns or scales of justice.
- **Don't** add a second stamp, a second accent hue, or use the marca's green and rose outside the marca.
- **Don't** rotate the sheet, body text or buttons; only placed objects tilt.
- **Don't** use hard or offset shadows, or round the sheet, panels or fields.
- **Don't** set readable text in Margin Numeral.
