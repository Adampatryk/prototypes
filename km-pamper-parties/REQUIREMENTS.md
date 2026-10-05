# KM Pamper Parties - Website Requirements

Build spec for the redesign of https://kmpamperparties.co.uk/. Facts about the business, the current site, pricing, treatments and all testimonials live in [BUSINESS.md](BUSINESS.md). This file says what to build and why. Items marked **TBC** need confirming with the client before build.

## 1. Goal of the site

This is a **lead-generation site**. Its single job is to produce enquiries (corporate quotes and party bookings). Everything on the page should either build trust or reduce friction to enquiring.

Secondary goals: look professional and established; make it fast for each audience to find the information relevant to them; work well on mobile (hen party organisers and office managers both browse on phones).

**Why rebuild rather than patch.** The current WordPress site has placeholder headings visible on the homepage, typos in live copy, a broken email link, a WhatsApp button with no number, pricing told three different ways on three pages, a homepage that leads with corporate then parties then corporate again, and stock photography despite the client having real team photos. Details in BUSINESS.md section 3.

## 2. Audiences and what each needs to see

| Audience | Who they are | What they need before they enquire |
|---|---|---|
| Workplace buyer | HR, office manager, wellbeing lead, EA at a company or university | That KM is credible and insured; who else uses them; what a day looks like; space/set-up needed; how pricing works (quoted individually); that regular programmes exist |
| Party organiser | Someone planning a hen do, birthday, baby shower | Prices per person; durations; minimum booking; occasions covered; that it happens at their home/venue; how to book quickly (WhatsApp) |

The homepage must route both audiences within the first screen, without leading with one at the expense of the other (client decision: balanced).

## 3. Content that must appear

Each item points to the source in BUSINESS.md.

