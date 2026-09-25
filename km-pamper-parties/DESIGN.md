---
name: KM Pamper Parties, Classic Edition
description: Cream paper, olive gold, Cormorant capitals held between gold rules, and the real team in every photograph.
colors:
  cream: "#F8F6F1"
  cream-2: "#F1ECE1"
  white: "#FFFFFF"
  ink: "#2F3437"
  ink-2: "#565B5F"
  ink-3: "#6B7074"
  gold: "#897600"
  gold-2: "#6E5E00"
  gold-line: "#D9CD9A"
  line: "#E6E0D2"
  rose: "#B8407F"
  pink-tint: "#FBEAF7"
typography:
  display:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(2.1rem, 4.6vw, 4rem)"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "0.05em"
  headline:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(1.7rem, 3.2vw, 2.5rem)"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "0.08em"
  title:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "1.35rem"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "0.06em"
  serif-line:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "1.35rem"
    fontWeight: 500
  caption:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "1.05rem"
    fontWeight: 500
  numeral:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(3rem, 6vw, 4.4rem)"
    fontWeight: 500
    lineHeight: 1
    fontFeature: "tabular-nums"
  body:
    fontFamily: "Lato, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.65
  lede:
    fontFamily: "Lato, system-ui, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Lato, system-ui, sans-serif"
    fontSize: "0.74rem"
    fontWeight: 700
    letterSpacing: "0.16em"
rounded:
  none: "0"
spacing:
  gutter: "20px"
  row: "1rem"
  lede: "1.2rem"
  stack: "1.8rem"
  after-heading: "2.6rem"
  grid: "3rem"
  grid-wide: "3.5rem"
  section: "4.5rem"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0.95rem 1.7rem"
  button-primary-hover:
    backgroundColor: "{colors.gold-2}"
    textColor: "{colors.white}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0.95rem 1.7rem"
  button-line-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.white}"
  button-white:
    backgroundColor: "transparent"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0.95rem 1.7rem"
  button-white-hover:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
  input:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "0.75rem 0.9rem"
  panel:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink-2}"
    rounded: "{rounded.none}"
    padding: "2rem"
  band:
    backgroundColor: "{colors.cream-2}"
    textColor: "{colors.ink}"
    padding: "4.5rem 0"
  nav-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink-2}"
    typography: "{typography.label}"
  nav-link-hover:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
---

# Design System: KM Pamper Parties, Classic Edition

This file records the Classic Edition concept only (`classic/index.html`), extracted from its shipped CSS. The plum and blush-gold concepts are separate visual worlds and are not covered here.

## Overview

**Creative North Star: "The Gold-Ruled Letterhead"**

