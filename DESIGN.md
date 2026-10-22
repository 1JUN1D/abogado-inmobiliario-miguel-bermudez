---
name: Bermúdez Abogados y Asociados
description: Real-estate lawyer in Bogotá; the certificado de tradición read with a highlighter, laid out as paper on an ink desk.
colors:
  desk-ink: "#141414"
  desk-ink-raised: "#262624"
  bond-white: "#ffffff"
  file-grey-light: "#edede7"
  file-grey: "#d6d6cf"
  highlighter: "#ffe01b"
  highlighter-soft: "#ffe963"
  highlighter-pale: "#fff09e"
  print-muted: "#4a4a47"
  on-ink: "#f4f4f0"
  on-ink-muted: "#b9b9b2"
  placeholder-ink: "#3f3a1d"
typography:
  display:
    fontFamily: "Archivo, 'Arial Narrow', Arial, sans-serif"
    fontSize: "clamp(38px, min(9.2vw, 13svh), 150px)"
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: "-0.005em"
    fontVariation: "'wdth' 62"
  headline:
    fontFamily: "Archivo, 'Arial Narrow', Arial, sans-serif"
    fontSize: "clamp(34px, 4.4vw, 66px)"
    fontWeight: 800
    lineHeight: 0.94
    letterSpacing: "-0.005em"
    fontVariation: "'wdth' 62"
  title:
    fontFamily: "Archivo, Arial, sans-serif"
    fontSize: "clamp(21px, 1.9vw, 28px)"
    fontWeight: 650
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Archivo, Arial, sans-serif"
    fontSize: "clamp(16px, 0.35vw + 13px, 18px)"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Archivo, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.45
rounded:
  none: "0px"
  notch: "50%"
spacing:
  margin: "clamp(16px, 2.2vw, 32px)"
  gutter: "clamp(16px, 1.7vw, 24px)"
  section: "clamp(96px, 11vw, 168px)"
  tab: "40px"
  strip: "clamp(40px, 6svh, 60px)"
components:
  button-primary:
    backgroundColor: "{colors.highlighter}"
    textColor: "{colors.desk-ink}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.bond-white}"
    textColor: "{colors.desk-ink}"
  button-ink:
    backgroundColor: "{colors.desk-ink}"
    textColor: "{colors.bond-white}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "56px"
  button-ink-hover:
    backgroundColor: "{colors.desk-ink-raised}"
    textColor: "{colors.highlighter}"
  field:
    backgroundColor: "{colors.highlighter-pale}"
    textColor: "{colors.desk-ink}"
    rounded: "{rounded.none}"
    padding: "0 16px"
    height: "52px"
  folder-tab:
    backgroundColor: "{colors.highlighter}"
    textColor: "{colors.desk-ink}"
    typography: "{typography.body}"
    padding: "0 30px"
    height: "40px"
---

# Design System: Bermúdez Abogados y Asociados

## Overview

**Creative North Star: "El folio leído con resaltador"**

The site is a lawyer's desk seen at night: an ink-black ground on which paper objects lie, each with real edges. A stack of case folders whose tabs name the sections, a punched certificado de tradición set as dense registry print, a services sheet with zigzag tear edges, a clip-out coupon, the back of a card with a typed folder label. The lawyer's act of reading is the one colour on the page: highlighter yellow, laid as whole fields, as marker strokes on the lines that matter, and on the single action.

Type is one family, Archivo, used at two widths: condensed heavy capitals for titles (the voice of a stamp or a registry header) and normal width for everything that is read. Photographs are stock placeholders treated as grayscale photocopies, so the only colour in the world stays the yellow and the folder papers.

The page refuses the category default of a law firm (navy and gold, serif titles, scales of justice, columns, three practice-area cards). Depth comes from stacked papers and tone steps, never shadows.

**Key Characteristics:**
- Ink desk ground, paper objects with cut edges, one highlighter yellow.
- One typeface in two widths; five sizes on the whole page.
- Square corners everywhere; the only curves are notches and scallops cut into paper.
- Grayscale photographs, never presented as the lawyer, his team or his office.

## Colors

A two-ink print job on bond paper: black, white and highlighter yellow, with two file-folder greys.

### Primary
- **Highlighter** (highlighter): the single action (WhatsApp buttons, the mobile dock), the open front folder, the coupon, the marker strokes on the folio's key lines, the active tab, the punched holes that show the folder through the sheet.

### Secondary
- **Soft highlighter** (highlighter-soft) and **Pale highlighter** (highlighter-pale): the neighbouring tones of the case cards, the process section ground, form fields inside the yellow coupon.

### Neutral
- **Desk ink** (desk-ink): page ground, hero, contact and footer; body text on paper.
- **Raised ink** (desk-ink-raised): hover state of ink buttons and the map frame.
- **Bond white** (bond-white): sheets, the menu, the "Antes de firmar" field, the back card.
- **File grey light** (file-grey-light) and **File grey** (file-grey): folder papers and the FAQ and services grounds.
- **Print muted** (print-muted): secondary text on paper (descriptions, service tags, empty slots of the coupon slip), 8.9:1 on white.
- **Placeholder ink** (placeholder-ink): placeholder text inside pale yellow fields.
- **On ink** (on-ink) and **On ink muted** (on-ink-muted): text on the desk.

### Named Rules
**The Highlighter Rule.** Yellow marks what the reader must act on or notice: the action, the open folder, the lines a lawyer would mark. On printed paper it is a line-bound marker stroke with uneven ends, never a padded box. It is never decoration and never a gradient.

**The Folder Ground Rule.** Each section takes the colour of the folder tab that names it in the hero stack (Su caso yellow, Servicios file grey, Antes de firmar white, Proceso pale yellow, Preguntas light grey) and opens under a textless trapezoid tab of its own paper, at the same horizontal position as in the stack.

