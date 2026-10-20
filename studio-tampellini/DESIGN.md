---
name: Studio Tampellini
description: Amministrazioni condominiali a Bologna, presented as an open partitario ledger.
colors:
  inchiostro: "#23221e"
  blu: "#2b4c8c"
  blu-deep: "#1d3870"
  rosso: "#b3362e"
  carta: "#edf1e8"
  carta-2: "#e2e8db"
  colonna: "#a3c2a9"
  riga: "#d2dccf"
  testo-2: "#4c5047"
  placeholder: "#5f6459"
typography:
  display:
    fontFamily: "Sofia Sans Condensed, sans-serif"
    fontSize: "clamp(40px, 5.3vw, 74px)"
    fontWeight: 800
    lineHeight: 0.98
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Sofia Sans Condensed, sans-serif"
    fontSize: "clamp(32px, 3.6vw, 48px)"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Sofia Sans Condensed, sans-serif"
    fontSize: "22px"
    fontWeight: 800
    lineHeight: 1.15
    letterSpacing: "0.01em"
  body:
    fontFamily: "Sofia Sans, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
    fontFeature: "tnum"
  body-small:
    fontFamily: "Sofia Sans, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Sofia Sans Condensed, sans-serif"
    fontSize: "13px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.14em"
  code:
    fontFamily: "Sofia Sans Condensed, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: "0.06em"
rounded:
  none: "0px"
  hair: "2px"
spacing:
  cell-y: "14px"
  cell-x: "20px"
  opening: "40px"
  section-top: "56px"
  column-data: "150px"
  column-rif: "132px"
  column-saldo: "340px"
components:
  button-primary:
    backgroundColor: "{colors.blu}"
    textColor: "#ffffff"
    rounded: "{rounded.hair}"
    padding: "14px 18px"
    width: "100%"
  button-primary-hover:
    backgroundColor: "{colors.blu-deep}"
    textColor: "#ffffff"
  button-filo:
    backgroundColor: "transparent"
    textColor: "{colors.blu}"
    rounded: "{rounded.hair}"
    padding: "14px 18px"
  button-filo-hover:
    backgroundColor: "{colors.blu}"
    textColor: "#ffffff"
  button-filo-compact:
    padding: "10px 14px"
  input-ruled:
    backgroundColor: "transparent"
    textColor: "{colors.inchiostro}"
    rounded: "{rounded.none}"
    padding: "6px 2px"
  ledger-row:
    backgroundColor: "{colors.carta}"
    textColor: "{colors.inchiostro}"
    padding: "14px 20px"
  column-head:
    backgroundColor: "{colors.carta}"
    textColor: "{colors.blu}"
    typography: "{typography.label}"
    padding: "10px 20px"
  saldo-panel:
    backgroundColor: "rgb(255 255 255 / .55)"
    textColor: "{colors.inchiostro}"
---

# Design System: Studio Tampellini

## Overview

**Creative North Star: "The Open Ledger"**

The site is a single partitario page laid on a darker desk. A pale green-grey sheet carries fine green column rules for Data, Causale, Rif. and Saldo; a blue double rule marks the column head and the Saldo column; a red double rule closes every block, the way a bookkeeper rules off a total. Everything the studio does is an entry on that sheet: a row with a time in Data, a description in Causale, a short code in Rif., and, where there is one, an action or a count in Saldo.

Density is that of a working register: rows are compact, separated by hairlines, and read across. Type is a condensed grotesk set like printed ledger heads, with a plain sans for text and tabular figures everywhere. Colour is ink, blue and red on paper, used as a bookkeeper uses them: blue for structure and action, red only for closures, deadlines and errors.

The world rejects the beige office-photo hero with three icon cards. Imagery is limited to the studio's own logo; no stock photography.

**Key Characteristics:**
- Four fixed ledger columns carry the layout on desktop; rows, not cards, are the unit.
- Double rules as punctuation: blue for heads and the Saldo column, red for closing a block.
- Condensed uppercase heads with open tracking; tabular numerals throughout.
- Flat paper with one soft page shadow; no card elevation.
- Every listed item carries a code (ORD.01, CON.06, DOC.03).

## Colors

Ink, ruling blue and closing red on pale ledger paper; the palette is the stationery of a bookkeeper.