The Classic Edition is the incumbent KM identity kept and finished rather than replaced. It behaves like good stationery: a sheet of cream paper (#F8F6F1), charcoal ink, and one metallic, olive gold, used the way a stationer uses foil: for hairline rules, small tracked capitals and the one solid block of a button. Every heading is a line of Cormorant Garamond capitals held between two gold rules that draw in when the page loads. The brand pink survives but is cooled to a rose reserved for the ways you reach KM (WhatsApp, email) and kept as a pale tint field under the parties section, so warmth arrives exactly where the party audience lands.

Density is generous and editorial. Sections breathe at 4.5rem, content follows its heading at a fixed 2.6rem, and lists are separated by hairlines rather than boxed. There are no cards in the ordinary sense: reasons sit in columns under a short 2px gold rule, prices sit in a ruled three-column strip, treatments and case studies are hairline rows. The only "panels" are white sheets (form, pricing note, success message) laid on the cream with a gold hairline edge. Corners are square everywhere, including form fields.

Photography is the system's proof. Every image is a real photograph of the team, served at two sizes, cropped with an explicit aspect ratio and object position, and captioned in italic Cormorant. The first viewport is a full-bleed photograph of six therapists with the tagline set low in white capitals over a charcoal gradient. The build confirms the direction contract's refusals: no stock-spa hero, no three icon cards, no rounded card grid.

**Key Characteristics:**
- Cream ground, charcoal text, olive gold as the single accent for rules, buttons and small capitals
- Every section heading is Cormorant tracked capitals held between two 1px gold hairlines
- Two golds: the saturated gold fills and rules; the deeper gold carries any gold text
- Rose appears only on contact links, error states and as the pale tint field under the parties section
- Square corners, no shadows at rest; depth is a white sheet or a cream-2 band with a gold hairline edge
- Hairline-separated lists and definition rows instead of cards
- Real photographs only, two sizes each, italic Cormorant captions

## Colors

A warm-neutral paper palette with one metallic accent and one cooled brand pink; every hue is low in chroma except the gold and the rose, and both are rationed.

### Primary
- **Olive Gold** (`gold`): the one accent. It is a fill and a line: button background, the 1px rules that flank headings (as its pale sibling), the 2px rule above each reason column, the 4px and 5px list dots, the FAQ plus sign, the star row, the 3px focus outline, the text-selection colour, the input caret. It carries white text only inside buttons and the skip link (4.51:1).
- **Deep Olive Gold** (`gold-2`): the text gold. Every tracked-capital label that is gold (logo strapline, route "Explore" links, definition terms, tier durations, contact keys, treatment settings, case dates), the route price, and the button hover fill. It clears AA on cream at 5.96:1 where Olive Gold would not (4.18:1).
- **Gold Hairline** (`gold-line`): the structural hairline. Heading rules, header and footer borders, band borders, the pricing strip's inner and outer borders, panel borders (form, note, success), the contact list's row rules, the team-line separators, the hamburger's border.

### Secondary
- **Cooled Rose** (`rose`): the brand pink cooled for links and errors. Contact list links (WhatsApp, email), the Google rating link on hover, the invalid-field border and the form error message. It never appears on a heading, a button or a rule.
- **Rose Tint** (`pink-tint`): the pale field under the pamper parties section, the single large appearance of the brand pink.

### Neutral
- **Cream Paper** (`cream`): the page ground, the input background, the mobile menu sheet, and at 92 to 95 percent opacity the blurred sticky header and mobile bar.
- **Folded Cream** (`cream-2`): the tonal band. Full-width bands between gold hairlines (clients, reviews) and the untinted enquiry section.
- **Card White** (`white`): the white sheet laid on cream for the form, the pricing note and the success message; also the text colour on buttons and over the hero photograph.
- **Charcoal Ink** (`ink`): headings, body text, the logo wordmark, the mobile hero gradient's foot, the hamburger bars.
- **Soft Charcoal** (`ink-2`): supporting text. Ledes, route and reason copy, definition descriptions, captions, footer, nav links at rest, form labels, reviewer names.
- **Grey Ink** (`ink-3`): tertiary text. Placeholders, treatment durations, "per person", the reviewer's context line.
- **Cream Hairline** (`line`): the in-list hairline. Row rules inside definition lists, case lists, treatment lists, FAQ items, the input border at rest and the open mobile menu.

### Named Rules
**The Two Golds Rule.** Olive gold (`gold`) is a fill and a line: buttons, rules, dots, focus rings, selection. Any gold text is set in deep olive gold (`gold-2`). Olive gold is never text on cream.

**The Rose Is Reachable Rule.** Rose marks the ways to reach KM and the ways a form can go wrong: contact links, the rating link hover, invalid borders, error text. It is never a heading, a button or a rule; its one large use is the pale tint field under the parties section.

**The Hairline Hierarchy Rule.** Gold hairline (`gold-line`) frames: the header, bands, panels, the pricing strip, the contact list. Cream hairline (`line`) separates rows inside a list. Do not swap them.

## Typography

**Display Font:** Cormorant Garamond (with Georgia, serif), weights 500 and 600, italic 500
**Body Font:** Lato (with system-ui, sans-serif), weights 400 and 700, italic 400
**Label/Mono Font:** none; labels are Lato 700 tracked capitals

**Character:** An engraved serif in tracked capitals for every heading and for the names of things, and a plain humanist sans for explanation and labels. Cormorant is never set small and never in Lato's role; Lato never becomes a heading. The pairing reads as stationery rather than as a website template.

### Hierarchy
- **Display** (500, clamp(2.1rem, 4.6vw, 4rem), 1.1, tracked 0.05em, uppercase): the hero tagline only, in white, balanced, capped at 22ch. Drops to 1.9rem under 700px.
- **Headline** (500, clamp(1.7rem, 3.2vw, 2.5rem), 1.1, tracked 0.08em, uppercase): every section heading, always rendered as the ruled heading. Route headings use a smaller clamp(1.5rem, 2.6vw, 2rem).
- **Title** (500, 1.35rem, 1.1, tracked 0.06em, uppercase): column headings under the short gold rules (1.15rem there); the logo wordmark is the same face at 600, 1.45rem, tracked 0.04em.
- **Serif line** (500, 1.2 to 1.4rem, body leading): the names of things set in Cormorant at reading size. Client names (clamp 1.2 to 1.4rem), treatment names (1.4rem), contact values and links (1.4rem), FAQ questions (1.35rem), occasions and the team line (1.3rem), case-study names and definition terms at 600. Review quotes are the italic form at 1.35rem with 1.4 leading.
- **Caption** (500 italic, 1.05rem, soft charcoal): the figcaption under every photograph, 0.8rem below it.
- **Numeral** (500, clamp(3rem, 6vw, 4.4rem), 1, tabular figures): the per-person price in each pricing tier.
- **Body** (400, 17px, 1.65): paragraphs and descriptions. Ledes step up to 1.05rem, soft charcoal, and are capped at 40rem (36rem in the hero). Reason and tier copy step down to 0.95 and 0.92rem.
- **Label** (700, 0.68 to 0.78rem, tracked 0.14 to 0.24em, uppercase): the tracked capital. Buttons (0.78rem, 0.14em), nav links (0.74rem, 0.14em), the hero's fine line (0.74rem, 0.18em), route links (0.76rem), reviewer names (0.74rem, 0.16em), tier durations (0.74rem, 0.2em), form labels (0.7rem, 0.16em), contact keys (0.7rem, 0.2em), treatment settings (0.68rem), the logo strapline (0.62rem, 0.24em). Colour is deep olive gold or soft charcoal, never olive gold.

### Named Rules
**The Capitals Between Rules Rule.** Every section heading is Cormorant tracked capitals held between two 1px gold hairlines. Nothing sits above a heading; the rules are its only ornament.

**The Serif Carries the Noun Rule.** Names (clients, treatments, occasions, questions, contact values, quotes) are set in Cormorant at 1.2 to 1.4rem. Lato carries explanation, and in tracked capitals, labels.

**The Middle Dot Rule.** Short facts in a line are separated by a spaced middle dot (Nottingham · Derby · Leicester), never by an em dash or a pipe.

## Layout

A single centred column of 1180px maximum with a 20px gutter on both sides. Sections stack with 4.5rem of vertical padding; the closing call-to-action band uses 4rem and the footer 2.5rem above, 4.5rem below (7.5rem below on mobile to clear the fixed bar). Inside a section, content follows its ruled heading at exactly 2.6rem, a lede at 1.2rem, a button row at 1.8rem, a caption at 0.8rem.

Two-column layouts are asymmetric grids: 0.85fr and 1.15fr for the corporate photo and definition list, 0.8fr and 1.2fr for case studies and the enquiry form, 1fr and 1fr for routes and the party grid. Column gaps are 3rem (routes, reviews, party grid) or 3.5rem (corporate, enquiry); the treatments list is a two-column CSS multicolumn with a 4rem gap. Four reasons sit in four equal columns at 2.5rem, collapsing to two at 900px and one at 520px.

Lists are vertical stacks of hairline rows with 1rem of padding above and below (1.1rem in definition rows), the first row carrying a top rule and the last a bottom rule. Definition rows put the term in a fixed 8.5rem column with a 1rem gap.

Responsive collapse happens between 900px and 520px depending on the grid: the nav collapses to a hamburger and two-column grids stack at 900px; reviews and the party grid at 860px; routes at 820px; case studies and the mobile bar appear at 800px; treatments go single-column at 760px; the hero restacks at 700px; the pricing strip at 640px; client names go to a single centred column at 600px; definition rows and the form at 560px; reason columns and the team line at 520px. At 700px and under the hero becomes a square photograph with the text block pulled 4.5rem up over it on a charcoal gradient, and its buttons go full width.

The hero itself is `min(78vh, 760px)` tall with its content aligned to the foot, 12rem of top padding and 3.2rem below, over a photograph cropped `object-fit: cover` at 50% 58% and a four-stop gradient of warm near-black (rgba(30,27,22) from 0.10 to 0.9).

## Elevation & Depth

The paper is flat. Nothing casts a shadow at rest; the single box-shadow in the system is the 3px olive-gold-at-15% ring on a focused field. Depth is tonal and linear: a white sheet on the cream ground with a 1px gold hairline (form, pricing note, success), a folded-cream band between two gold hairlines (clients, reviews), and the pale rose field under parties. Sticky surfaces (the header and the mobile action bar) are cream at 92 and 95 percent opacity over a 10px backdrop blur, edged by a gold hairline, so the page shows through faintly as it scrolls.

### Shadow Vocabulary
- **Field focus ring** (`box-shadow: 0 0 0 3px rgba(137,118,0,.15)`): with a gold border, on a focused input, select or textarea. Not used anywhere else.

### Named Rules
**The Paper Is Flat Rule.** No shadows at rest and no shadows on hover. Depth is a white sheet or a cream band with a gold hairline edge.

## Shapes

Everything is rectangular. Buttons, inputs, panels, photographs and the pricing strip all have a 0 radius, and inputs set `border-radius: 0` explicitly to defeat the user agent. The only curves are the 4px gold dot between client names and the 5px gold bullet before each occasion, both `border-radius: 50%`.

Lines are thin. Hairlines are 1px (gold or cream); the button border and the nav link's underline are 1.5px; the one heavier line is the 2px gold rule above each reason column. The FAQ marker is a 16px plus sign built from two 1.5px gold gradients that rotates 45 degrees to a cross when open. Photographs are clipped to fixed aspect ratios (16/10 for routes, 16/9 for the team, 4/5 for the corporate portrait, 1/1 for case studies and the mobile hero, 4/3 for the party image) and cropped with `object-fit: cover` and an explicit `object-position`.

## Components

### Buttons
Rectangular, tracked, quiet. A button is a block of tracked capitals with a 1.5px border in the same colour as its fill, so the outline variants read as the same object emptied out.
- **Shape:** square corners (0 radius), 1.5px border, inline-flex with a 0.6rem gap for any leading mark
- **Primary:** olive gold fill and border, white text, 0.95rem by 1.7rem padding, Lato 700 at 0.78rem tracked 0.14em uppercase. In the header it is compact (0.6rem by 1.1rem; 0.55rem by 0.8rem under 900px); in the mobile bar each button flexes to half width at 0.85rem by 1rem.
- **Hover / Focus:** fill and border shift to deep olive gold over 0.15s; focus-visible draws a 3px olive gold outline offset 3px (the global focus treatment for every link, button, summary and field).
- **Line:** transparent fill, olive gold border, charcoal text; on hover fills olive gold with white text. Used for the WhatsApp action beside a primary button.
- **White:** transparent fill, white border and text, for use over the hero photograph; on hover fills white with charcoal text.

### Ruled Heading
The signature. An h2 laid in a three-column grid: a flexible 1px gold hairline, the capitals at their natural width, a flexible 1px gold hairline, each rule at least 2.5rem wide with a 1.4rem gap to the text. Both rules scale in from the text outward over 1.1s on an ease-out curve (cubic-bezier(.16,1,.3,1)) after a 0.15s delay; reduced motion disables it. The `left` variant drops the leading rule and left-aligns the text so the trailing rule runs to the column edge; a lede following it also left-aligns. A one-line lede in soft charcoal may follow at 1.2rem, centred, capped at 40rem.

### Cards / Containers
There are no cards. The containers are:
- **White sheet:** card white fill, 1px gold hairline border, 2rem padding (1.3rem under 560px), 0 radius. The enquiry form, the success message (Cormorant 2rem with a Lato 1.05rem line beneath), and the pricing note (1.2rem by 1.4rem padding, soft charcoal with charcoal bold lead-in).
- **Band:** folded cream fill with a 1px gold hairline above and below, full width, 4.5rem vertical padding. The `tint` variant drops the borders; the parties section uses the rose tint field instead.
- **Ruled column:** a 2px olive gold top rule, 1.2rem padding above a 1.15rem title and a 0.95rem soft charcoal paragraph. Four across, no background, no border elsewhere.
- **Pricing strip:** three equal cells with a gold hairline above and below the strip and between cells, 2rem by 1.4rem padding, centred. Each cell is a tracked duration label in deep gold, the numeral price, "per person" in grey ink at 0.85rem, and a 0.92rem paragraph capped at 24rem. Cells stack with horizontal rules under 640px.

### Inputs / Fields
- **Style:** Lato at 1rem, 0.75rem by 0.9rem padding, 1px cream hairline border, cream paper fill, charcoal text, 0 radius, full width. Placeholders in grey ink. Labels are a grid above the field with a 0.4rem gap, Lato 700 at 0.7rem tracked 0.16em uppercase in soft charcoal. Caret and native controls are gold.
- **Focus:** border turns olive gold and a 3px gold-at-15% ring appears; the outline is suppressed in favour of the ring.
- **Error:** an invalid field takes a rose border; the message is rose, Lato 700 at 0.9rem, with `role="alert"`.
- **Layout:** fields stack at 1.1rem; paired fields sit in a two-column grid at the same gap, stacking under 560px.

### Navigation
- **Style:** sticky header of cream at 92 percent over a 10px blur with a gold hairline underneath; 0.9rem vertical padding, 2rem gaps. The logo is a two-line grid: Cormorant 600 at 1.45rem tracked 0.04em uppercase in charcoal over a Lato 700 strapline at 0.62rem tracked 0.24em in deep gold.
- **Links:** Lato 700 at 0.74rem tracked 0.14em uppercase in soft charcoal, 1.7rem apart, with a 1.5px transparent underline 0.25rem below the baseline.
- **Hover / Current:** text turns charcoal and the underline turns olive gold; the current page is marked with `aria-current="page"`.
- **Mobile (900px and under):** links hide behind a 44px square hamburger with a gold hairline border and three 20px by 1.5px charcoal bars; the strapline hides and the wordmark drops to 1.2rem. The open menu is a cream sheet below the header with a gold hairline foot, each link a full-width row at 0.9rem with a cream hairline beneath. A compact Enquire button stays visible.
- **Mobile bar (800px and under):** a fixed bar at the foot, cream at 95 percent over a 10px blur with a gold hairline above, safe-area padded, holding a line WhatsApp button and a primary Enquire button at equal width.

### Hairline List
Rows separated by 1px cream hairlines with 1rem padding above and below; the first row rules its top and the last rules its bottom. Three shapes share it: the treatments row (a Cormorant name at 1.4rem with a Lato 0.82rem grey duration beside it, and a tracked deep-gold setting label right-aligned at the far end), the case-study row (Cormorant 600 name at 1.35rem, a 0.95rem soft charcoal line, and a tracked deep-gold date at 0.7rem), and the FAQ item (a Cormorant 1.35rem question as a summary with the gold plus at the right, the answer in soft charcoal at 0.5rem capped at 60ch). The contact list is the same row with gold hairlines: a tracked deep-gold key at 0.7rem over a Cormorant 1.4rem value, links in rose turning charcoal on hover.

### Definition Rows
A description list rendered as rows: term in an 8.5rem column, description beside it with a 1rem gap, 1.1rem padding above and below, cream hairlines between rows and closing the list. Terms are Cormorant 600 at 1.2rem tracked 0.04em uppercase in deep gold; descriptions lead with a charcoal bold line then soft charcoal. Rows stack under 560px.

### Client Roll
Client names set in Cormorant 500 at clamp(1.2rem, 1.8vw, 1.4rem), centred, wrapping, 1.1rem padding either side, with a 4px olive gold dot between neighbours. Two rows, the first 1.8rem below the heading, the second 0.5rem below the first. Under 600px the roll becomes a single centred stack without dots.

### Photograph with Caption
A figure with no margin. The image is served in two sizes with `srcset` and a `sizes` hint matched to its column, `loading="lazy"` on everything except the hero (which carries `fetchpriority="high"`), a fixed aspect ratio, `object-fit: cover` and an explicit `object-position`. The caption is Cormorant italic at 1.05rem in soft charcoal, 0.8rem below, centred under full-width images and left-aligned under column images. Route images brighten 4 percent on hover over 0.3s.

### Route Link
A whole-block link: image (16/10), a Cormorant heading, a soft charcoal paragraph and a tracked deep-gold "Explore" line with a 20px arrow that nudges 4px right on hover over 0.2s. Content stacks at 1rem.

## Do's and Don'ts

### Do:
- **Do** set every section heading as the ruled heading: Cormorant tracked capitals between two 1px gold hairlines, content 2.6rem below.
- **Do** use olive gold (`gold`) for fills, rules, dots and focus rings, and deep olive gold (`gold-2`) for any gold text.
- **Do** keep every corner square (0 radius) and every surface flat; depth is a white sheet or a cream band with a gold hairline edge.
- **Do** separate rows with hairlines (cream inside lists, gold around panels and bands) instead of boxing them in cards.
- **Do** set tracked labels in Lato 700 at 0.68 to 0.78rem, tracked 0.14 to 0.24em, uppercase, in deep gold or soft charcoal.
- **Do** serve every photograph at two sizes with `srcset` and `sizes`, a fixed aspect ratio, `object-fit: cover`, an explicit `object-position`, lazy loading below the hero and an italic Cormorant caption.
- **Do** open with a full-bleed photograph of the real team and the tagline in white capitals over a charcoal gradient rising from the foot.
- **Do** keep WhatsApp and Enquire fixed at the foot of the screen at 800px and under, and give every interactive element the 3px olive gold focus outline.
- **Do** separate short facts with a spaced middle dot.

### Don't:
- **Don't** put a kicker, eyebrow or ornament above a heading; the gold rules are the heading's only ornament.
- **Don't** use stock photography, icon-tile card grids, checkmark trust strips or "most popular" badges; the site's proof is real photographs, named clients and verbatim reviews.
- **Don't** round a corner or cast a shadow; the only radius is the gold dot and the only shadow is the field focus ring.
- **Don't** set olive gold (`gold`) as text on cream, and don't set grey ink (`ink-3`) or rose as small text on the cream-2 or rose tint fields, where both fall under 4.5:1.
- **Don't** use rose for a heading, a button or a rule; it belongs to contact links, errors and the parties field.
- **Don't** set Cormorant below 1.05rem or Lato as a heading; each face keeps its role.
- **Don't** fall back to a system display face; if Cormorant Garamond fails, Georgia is the only substitute.
- **Don't** use an em dash in copy; use the middle dot or a full stop.