## Typography

**Display Font:** Archivo at width 62, weight 800, uppercase (fallback Arial Narrow).
**Body Font:** Archivo at width 100, weights 400 to 750 (fallback Arial).

**Character:** an Argentine grotesque whose name means "file"; condensed and heavy it reads like a registry stamp, at normal width it reads like a well-set contract.

### Hierarchy
- **Display** (800, clamp(38px, min(9.2vw, 13svh), 150px), 0.9): the hero title and the closing name in the footer.
- **Headline** (800, clamp(34px, 4.4vw, 66px), 0.94): every section title, uppercase, two lines at most.
- **Title** (650, clamp(21px, 1.9vw, 28px), 1.15): the hero sentence, card titles, the certificate title, tab panel titles.
- **Body** (400, 16–18px, 1.55): all reading text, folder tabs, form fields, 45–75 characters per line.
- **Label** (400, 15px, 1.38–1.45): registry print on the folio and the coupon slip (field names in bold capitals: ANOTACIÓN, ESPECIFICACIÓN, DE, A), service tags, captions, the imprint.

### Named Rules
**The Five Sizes Rule.** The page uses five sizes and no more; a new element maps to one of them.

**The Stamp Rule.** Capitals belong to the condensed display and headline voices and to registry field names and act names of three words or fewer; nothing longer is set in capitals, and no small text is tracked out.

**The Registry Print Rule.** Registry content keeps its own grammar (ANOTACIÓN: Nro n, Fecha DD-MM-AAAA, Radicación, ESPECIFICACIÓN, DE / A, X for the titular) with tabular figures and tight leading, without zero-padded numbers and without any official emblem.

## Layout

A 12-column grid between equal outer margins (16–32px). Large objects run from margin to margin (the folder stack, the folio panel, the coupon and the back card sit on columns 2–11). Sections are separated by 96–168px and by a hard change of ground colour. The hero is a centred composition whose folder stack begins near half the viewport height so the open folder and the WhatsApp button show in the first screen. On phones every split becomes a single column, the coupon turns upright with its perforation horizontal, and a solid yellow WhatsApp bar stays at the bottom with the safe area respected.

## Elevation & Depth

No shadows anywhere. Depth is the stacking of papers: folder bands overlap by a fixed strip, sheets sit on a contrasting ground, and a sheet's tone differs from the ground it lies on.

### Named Rules
**The Paper Stack Rule.** Things are in front because they overlap, never because they cast a shadow.

## Shapes

Square corners on every rectangle, button and field (0px). Paper edges carry the shape language: trapezoid folder tabs on the hero stack and on top of each section, two punched holes on the folio sheet, zigzag tear edges on the services sheet, semicircular notches and a dotted perforation on the coupon, a row of scallops on the back card. These are filled shapes in the colour of what lies beneath, or SVG fills, never outlines. The lawyer's hand appears only as marker strokes and a pen bracket beside the margin notes.

## Components

### Buttons
- **Shape:** square (0px), 56px tall, 44px minimum for the small header button.
- **Primary:** highlighter fill, ink text, WhatsApp glyph at 1.15em, label "Consultar por WhatsApp" everywhere.
- **Ink:** ink fill with white text where the primary would sit on yellow (front folder, coupon submit).
- **Hover / Focus:** colour swap in 180ms, press scales to 0.97; focus is a 3px outline offset 3px, ink on light grounds and yellow on the desk.

### Cards / Containers
- **Corner Style:** square.
- **Background:** the three highlighter tones for the case cards; bond white for sheets.
- **Shadow Strategy:** none, see Elevation.
- **Internal Padding:** 22–40px.

### Inputs / Fields
- **Style:** filled blocks in pale highlighter, 48px tall, no border, set inline inside a sentence whose words are the visible labels; they size to their content and stack full width on phones.
- **Focus:** 3px ink outline; a filled field turns bond white.

### Navigation
- The hero folder tabs are the first navigation. After the hero a solid ink bar slides in on desktop with the wordmark, five section links and the yellow action. On phones the yellow dock replaces it.

### Folio sheet (signature)
A punched white certificate in dense registry print: title and matrícula, then anotaciones (number, date, radicación, especificación, DE / A). The lines that matter carry a marker stroke that draws across once as the entry enters; the lawyer's plain-language note sits in a margin column behind a pen bracket. Always labelled as an illustrative example.

### Clip-out coupon (signature)
The yellow coupon, "Arme su anotación", is one sentence the visitor completes ("Mi caso es que … con … Hoy … Me llamo …"). A white slip under it shows the result as an anotación (ESPECIFICACIÓN, DE / A, Estado), the left half lists the documents to bring, and a status line says what is missing; the button opens WhatsApp with the message written. States: empty, marked, ready.

### Process row
A horizontal row of steps that snaps, with photographs on one top line, a plain "n de 7" count and two square ink buttons; no progress rule.

## Do's and Don'ts

### Do:
- **Do** keep the ground ink and lay paper on it; every new section is another piece of the same stationery.
- **Do** use highlighter yellow (#ffe01b) for the action and for what the reader must notice, at page scale.
- **Do** treat placeholder photographs in grayscale and caption them as what they are.
- **Do** keep one primary action name: "Consultar por WhatsApp".
- **Do** mark a sample phone number as "(número de muestra)" wherever it is visible until the real one exists.

### Don't:
- **Don't** use navy and gold, serif display faces, scales of justice, gavels, columns or law-book shelves.
- **Don't** add shadows, gradients, glass, rounded "soft" corners or thin divider lines.
- **Don't** put small labels above headings or number sections 01/02/03.
- **Don't** present stock photographs as Miguel Bermúdez, his team or his office, and don't invent reviews, figures or results.