- **Two service lines** clearly separated: workplace wellbeing (one-off days, recurring programmes, large events; desk vs chair format) and pamper parties (occasions list). Section 1.
- **Areas covered**: Nottingham, Derby, Leicester headline; full 15-town list on the corporate and contact pages. Section 1.
- **Trust strip**: professional & experienced team · established over 22 years · fully insured · on-site service · tailored to your needs. Section 6.
- **Corporate client names** as a "trusted by" strip on home and workplace pages. Names only until permission is confirmed. Section 7.
- **Per-person pricing table** (20/30/60 minutes) with the 2-hour minimum, on the parties page and reachable from home. Section 5.
- **Corporate pricing disclaimer**, client's own wording, next to any pricing: "Pamper party prices do not apply to corporate massage, wellbeing days or ongoing projects. All corporate enquiries are quoted individually." Section 5.
- **Booking terms** (deposit, full payment 7 days prior, gift vouchers) on the parties page. Section 5.
- **Treatment list** with duration and which settings each suits (workplace vs party). Section 4.
- **Corporate benefits** and the three case studies (RAF Lincolnshire, Hakim Group conference, Microlise) on the workplace page. Sections 6 and 7.
- **Google reviews**, verbatim, with a badge linking to the Google Business profile. Section 7.
- **Contact**: phone, WhatsApp (number shown, deep-linked), email, areas covered. Section 2.
- **Taglines**: "Sit back, relax, and let us take care of you" as the primary; others available for section headings. Section 6.
- **Accommodation partners** on the pamper parties page, as confirmed by Kathleen on 4 Oct 2026: Group Escape Houses (link, wording below), Ashbourne Self Catering (link to https://www.ashbourneselfcatering.com/) and Darley House, Matlock (no link; contact Lucy Arterton, 07719 894 663). An Airbnb profile link will follow. Leave off The Malthouse, The Temple, The Mill Managers and The Old Barn Apartments for now. Details in BUSINESS.md section 8.
- **Group Escape Houses wording** on the pamper parties page, in a short "group weekends and holiday lets" paragraph. Keep their anchor text "Group Escape Houses" pointing at their pamper party listing, but keep KM's direct enquiry as the primary route so East Midlands visitors aren't sent away. Suggested wording: "Staying in a holiday let, cabin or hotel? We come to you anywhere in the East Midlands. Planning a group weekend elsewhere in the UK? You can also book a pamper party for a group weekend through Group Escape Houses." Section 8.

## 4. Site structure

Real multi-page navigation (not in-page anchors):

- **Home**: hero with two clear routes (workplaces / parties), trust signals, client names, reviews, single call to action.
- **Workplace wellbeing** (corporate): formats (one-off, recurring, large events), how a day runs, benefits, set-up needs (desk vs chair, space required), pricing explanation, client list, case studies, corporate FAQs, enquiry form.
- **Pamper parties**: occasions, per-person pricing, minimum booking, booking terms, gallery/photo, enquiry form.
- **Treatments**: full list with duration and suitable settings.
- **Contact**: enquiry form, WhatsApp, email, areas covered.
- **About**: one short page. Kathleen's photo with a "22+ years of experience" badge, a three-sentence story built only from facts on file (co-founder, established over 22 years, a team of twenty-plus, named in every Google review), one verbatim review and a single button to the contact page. To be replaced with Kathleen's own words and preferred portrait (open question 25).
- **Blog**: an index with the newest post featured and earlier posts beneath it; each post is its own page, set in the workplace or party colours to match its subject, and ends with the enquiry form pre-set to that side. Kathleen supplies posts as text plus photos. First entries: the hen party at Red Roofs Barn (new, 4 Oct 2026) and the three posts from the current site (RAF Lincolnshire, Hakim Group conference, Microlise). Inventory and old URLs in BUSINESS.md section 10. The three workplace posts are also linked from "Days on site" on the workplace page.
- (Optional, on current site) About Us, Gallery, Prices, Testimonials. Fold into the above unless client wants them separate.

Keep the current URLs listed in BUSINESS.md section 3, or redirect them at launch, so existing rankings aren't lost.

## 5. Functional requirements

- Enquiry form with fields: enquiry type (workplace day / regular programme / pamper party / individual), name, email or phone, organisation or occasion, number of people, dates/location/notes. Validates name and contact method with a visible error message. Shows a confirmation state. **Real submission destination TBC** (email to client, or form service).
- Pre-selecting the enquiry type when the user arrives from a corporate or party call-to-action.
- WhatsApp link (https://wa.me/44…) wherever WhatsApp is mentioned; opens the app on mobile.
- Mobile menu (hamburger) below ~900px; current page highlighted in the nav.
- Sticky header; on mobile a persistent WhatsApp/Enquire bar is desirable.
- Google review badge linking to the Google Business profile (place ID in BUSINESS.md section 2).
- No em dashes in copy (client preference).
- Outbound partner links (Group Escape Houses, Ashbourne Self Catering) open in a new tab with rel="noopener", stay followed (no nofollow) because they are genuine editorial partners, and sit below KM's own call to action, never in the header or hero.
- noindex on prototypes; remove for launch. SEO basics for launch: page titles, meta descriptions, local keywords (Nottingham, Derby, Leicester, corporate massage, pamper party), Google Business link, schema for LocalBusiness. Current titles and descriptions are in BUSINESS.md section 3 as a baseline.

## 6. Design requirements

- Must look professional and established, and must not look template-generated. Avoid: rounded card grids with icon tiles, checkmark trust strips, "most popular" badges, generic gradient heroes.
- Use the client's real photography (listed in BUSINESS.md section 3) rather than stock. Source photos live in `assets/`; web-sized JPEGs the prototypes reference live in `img/` (two sizes each, served via srcset).
- **Client's brand direction (4 Oct 2026).** Kathleen sent a visual brand sheet (`assets/kmp-brand-sheet.png`) as the starting point for the rebuild, not something to copy exactly. Palette: charcoal black #1A1A1A, warm gold #C9A96A, blush pink #D9B4B0, cream #F7EFE9, white. Type: Playfair Display headings, Montserrat sub headings and body. Logo: a lotus over a three-colour KMP. Feel: professional, warm, luxurious and welcoming, not overly corporate or clinical; cohesive, softer details, premium wellbeing, clean and easy to navigate. Corporate wellbeing gets its own professional identity (Holistic Therapy Team, on-site chair massage, wellbeing days, team building, stress relief, healthier happier teams); pamper parties keep a softer, boutique, welcoming feel. Full notes in BUSINESS.md section 9.
- **Naming.** The business and website stay "KM Pamper Parties / Holistic Therapy Team – Wellbeing Services". "KMP" is the merchandise and event branding. The imagery on the brand sheet is AI-generated and must not be used; the site uses Kathleen's own photographs, which she will send.
- Earlier brand (before the sheet): pink, gold, navy, lotus/heart motif, "Holistic Therapy Team" wordmark. Five concepts have been produced:

| Concept | Folder | Direction | Notes / feedback |
|---------|--------|-----------|------------------|
| Plum Edition | `plum/` | Dark plum, blush, gold; bold editorial serif | Adam's preferred direction |
| Blush & Gold | `blush-gold/` | Blush paper, navy ink, gold rules; brochure feel | |
| Classic Edition | `classic/` | The existing site's own brand refined: cream paper, olive gold, Cormorant capitals between rules, real photos | Replaced the earlier "Wellbeing at Work" concept, which read as generic. Adam's feedback: hero photo must not be cropped or upscaled; reviews should lead the proof; keep text minimal |
| KMP Collection | `kmp-collection/` | Built from Kathleen's brand sheet: apron charcoal, warm gold, blush and cream; the lotus KMP lockup centred in a charcoal header; a single calm home hero (tagline, one sentence naming both sides, a charcoal and gold button for workplaces and a blush button for parties, the team photo); Playfair Display and Montserrat; ribbon lines at the foot of dark and blush bands. Workplace pages run in charcoal and gold, party pages in blush; the header and the "Pamper Parties" title under the logo are identical on every page, and the workplace and parties heroes are the same height | The first concept that follows the client's own direction. Uses the existing real photos until Kathleen sends hers |
| Black Apron | `black-apron/` | Built from the team's uniform: black apron cotton, gold arched lettering as on the aprons, tan leather pocket label as the button, brass hairlines. Photo-led, built around the four new location photos | Replaced a "Day Sheet" document-style concept that Adam felt fitted nothing |

- Every concept: single-page-app style routing across the five pages above, self-contained HTML, no build step.

## 7. Open questions for the client

1. Real WhatsApp number, email, phone and social links. Confirm 07891 652 750 and info@kmpamperparties.co.uk from the current site are still correct.
2. Confirmation that all ten corporate clients can be named publicly; logos or names only. Same for RAF Lincolnshire and Microlise, which are already named on the current blog. Would any client give a short quote?
3. Preferred concept, or elements to combine. Since the brand sheet arrived, the question is mostly whether the KMP Collection concept reads the sheet the way Kathleen intends.
4. Where enquiry form submissions should go.
5. Any treatments to add or remove; confirm durations. Keep the manicure/pedicure and men's facial lines?
6. Keep the Amethyst / Sapphire / Diamond packages, or move to per-person pricing only?
7. Whether individual (non-party) mobile bookings should be promoted or kept quiet.
8. Gift vouchers: sold online or by enquiry only?
9. Domain and hosting for launch. Current site is WordPress hosted by Vitty; who holds the domain and hosting login?
10. "Award-winning" appears on the current site. Which award, and can we cite it?
11. Does "established over 22 years" refer to Kathleen's practice or the KM Pamper Parties business?
12. Deposit amount and cancellation policy, so booking terms can be stated clearly.
13. Is there an existing Google Analytics / Search Console property (Site Kit is installed) to carry over?
14. Group Escape Houses: their listing doesn't name KM or link back, and shows a different package and price. Is KM the supplier behind it for East Midlands bookings? Can Kathleen ask them for a named listing and a link to kmpamperparties.co.uk in return? Is there a similar arrangement with Forest Holidays (Sherwood Pines)?

15. Logo artwork: can Kathleen send the KMP lotus logo as vector files (SVG, AI or PDF), in the dark and light versions? The prototype redraws it in code.
16. Should the KMP mark lead the website header, given the business name stays KM Pamper Parties? The prototype uses the KMP lockup with "Pamper Parties" and "Holistic Therapy Team" beneath it, and "KM Pamper Parties" in the footer and page titles.
17. Original photographs for the build: events, pamper parties, corporate bookings and the team, ideally including the new aprons, banners and backdrops once they exist.
18. Airbnb profile link, due once the profile is live.
19. Which straplines are approved for the site: "Restore · Recharge · Reconnect", "Restoring People · Empowering Teams · Brighter Workplaces", "Invest in your team's wellbeing", "Relax · Rejuvenate"?
20. The current site has 44 further articles that are live but hidden from its blog page (generic how-to guides such as "How to Host the Ultimate DIY Spa Party at Home", around 2,000 words each, with illustrative rather than original images). Migrate, redirect to the new blog, or drop? They were not brought into the prototype.
21. Red Roofs Farm or Red Roofs Barn? Kathleen's suggested title says Farm; her text and a notice in her photo say Barn. The prototype uses Barn.
22. Answered 4 Oct 2026 (Adam): the hen party guests are happy to be pictured.
23. The RAF post cites another massage provider's blog (atworkwellbeing.co.uk) as its source for "Studies indicate…". Keep the link, point it at an independent source, or remove it? Answered 4 Oct 2026 (Adam): keep the links.
24. Three photos from the Microlise post were left out because they are mainly Microlise branding (logo wall, banner, Queen's Award plaque). Add them back once Microlise has agreed to its name and logo being used?
25. About page: can Kathleen send her own short story (how she started, who she co-founded the business with, what she enjoys about the work) and a portrait she is happy with? Answered 4 Oct 2026: Adam supplied a portrait of Kathleen standing in front of a wall mural, which the prototype now uses after clean-up (see BUSINESS.md section 10). Her own story in her own words is still needed.
26. Is Lesley Gilchrist (Elite Athlete Centre and Hotel, Loughborough University) happy for her feedback to appear on the site with her name, job title and employer?
27. Hakim Group 2026 post: add the organiser's feedback when Kathleen receives it. Are the four delegates in the massage photo happy to be pictured? The post says "KMP Pamper Parties" throughout; should posts use that or "KM Pamper Parties"?

## 8. Decisions log

| Date | Decision | Why |
|------|----------|-----|
| 2026-09-25 | Produced three homepage concepts for review | Give the client a real choice of direction rather than one design |
| 2026-09-25 | Homepage routes both audiences equally | Client decision: balanced, not corporate-first or party-first |
| 2026-09-25 | Names only for corporate clients until permission confirmed | Avoid using logos without consent |
| 2026-09-25 | Split requirements into REQUIREMENTS.md (build spec) and BUSINESS.md (reference) | Spec was buried under testimonials and audit detail |
| 2026-09-25 | Replaced the Wellbeing at Work concept with Classic Edition, based on the current site's brand | Adam found the teal concept generic; the client's existing look, done well, is a fairer third option |
| 2026-09-25 | Photos moved out of the HTML into a shared `img/` folder | Four new full-size photos supplied; inline base64 would have tripled every page |
| 2026-09-25 | Added a fourth concept, Black Apron, built from the therapists' uniform and the four new location photos | Adam rejected a first attempt (Day Sheet, a document-style concept) as fitting nothing; the aprons in every photo are the one consistent piece of brand the client already owns |
| 2026-10-04 | Added a fifth concept, KMP Collection, built from the client's own brand sheet | Kathleen sent her brand and website style direction; this is the first concept that starts from it rather than from our reading of the old brand |
| 2026-10-04 | Added a Blog to the KMP Collection concept: Kathleen's new hen party post plus the three posts shown on the current site's blog page, carried over word for word | Kathleen sent a first new post with six photos, and asked for the existing posts to sit beneath it as older entries |
| 2026-10-04 | Post titles keep the author's title case; everything else on the site stays sentence case | The titles are Kathleen's published content and existing search listings, not interface headings |
| 2026-10-04 | The 44 hidden articles on the current site were not migrated | They are not listed on its blog page, read as generic search-engine filler, and use non-original images; left as an open question |
| 2026-10-04 | Added a favicon to the KMP Collection concept: the lotus from the KMP mark on apron charcoal, over a short gold line | Adam asked for one; the lotus is the part of Kathleen's logo that still reads at tab size |
| 2026-10-04 | Added a simple About page, "Meet Kathleen", and an About link in the header, phone menu and footer | Adam asked for a very simple page with her picture and a short story; nothing in the story goes beyond facts already on file |
| 2026-10-04 | KMP Collection home page cut to five parts: tagline, the two banners, a three-item trust line, one review with the Google link and client names, and one closing call to action | Adam found the page a bit too busy. Removed: the one-line descriptions inside each banner, the heart rule, two of five trust items, two of three reviews and their heading, the team photo and paragraph (now covered by the About page), and the closing sentence and WhatsApp button (WhatsApp stays in the phone bar and footer). About 290 words down to about 130 |
| 2026-10-04 | About page portrait replaced with a close-up selfie and given a "22+ years of experience" badge | Adam asked for a better picture and a quick badge; the earlier full-length photo was low resolution. "More than 22 years of experience" is Kathleen's own wording in her hen party post |
| 2026-10-04 | KMP Collection home page: the two-colour split screen replaced by one hero. Tagline, one sentence that names the business and both sides, two buttons in the sides' colours, and the team photo | Adam found the split screen busy and was not a fan of it. The two sides are still stated in the first sentence and routed by two equal buttons, which keeps the client's "balanced" decision |
| 2026-10-04 | Page changes in the KMP Collection concept cross-fade, the header stays still, the phone menu eases in, and Back returns to the previous scroll position | Adam asked for switching between pages to feel more fluid. Uses the browser's view transitions with a plain fade as fallback; switched off for reduced-motion users |
| 2026-10-04 | Hen party post now leads with the photo of the four guests, on the blog page and at the top of the post | Adam asked for a better photo for the latest post; the previous lead was a dark close-up of the couch |
| 2026-10-04 | About page uses the portrait Adam supplied of Kathleen in front of a wall mural, cropped, cleaned and sharpened | Adam chose this photo and asked for its quality to be improved. The wall behind her carried a company's mission statement and she wore a visitor pass, so the lettering was removed from the background and the pass blurred; the face was not retouched beyond sharpening and a light exposure lift |
| 2026-10-04 | The title under the header logo no longer changes on workplace pages; it reads "Pamper Parties" everywhere | Adam did not like it switching to "Holistic Therapy Team" between pages. The workplace page still names the Holistic Therapy Team in its intro and keeps its charcoal and gold colours, which is how it carries the separate identity Kathleen asked for |
| 2026-10-04 | Workplace and parties heroes share one portrait photo shape (4:5), so they are the same height | Adam preferred the taller workplace hero and wanted the two to match. The parties hero now uses the hen party welcome sign, because the landscape SPA letters photo loses a letter when cropped to portrait |
| 2026-10-04 | KMP Collection audited with the impeccable skill (15/20) and the findings fixed: focus and a screen-reader announcement on each page change, photos on other pages load only when needed, no text under 12px, all colours held as named tokens, the enquiry error tied to its field, 44px tap targets, and reduced-motion keeps colour feedback | Adam asked for a mini design audit and then for the fixes. Fonts are still served by Google; self-host them in the production build |
| 2026-10-04 | Accommodation partners section holds three entries: Group Escape Houses, Ashbourne Self Catering, Darley House | Kathleen checked which providers actually link to or refer guests to her; the others give out her email directly, so they stay off for now |
| 2026-09-25 | Classic hero rebuilt as a split: tagline left, the six-therapist photo right at its own size (no crop, no overlay); reviews moved up to follow the two routes, set in full olive gold with one featured quote; the four "why" points kept as single lines; route and team copy cut to one or two sentences | Adam: heads were cut off, the image looked low quality and oddly sized, the page read as uninspiring, and he wants more focus on the reviews with clean, clutter-free text. The source photos are about 1000px wide, so any full-width hero upscales them; showing the photo at column width keeps it sharp |
