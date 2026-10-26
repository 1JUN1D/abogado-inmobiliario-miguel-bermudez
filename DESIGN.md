---
name: Miguel Bermúdez – Abogado
description: Real-estate lawyer in Bogotá and the Sabana Norte; the certificado de tradición read with a champagne marker, laid as paper on graphite car paint.
colors:
  graphite: "#18191b"
  graphite-raised: "#2b2c2f"
  bond-white: "#ffffff"
  silver-light: "#ecebe8"
  silver: "#cfd0cf"
  champagne: "#ddc589"
  champagne-soft: "#e8d6a8"
  champagne-pale: "#f1e7cc"
  marker: "#e6cd8a"
  print-muted: "#4a4a4c"
  on-graphite: "#f4f4f2"
  on-graphite-muted: "#b8b9bc"
  placeholder-ink: "#4d4433"
typography:
  display:
    fontFamily: "Archivo, 'Arial Narrow', Arial, sans-serif"
    fontSize: "clamp(30px, min(6.2vw, 11svh), 120px)"
    fontWeight: 800
    lineHeight: 0.96
    letterSpacing: "-0.01em"
    fontVariation: "'wdth' 112"
  headline:
    fontFamily: "Archivo, 'Arial Narrow', Arial, sans-serif"
    fontSize: "clamp(30px, 3.5vw, 54px)"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.01em"
    fontVariation: "'wdth' 112"
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
  strip: "clamp(26px, 3.4svh, 44px)"
components:
  button-primary:
    backgroundColor: "{colors.champagne}"
    textColor: "{colors.graphite}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.bond-white}"
    textColor: "{colors.graphite}"
  button-ink:
    backgroundColor: "{colors.graphite}"
    textColor: "{colors.bond-white}"
    rounded: "{rounded.none}"
    padding: "0 26px"
    height: "56px"
  button-ink-hover:
    backgroundColor: "{colors.graphite-raised}"
    textColor: "{colors.champagne}"
  field:
    backgroundColor: "{colors.champagne-pale}"
    textColor: "{colors.graphite}"
    rounded: "{rounded.none}"
    padding: "0 16px"
    height: "52px"
  folder-tab:
    backgroundColor: "{colors.champagne}"
    textColor: "{colors.graphite}"
    typography: "{typography.body}"
    padding: "0 30px"
    height: "40px"
---

# Design System: Miguel Bermúdez – Abogado

## Overview

**Creative North Star: "El folio sobre pintura de grafito"**

The site is a lawyer's desk made of new-car paint: a graphite metallic ground, photographed, on which paper objects lie, each with real edges. A stack of case folders whose tabs name the sections, a punched certificado de tradición set as dense registry print, a services sheet with zigzag tear edges, a clip-out coupon, the back of a card with a typed folder label. The lawyer's act of reading is the one warm colour on the page: champagne gold, laid as whole fields of metallic paint (the open front folder, the coupon, the first case card, the action) and as marker strokes on the lines that matter.

Type is one family, Archivo, used at two widths: expanded heavy capitals for titles (the voice of a car badge or a registry header) and normal width for everything that is read. Photographs are stock placeholders treated as grayscale photocopies, so the only colour in the world stays the champagne and the silver and white papers.

The client asked for metallic colours "como pintura de carro nuevo", something striking, and a more modern font. The metal comes from real photographs of car paint, never from CSS gradients, bevels or glows. The page still refuses the category default of a law firm (navy and gold, serif titles, scales of justice, columns, three practice-area cards). Depth comes from stacked papers and tone steps, never shadows.

**Key Characteristics:**
- Graphite car-paint ground, paper objects with cut edges, one champagne metal.
- One typeface in two widths; five sizes on the whole page.
- Square corners everywhere; the only curves are notches and scallops cut into paper.
- Grayscale photographs, never presented as the lawyer, his team or his office.

## Colors

A three-metal job: graphite, silver and champagne, with bond white for the papers.

### Primary
- **Champagne** (champagne): the single action (WhatsApp buttons, the mobile dock), the open front folder, the coupon, the first case card, the marker strokes on the folio's key lines, the active tab, the punched holes that show the folder through the sheet. Large fields and the action carry the same car-paint photograph as the graphite, re-toned to champagne by a luminance map (`assets/tex/champana-*.webp`); its mean colour is this token, so a flat tab and a painted field meet without a seam, and its darkest tone still holds graphite text at 6.4:1.

