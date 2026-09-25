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
- **Partner link to Group Escape Houses** on the pamper parties page, in a short "group weekends and holiday lets" paragraph. Keep their anchor text "Group Escape Houses" pointing at their pamper party listing, but keep KM's direct enquiry as the primary route so East Midlands visitors aren't sent away. Suggested wording: "Staying in a holiday let, cabin or hotel? We come to you anywhere in the East Midlands. Planning a group weekend elsewhere in the UK? You can also book a pamper party for a group weekend through Group Escape Houses." Section 8.

## 4. Site structure

Real multi-page navigation (not in-page anchors):

- **Home**: hero with two clear routes (workplaces / parties), trust signals, client names, reviews, single call to action.
- **Workplace wellbeing** (corporate): formats (one-off, recurring, large events), how a day runs, benefits, set-up needs (desk vs chair, space required), pricing explanation, client list, case studies, corporate FAQs, enquiry form.
- **Pamper parties**: occasions, per-person pricing, minimum booking, booking terms, gallery/photo, enquiry form.
- **Treatments**: full list with duration and suitable settings.
- **Contact**: enquiry form, WhatsApp, email, areas covered.
- (Optional, on current site) About Us, Gallery, Prices, Testimonials, Blog. Fold into the above unless client wants them separate. The three blog posts work better as case studies on the corporate page.

Keep the current URLs listed in BUSINESS.md section 3, or redirect them at launch, so existing rankings aren't lost.

## 5. Functional requirements

- Enquiry form with fields: enquiry type (workplace day / regular programme / pamper party / individual), name, email or phone, organisation or occasion, number of people, dates/location/notes. Validates name and contact method with a visible error message. Shows a confirmation state. **Real submission destination TBC** (email to client, or form service).
- Pre-selecting the enquiry type when the user arrives from a corporate or party call-to-action.
- WhatsApp link (https://wa.me/44…) wherever WhatsApp is mentioned; opens the app on mobile.
- Mobile menu (hamburger) below ~900px; current page highlighted in the nav.
- Sticky header; on mobile a persistent WhatsApp/Enquire bar is desirable.
- Google review badge linking to the Google Business profile (place ID in BUSINESS.md section 2).
- No em dashes in copy (client preference).
- Outbound partner links (Group Escape Houses) open in a new tab with rel="noopener", stay followed (no nofollow) because they are genuine editorial partners, and sit below KM's own call to action, never in the header or hero.
- noindex on prototypes; remove for launch. SEO basics for launch: page titles, meta descriptions, local keywords (Nottingham, Derby, Leicester, corporate massage, pamper party), Google Business link, schema for LocalBusiness. Current titles and descriptions are in BUSINESS.md section 3 as a baseline.

## 6. Design requirements

- Must look professional and established, and must not look template-generated. Avoid: rounded card grids with icon tiles, checkmark trust strips, "most popular" badges, generic gradient heroes.
- Use the client's real photography (listed in BUSINESS.md section 3) rather than stock. Source photos live in `assets/`; web-sized JPEGs the prototypes reference live in `img/` (two sizes each, served via srcset).
- Client's existing brand: pink, gold, navy, lotus/heart motif, "Holistic Therapy Team" wordmark. New direction may depart from this; four concepts have been produced for the client to choose from:

| Concept | Folder | Direction | Notes / feedback |
|---------|--------|-----------|------------------|
| Plum Edition | `plum/` | Dark plum, blush, gold; bold editorial serif | Adam's preferred direction |
| Blush & Gold | `blush-gold/` | Blush paper, navy ink, gold rules; brochure feel | |
| Classic Edition | `classic/` | The existing site's own brand refined: cream paper, olive gold, Cormorant capitals between rules, real photos | Replaced the earlier "Wellbeing at Work" concept, which read as generic. Adam's feedback: hero photo must not be cropped or upscaled; reviews should lead the proof; keep text minimal |
| Black Apron | `black-apron/` | Built from the team's uniform: black apron cotton, gold arched lettering as on the aprons, tan leather pocket label as the button, brass hairlines. Photo-led, built around the four new location photos | Replaced a "Day Sheet" document-style concept that Adam felt fitted nothing |

- Every concept: single-page-app style routing across the five pages above, self-contained HTML, no build step.

## 7. Open questions for the client

1. Real WhatsApp number, email, phone and social links. Confirm 07891 652 750 and info@kmpamperparties.co.uk from the current site are still correct.
2. Confirmation that all ten corporate clients can be named publicly; logos or names only. Same for RAF Lincolnshire and Microlise, which are already named on the current blog. Would any client give a short quote?
3. Preferred concept, or elements to combine.
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
| 2026-09-25 | Classic hero rebuilt as a split: tagline left, the six-therapist photo right at its own size (no crop, no overlay); reviews moved up to follow the two routes, set in full olive gold with one featured quote; the four "why" points kept as single lines; route and team copy cut to one or two sentences | Adam: heads were cut off, the image looked low quality and oddly sized, the page read as uninspiring, and he wants more focus on the reviews with clean, clutter-free text. The source photos are about 1000px wide, so any full-width hero upscales them; showing the photo at column width keeps it sharp |