### Primary
- **Ruling Blue** (blu): the column-head rule, the Saldo column's double rule, column-head labels, Data-column times, roles, links, primary and outline buttons, focus outlines, the row ruler on hover, selection. Its deeper press (blu-deep) is the primary button's hover only.

### Secondary
- **Closing Red** (rosso): the double rule that closes a block (`.chiusa` rows and the Saldo total), the post-closing 180-day stretch on the timeline, the deadline date, and invalid-field underlines and error text. It never fills a button or a background.

### Neutral
- **Ledger Ink** (inchiostro): all primary text, the timeline frame, the "today" marker.
- **Ledger Paper** (carta): the register sheet itself and the sticky column head.
- **Desk Paper** (carta-2): the page behind the sheet and the section-head rows, which read as a slightly darker band on the sheet.
- **Column Green** (colonna): vertical column rules, the timeline month dividers, the top rule of the opening office list, the scrollbar thumb.
- **Row Hairline** (riga): the 1px rule beneath every row.
- **Faded Ink** (testo-2): secondary text, explanatory small lines, codes, field labels, footer.
- **Placeholder Ink** (placeholder): input placeholder text only.

### Named Rules
**The Bookkeeper's Pens Rule.** Blue rules and acts; red closes and warns; ink writes. A new surface uses red only for a closing rule, a deadline or an error.

**The Closing Rule.** Every block of rows ends with a 3px red double rule (`border-bottom: 3px double`), never a plain line or a spacer.

## Typography

**Display Font:** Sofia Sans Condensed (with sans-serif)
**Body Font:** Sofia Sans (with system-ui, sans-serif)

**Character:** The condensed face, heavy and tightly leaded, sets heads like the printed rubrics of a ledger; the plain Sofia Sans carries descriptions without competing. Tabular numerals are on at the body level so codes, postcodes, phone numbers and counts align in columns.

### Hierarchy
- **Display** (800, clamp(40px, 5.3vw, 74px), 0.98): the opening statement only; balanced wrapping; an emphasised phrase turns Ruling Blue without italics.
- **Headline** (800, clamp(32px, 3.6vw, 48px), 1): section-head rows.
- **Title** (800, 22px, 1.15): register titles and the timeline title; the Saldo heading runs larger (26px), person names smaller (20px), the logo name 26px at 700.
- **Body** (400, 17px, 1.55; 16px under 520px): entry descriptions at weight 500; section intros capped at 42em, the opening mission at 19px and 36em.
- **Body small** (400, 15px): the explanatory line under an entry, contact sub-lines, footer.
- **Label** (700, 13px, 0.14em, uppercase): column heads. The same condensed uppercase family at 12 to 15px with 0.03 to 0.12em tracking serves field labels, Data-column times, roles and page folios.
- **Code** (600, 14px, 0.06em): Rif. codes such as ORD.01 and DOC.03; register codes (ORD, OPE, CON) at 700, 0.1em, in blue.

### Named Rules
**The Printed Head Rule.** Anything that labels, times or codes is condensed, bold and tracked; anything that describes is Sofia Sans in sentence case.

**The Tabular Rule.** Figures are always tabular (`font-variant-numeric: tabular-nums`); never switch to proportional figures for a number in a column.

## Layout

The register is one centred sheet, `min(1240px, 100% - 32px)` wide, on the darker desk colour. A shared four-column grid (Data 150px, Causale 1fr, Rif. 132px, Saldo 340px) drives both the absolutely positioned column rules and every row, so content always sits between the same rules. Cells pad 14px by 20px; the column head pads 10px by 20px and sticks to the top on scroll. Section-head rows open with 56px above and 18px below, their content spanning Causale through Saldo; the opening row pads 40px vertically. Entries that have nothing for a column leave the cell empty rather than collapsing it.

Under 1100px the columns narrow (120px, 110px, 300px). Under 900px the column rules disappear and the sheet takes a blue double rule on its left edge; rows become a two-column stack with the Data value top-left and the Rif. code top-right, description and action below; the column head shows only Data and Rif.; the Saldo form becomes a bordered panel inset 18px. Under 520px body text drops to 16px.

### Named Rules
**The Same Rules Rule.** Every row uses the shared column grid; a new component either fits in Data / Causale / Rif. / Saldo or spans a defined run of them (2-3, 2-4, full).