### Secondary
- **Champagne soft** (champagne-soft) and **Champagne pale** (champagne-pale): the neighbouring tones of the case cards, the process section ground, form fields inside the coupon. Champagne soft is also the colour of the proof line on graphite ("16 años de experiencia…").
- **Marker** (marker): the marker stroke on registry print, multiplied over white.

### Neutral
- **Graphite** (graphite): page ground under the photographs, casos and contact; body text on paper. The hero, the experience section and the footer carry the graphite car-paint photograph (`assets/tex/grafito-*.webp`).
- **Raised graphite** (graphite-raised): hover state of ink buttons and the map frame.
- **Bond white** (bond-white): sheets, the menu, the "Antes de firmar" field, the back card.
- **Silver light** (silver-light) and **Silver** (silver): folder papers and the FAQ and services grounds.
- **Print muted** (print-muted): secondary text on paper, 8.9:1 on white, 5.7:1 on silver.
- **Placeholder ink** (placeholder-ink): placeholder text inside pale champagne fields.
- **On graphite** (on-graphite) and **On graphite muted** (on-graphite-muted): text on the graphite. Text over the car-paint photographs is checked against the brightest 3% of the photo under it.

### Named Rules
**The Champagne Rule.** Champagne marks what the reader must act on or notice: the action, the open folder, the lines a lawyer would mark, the sixteen years. On printed paper it is a line-bound marker stroke with uneven ends, never a padded box. It is never decoration and never a gradient.

**The Real Metal Rule.** Metal is a photograph of paint, cropped and toned, never a CSS gradient, sheen, bevel or glow. Graphite photos stay dark enough that white text keeps 4.5:1 over their brightest highlight.

**The Folder Ground Rule.** Each section takes the colour of the folder tab that names it in the hero stack (Su caso champagne, Servicios silver, Antes de firmar white, Proceso pale champagne, Preguntas light silver) and opens under a textless trapezoid tab of its own paper, at the same horizontal position as in the stack.

## Typography

**Display Font:** Archivo at width 112, weight 800, uppercase (100 on tablets, 87 on phones so the hero stays on two lines).
**Body Font:** Archivo at width 100, weights 400 to 750 (fallback Arial).
**Wordmark:** "Miguel Bermúdez – Abogado" in Archivo width 125, weight 700, uppercase, never tracked out.

**Character:** an Argentine grotesque whose name means "file"; expanded and heavy it reads like a badge on a car body or a registry header, at normal width it reads like a well-set contract.

### Hierarchy
- **Display** (800, clamp(30px, min(6.2vw, 11svh), 120px), 0.96): the hero title and the closing name in the footer.
- **Headline** (800, clamp(30px, 3.5vw, 54px), 1): every section title, uppercase, two lines at most.
- **Title** (650, clamp(21px, 1.9vw, 28px), 1.15): the hero sentence, the experience statement, card titles, the certificate title, tab panel titles.
- **Body** (400, 16–18px, 1.55): all reading text, folder tabs, form fields, 45–75 characters per line.
- **Label** (400, 15px, 1.38–1.45): registry print on the folio and the coupon slip (field names in bold capitals: ANOTACIÓN, ESPECIFICACIÓN, DE, A), service tags, captions, the imprint.

### Named Rules
**The Five Sizes Rule.** The page uses five sizes and no more; a new element maps to one of them.

**The Badge Rule.** Capitals belong to the expanded display and headline voices, the wordmark, and registry field names; nothing longer is set in capitals, and no small text is tracked out.

**The Registry Print Rule.** Registry content keeps its own grammar (ANOTACIÓN: Nro n, Fecha DD-MM-AAAA, Radicación, ESPECIFICACIÓN, DE / A, X for the titular) with tabular figures and tight leading, without zero-padded numbers and without any official emblem.

## Layout

A 12-column grid between equal outer margins (16–32px). Large objects run from margin to margin (the folder stack, the folio panel) or sit on columns 2–11 (the coupon, the back card). Sections are separated by 96–168px and by a hard change of ground. The hero is a centred composition whose folder stack begins near half the viewport height so the open folder and the WhatsApp button show in the first screen. The experience section splits title (columns 1–5) and text (7–12). On phones every split becomes a single column and the coupon turns upright with its perforation horizontal. Below 1024px (phones and tablets) a champagne WhatsApp bar stays at the bottom with the safe area respected; it steps aside while the folder's button or the coupon is on screen.

## Elevation & Depth

