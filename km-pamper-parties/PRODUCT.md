# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Self-contained static HTML/CSS/JS prototypes, one file per concept, hash routing across five "pages", no build step, hosted on GitHub Pages. Production build target is a real multi-page site (platform TBC). Recorded from REQUIREMENTS.md.

## Users

- **Workplace buyer.** HR, office manager, wellbeing lead or EA at a company, university or college in the East Midlands. Planning a one-off wellbeing day, a conference or event, or a recurring monthly/fortnightly programme. Often browsing on a phone between other tasks. Needs before enquiring: that KM is credible and insured, who else uses them, what a day looks like, the space and set-up needed, that pricing is quoted individually, that regular programmes exist.
- **Party organiser.** Someone planning a hen do, birthday, baby shower, Mother's Day, girls' night in or a couples treat, at home, a holiday let or a venue. Browsing on a phone. Needs: per-person prices, durations, the 2-hour minimum, occasions covered, that it happens at their venue, and a fast way to book (WhatsApp).
- Client decision: the homepage routes both audiences within the first screen, balanced, neither leading.

## Product Purpose

Lead-generation website for KM Pamper Parties (trading names: KM Pamper Parties, Holistic Therapy Team, "Massage, Beauty & Wellbeing Services"), a mobile massage, beauty and wellbeing service across the East Midlands. Its single job is to produce enquiries: corporate quotes and party bookings. Success is enquiries via the form or WhatsApp. Secondary goals: look professional and established, route each audience fast, work well on mobile. It replaces a WordPress/Elementor site with placeholder headings, typos, a broken email link, pricing told three ways and stock photography.

## Positioning

One crew of twenty-plus qualified, insured therapists, co-founded by KM (Kathleen), established over 22 years, that comes to the client: office, venue or home. The same team scales from a night in with six friends to a 2,000-attendee conference (Hakim Group, Telford International Centre, Dec 2024). Every Google review names Kathleen personally. Named workplace clients: Loughborough University, University of Leicester, Loughborough College, Miniclip, Hakim Group, Mosca, SDL Surveying, Rank Interactive, Homes By Honey, PR Eden (names only until permission is confirmed; RAF Lincolnshire and Microlise appear on the current blog).

## Operating Context

- Mobile service. The team brings chairs, couches, towels, music and a sign-up sheet.
- Workplace formats: desk massage (short, at the desk) or seated chair massage (needs a quiet ~2m x 2m space and a plug socket per therapist). Fully clothed, no oils, 15 to 20 minute slots, roughly 18 to 24 people per therapist per day. Delivered as one-off wellbeing days, multi-therapist events, or recurring programmes with one monthly invoice. Corporate work is quoted per therapist per session on hours and headcount.
- Parties: guests pick and mix treatments in 20, 30 or 60 minute slots at £24, £35 or £65 per person. Minimum booking 2 hours. Deposit on booking, full payment 7 days before. Gift vouchers by enquiry. Additional therapists for larger parties.
- Areas: Nottingham, Derby, Leicester headline. Full list: Leicester, Lincoln, Grantham, Boston, Nottingham, Mansfield, Kettering, Melton Mowbray, Derby, Chesterfield, Worksop, Hinckley, Northampton, Loughborough, Corby.
- Contact channels: enquiry form, WhatsApp (deep link, number must be shown), email, phone.

## Capabilities and Constraints

- Pages: Home, Workplace wellbeing, Pamper parties, Treatments, Contact. Prototypes simulate these with hash routing in one file. Production keeps or redirects the current URLs.
- Enquiry form: type (workplace day / regular programme / pamper party / individual), name, email or phone, organisation or occasion, headcount, dates/location/notes. Validates name and contact method with a visible message, shows a confirmation state, pre-selects type when arriving from a corporate or party CTA. Submission destination TBC.
- Sticky header; hamburger menu below ~900px; current page highlighted; persistent WhatsApp/Enquire bar on mobile desirable.
- Google review badge linking to the Google Business profile (place ID ChIJPbNj01L5gS4R5uGWW4tK2kU).
- Copy: no em dashes. Prototypes are noindex.
- Mandatory disclaimer beside any pricing, client's wording: "Pamper party prices do not apply to corporate massage, wellbeing days or ongoing projects. All corporate enquiries are quoted individually."
- Treatments with duration and suitable setting: aromatherapy/full body, back, seated chair, hot stone, Indian head, facials, reflexology, pregnancy massage, Hammam experience. TBC whether to keep deep tissue, Back to Life Hammam, organic facials, express manicure/pedicure, foot therapy, and the Amethyst/Sapphire/Diamond packages.
- Undecided, do not invent: real phone, WhatsApp, email and social links (prototypes use placeholder 07700 900123 and hello@; the current site shows 07891 652 750 and info@); client-name permission and logo use; whether individual bookings are promoted; gift vouchers online or by enquiry; the "award-winning" claim; whether "22 years" is Kathleen's practice or the business; deposit amount and cancellation policy; analytics carry-over.

## Brand Commitments

- Names: "KM Pamper Parties", "Holistic Therapy Team". Co-founder KM (Kathleen) is named in every review.
- Existing identity: pink, gold, navy, a lotus/heart motif, "Holistic Therapy Team" wordmark. The client is open to a new direction; three concepts are being compared.
- Taglines available: "Sit back, relax, and let us take care of you" (primary), "A happier, healthier you", "Wellbeing at Work", "Take time for you", "Relax · Recharge · Feel Amazing", "For people · for teams · for every occasion".
- Must look professional and established and must not look template-generated. Avoid rounded card grids with icon tiles, checkmark trust strips, "most popular" badges, generic gradient heroes.
- Real photography only, no stock.

## Evidence on Hand

- Photos (full-size sources in `assets/`, web-sized JPEGs with `-sm` variants in `img/`, referenced by every prototype via srcset): six therapists giving a thumbs up at a Hakim Group wellbeing day (`team-six`, plus `team-six-hero` portrait and `team-six-wide` landscape crops); the full team of twenty-plus seated in a conference hall (`team-all`); two therapists beside a pink "Massages" sign at a client's offices (`spa-pair`); two therapists outside a branded hospitality truck at a golf event (`event-truck`, the truck carries a third-party brand, so caption it as "a golf event", not as a client); a seated chair massage under a "Wellbeing at Work" neon sign (`chair-massage`, has baked-in text); SPA marquee letters and balloons at a party (`spa-letters`). All sources are around 1000 to 1450px on the long edge, so avoid layouts that stretch one photo beyond about 1200px wide. No other imagery exists; do not use stock.
- Seven verbatim 5-star Google reviews and other testimonials, in BUSINESS.md.
- Case studies: RAF Lincolnshire training-day wellbeing session (Mar 2025); Hakim Group annual conference, Telford, Dec 2024, 2,000+ attendees; Microlise, Eastwood, corporate wellbeing day (Feb 2025).
- Absent: client logos, an award citation, corporate prices. None may be fabricated.

## Product Principles

1. Every element either builds trust or reduces friction to enquiring.
2. Both audiences are routed equally in the first screen.
3. Proof over claims: real photos, named clients, verbatim reviews, concrete facts (22 years, 20+ therapists, 5.0 from 7 reviews).
4. Pricing is told once, consistently, with the corporate disclaimer beside it.
5. Phone-first: WhatsApp reachable everywhere, primary actions in the thumb zone.

## Accessibility & Inclusion

WCAG AA text contrast, keyboard-operable navigation, menu and form, visible focus states, reduced-motion respected, meaningful alt text on the real photos.