## Elevation & Depth

The system is flat. Depth comes from paper on desk: the sheet (Ledger Paper) lies on the darker Desk Paper with a single soft, long, low shadow beneath it. Inside the sheet nothing lifts; hierarchy is carried by rules, the darker section-head band, and the translucent white Saldo panel.

### Shadow Vocabulary
- **Sheet** (`box-shadow: 0 30px 50px -40px rgb(30 40 30 / .45)`): only under the register sheet.
- **Row ruler** (`box-shadow: inset 0 -2px 0 #2b4c8c` with a 3.5% blue wash): a ruler laid along the hovered or focused entry; a state, not elevation.

### Named Rules
**The One Sheet Rule.** Only the page itself casts a shadow. Rows, panels and buttons stay flat.

## Shapes

Square ledger geometry. Fields and rows are square (0); buttons take a barely softened 2px corner. Form is built from rules: 1px hairlines between rows, 1px green column rules, 3px double rules in blue and red, a 1px ink frame on the timeline. The timeline's post-closing stretch is hatched with thin 135-degree red lines, a ledger's way of marking a period apart.

## Components

### Buttons
Plain stationery buttons, condensed and bold, ruled in blue.
- **Shape:** nearly square (2px), 1.5px Ruling Blue border, 800 weight condensed at 17px, 0.04em tracking, optional 20px inline SVG icon at a 10px gap.
- **Primary (pieno):** Ruling Blue fill, white text, full width, used once, for the quote request in the Saldo column, sitting on the red closing rule.
- **Outline (filo):** transparent with blue text; fills blue on hover. Used for Chiama, Scrivi, Scarica, Apri la mappa. In contact rows it compacts to 10px by 14px at 15px.
- **Hover / Focus:** background and colour transition over 0.2s; focus is a 2px blue outline offset 2px.

### Inputs / Fields
- **Style:** written-on-the-line fields: transparent background, a 1px ink underline, no radius, 17px Sofia Sans at 500; label above in condensed uppercase 12px, 0.12em, Faded Ink.
- **Focus:** the underline thickens to 2px Ruling Blue.
- **Error:** the underline turns Closing Red, with a red 14px message below.

### Navigation
Condensed bold 16px links in ink, right-aligned in the header row across Rif. and Saldo; hover turns blue with a 1px blue underline. Under 900px the list wraps left-aligned beneath the logo.

### Ledger Row (signature)
The unit of the system. A grid row across the four columns with a hairline below: Data holds a condensed uppercase blue time or folio, Causale the description with an optional small explanatory line, Rif. the code, Saldo an action or a "Voci" count. On hover or keyboard focus within, the row gets the blue ruler underline and a faint blue wash (0.15s). The last row of a block carries the red double closing rule; a register count ("Voci 7") sits in its Saldo cell.

### Column Head
A sticky row of condensed uppercase blue labels (Data, Causale, Rif., Saldo) on Ledger Paper, ruled underneath with a 3px blue double rule; the last label right-aligned.

### Condominium-Year Timeline (signature)
A 44px bar framed in ink whose segments are proportional to real time: twelve months at their true day counts in a 365-day exercise, then a hatched red 180-day stretch for convening the rendiconto assembly, separated by a red double rule. A solid 2px ink marker shows today, easing into place over 1s (`cubic-bezier(.16,1,.3,1)`); a dashed blue pointer follows the cursor and a blue live readout names the date and the obligation. Length always means duration.

## Do's and Don'ts

### Do:
- **Do** lay every new block out as ledger rows on the shared Data / Causale / Rif. / Saldo grid.
- **Do** close every block with the 3px red double rule.
- **Do** give every listed service, document or item a Rif. code (ORD.01, DOC.05).
- **Do** set labels, times, codes and heads in Sofia Sans Condensed, bold and tracked, with tabular figures.
- **Do** make bar or segment length equal real duration whenever time is drawn.

### Don't:
- **Don't** use the beige office-photo hero with three icon cards.
- **Don't** invent amounts, building counts or reviews to fill the Saldo column; it holds actions and counts of real entries only.
- **Don't** put shadows on rows, panels or buttons; only the sheet casts one.
- **Don't** use red for anything other than closing rules, deadlines and errors.
- **Don't** round corners beyond the buttons' 2px.