No shadows anywhere. Depth is the stacking of papers on the painted ground: folder bands overlap by a fixed strip, sheets sit on a contrasting ground, and a sheet's tone differs from the ground it lies on.

### Named Rules
**The Paper Stack Rule.** Things are in front because they overlap, never because they cast a shadow.

## Shapes

Square corners on every rectangle, button and field (0px). Paper edges carry the shape language: trapezoid folder tabs on the hero stack and on top of each section, two punched holes on the folio sheet, zigzag tear edges on the services sheet, semicircular notches and a dotted perforation on the coupon, a row of scallops on the back card. These are filled shapes in the colour of what lies beneath, or SVG fills, never outlines. The lawyer's hand appears only as marker strokes and a pen bracket beside the margin notes.

## Components

### Buttons
- **Shape:** square (0px), 56px tall, 44px minimum for the small header button.
- **Primary:** champagne paint, graphite text, WhatsApp glyph at 1.15em, label "Consultar por WhatsApp" everywhere.
- **Ink:** graphite fill with white text where the primary would sit on champagne (front folder, coupon submit).
- **Hover / Focus:** colour swap in 180ms, press scales to 0.97; focus is a 3px outline offset 3px, graphite on light grounds and champagne on graphite.

### Cards / Containers
- **Corner Style:** square.
- **Background:** the three champagne tones for the case cards (the first one painted); bond white for sheets.
- **Shadow Strategy:** none, see Elevation.
- **Internal Padding:** 22–40px.

### Inputs / Fields
- **Style:** filled blocks in pale champagne, 48px tall, no border, set inline inside a sentence whose words are the visible labels; they size to their content and stack full width on phones. Option texts stay under 30 characters so they never clip on a 360px phone.
- **Focus:** 3px graphite outline; a filled field turns bond white.

### Navigation
- The hero folder tabs are the first navigation. After the hero a solid graphite bar slides in from 1024px with the wordmark, five section links (Experiencia, Casos, Servicios, Proceso, Preguntas) and the champagne action. Below 1024px the champagne dock replaces it.

### Folio sheet (signature)
A punched white certificate in dense registry print: title and matrícula, then anotaciones (number, date, radicación, especificación, DE / A). The lines that matter carry a marker stroke that draws across once as the entry enters; the lawyer's plain-language note sits in a margin column behind a pen bracket. Always labelled as an illustrative example.

### Experience band
Graphite paint, the headline "16 años en los estrados" with the years in champagne, one statement on judicial and extrajudicial representation of people and companies, two short columns (Para prevenir, Para resolver) and the zone line (Bogotá y la Sabana Norte: Chía, Cajicá y Zipaquirá).

### Clip-out coupon (signature)
The champagne coupon, "Arme su anotación", is one sentence the visitor completes ("Mi caso es que … con … Hoy … Me llamo …"). A white slip under it shows the result as an anotación (ESPECIFICACIÓN, DE / A, Estado), the left half lists the documents to bring, and a status line says what is missing; the button opens WhatsApp (+57 301 507 0487) with the message written. States: empty, marked, ready.

### Case deck
On wide screens (1100px and up, motion allowed) the six case cards are pinned and fold one by one into labelled spines as the visitor scrolls. A card's words leave before its spine label arrives, so the two never overlap, and the open card narrows on smaller desktops so the last card always ends inside the grid. Elsewhere the cards are a plain stack.

### Process row
A horizontal row of steps that snaps, with photographs on one top line, a plain "n de 7" count and two square graphite buttons; no progress rule.

## Do's and Don'ts

### Do:
- **Do** keep the ground graphite and lay paper on it; every new section is another piece of the same stationery.
- **Do** use champagne (#ddc589) for the action and for what the reader must notice, at page scale.
- **Do** say "16 años de experiencia en representación judicial y extrajudicial de personas y empresas" and "Bogotá y la Sabana Norte (Chía, Cajicá, Zipaquirá)" where the visitor decides.
- **Do** treat placeholder photographs in grayscale and caption them as what they are.
- **Do** keep one primary action name: "Consultar por WhatsApp".

### Don't:
- **Don't** use navy and gold, serif display faces, scales of justice, gavels, columns or law-book shelves.
- **Don't** add shadows, CSS gradients, glass, chrome bevels, rounded "soft" corners or thin divider lines.
- **Don't** put small labels above headings or number sections 01/02/03.
- **Don't** present stock photographs as Miguel Bermúdez, his team or his office, and don't invent reviews, figures or results.
- **Don't** publish an address for the Chía office until the client gives one.
