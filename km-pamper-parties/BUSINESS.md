# KM Pamper Parties - What we know

Reference material about the business, the current website and the content available for the new one. Grows as the client answers questions. The build spec is in [REQUIREMENTS.md](REQUIREMENTS.md).

Sources: audit of https://kmpamperparties.co.uk/ on 25 Sep 2026, the client's own homepage design, photos supplied, and the client's list of corporate customers. Items marked **TBC** need confirming with the client.

## 1. The business

**Trading names:** KM Pamper Parties · Holistic Therapy Team · "Massage, Beauty & Wellbeing Services". Co-founded by KM (Kathleen), who is the therapist named in every review.

**What they do:** Mobile massage, beauty and wellbeing treatments delivered at the client's location. Two audiences, one team.

1. **Corporate / workplace wellbeing**: on-site chair massage and wellbeing treatments for businesses, universities, colleges, conferences and events. Delivered as one-off wellbeing days, larger multi-therapist events, or **recurring programmes** (monthly or fortnightly visits are common). Current site offers two formats: **desk massage** (short, at the employee's desk) and **seated chair massage** (therapist brings a chair; needs a small, ideally secluded space). Corporate quotes are based on number of staff and time per person.
2. **Pamper parties and special occasions**: hen parties, birthdays, baby showers, girls' nights in, Mother's Day, couples ("Time Out for 2"), pregnancy massage, gift vouchers. Delivered at the client's home, holiday accommodation or venue. Additional therapists available for larger parties.

Individual mobile appointments are also offered (implicit on current site; reviews mention couples booked at a Forest Holidays cabin at Sherwood Pines).

**Where:** East Midlands. Nottingham, Derby, Leicester headline everywhere. The corporate page lists 15 areas covered: Leicester, Lincoln, Grantham, Boston, Nottingham, Mansfield, Kettering, Melton Mowbray, Derby, Chesterfield, Worksop, Hinckley, Northampton, Loughborough, Corby. Mobile service; the team comes to the client.

**Credentials:**
- Established over 22 years (client's design). Not stated on the current site.
- Team of 20+ therapists (per group photo). Current site says "team" and "additional therapist available for larger parties".
- Fully insured (client's design). Current site says "fully qualified" and "highly trained" but not "insured".
- 5.0 rating from 7 Google reviews (verified on current site via Trustindex widget).
- Current site claims "our award-winning Pamper Parties East Midlands service". **TBC:** which award, and whether it can be cited.

**Corporate clients:** see section 7, social proof.

## 2. Contact details

| Channel | Current site | Client brief | Use in build |
|---|---|---|---|
| Phone | 07891 652 750 | TBC | Use 07891 652 750, confirm with client |
| WhatsApp | Button only, number hidden | TBC (placeholder 07700 900123 in prototypes) | Confirm it's the same 07891 number, then deep-link to wa.me/447891652750 |
| Email | info@kmpamperparties.co.uk | TBC (placeholder hello@) | Use info@, confirm with client |
| Facebook, Instagram, LinkedIn | Not found | TBC | Get URLs from client |
| Twitter/X | Not found in this audit | Brief says @kmpamperparties exists | Confirm whether still active; drop if not |

**Google Business place ID:** ChIJPbNj01L5gS4R5uGWW4tK2kU
- Profile: https://www.google.com/maps/place/?q=place_id:ChIJPbNj01L5gS4R5uGWW4tK2kU
- Write a review: https://search.google.com/local/writereview?placeid=ChIJPbNj01L5gS4R5uGWW4tK2kU

## 3. Current website

**Platform:** WordPress with Elementor 4.3 and WP Rocket caching. Footer reads "Copyright © 2024 | KM Pamper Parties" and "Website hosted by Vitty". Google Site Kit installed, so there is likely an existing Analytics / Search Console property to carry over.

**Pages and navigation:** Home · Massage and Beauty Treatments · Pamper Parties · Corporate Massage · Testimonials · Blog · Contact.

| Page | URL |
|------|-----|
| Home | / |
| Treatments | /massage-and-beauty-treatments/ |
| Pamper parties | /pamper-party-packages/ (nav links to /pamper-parties/) |
| Corporate | /corporate-massage/ |
| Testimonials | /testimonials/ |
| Blog | /blog/ |
| Contact | /contact/ |

**Current SEO baseline:**
- Title: "Pamper Parties & Corporate Massage | East Midlands Experts"
- Description: "Mobile pamper parties, corporate massage, hen do treatments & beauty services across the East Midlands. Book professional, relaxing sessions at home or work."
- Sub-page titles follow "Pamper Party Packages East Midlands | KM Pamper Parties" and "Corporate Massage East Midlands | Workplace Wellbeing".

**Visual style today:** fonts Cormorant (headings), Roboto, Roboto Slab and Lato. Dominant colours are an olive gold (#897600), a bright pink (#fa9fff), off-white (#f8f6f1) and grey text (#54595f). Imagery is generic stock spa photography (hot stone, facial, back massage) plus a couple of real photos from 2023 (couples massage, mother and daughter) and one 2025 photo of a chair massage in an office. Logo file is a small square "Group-1" PNG.

**Existing brand assets:** pink, gold, navy, lotus/heart motif, "Holistic Therapy Team" wordmark. Real photography supplied by the client: team photo at the Hakim Group wellbeing day (six therapists, thumbs up), full-team group photo (20+) seated in a conference hall, two therapists beside a pink "Massages" sign at a client's offices, two therapists outside a branded hospitality truck at a golf event (third-party branding visible, so not to be captioned as a client), chair massage under the "Wellbeing at Work" neon, SPA marquee letters at a party. Sources in `assets/`, web sizes in `img/`.

**Current enquiry form fields:** full name, pamper party location, date, number of people, duration (2, 3, 4 or 5 hours), email, contact number.

**Known defects:** three "Add Your Heading Text Here" Elementor placeholder headings on the homepage; typos in live copy ("Hamman", "rime", "area's"); a mailto link pointing at an IP address; WhatsApp promoted but number never shown; pricing told three different ways across three pages; homepage leads with corporate, then parties, then corporate again; stock photography despite real team photos existing.

## 4. Treatments

From the client's brief: aromatherapy / full body massage · back massage · seated chair massage (workplace) · hot stone massage · Indian head massage · facials · reflexology · pregnancy massage · Hammam experience.

Also on the current site, **TBC** whether to keep:
- Deep tissue massage (with warming oils)
- Back to Life Hammam therapy (shower paste, body scrub, mud mask, hot steam, hot oil back/neck/shoulder massage). Minimum 60 minutes.
- Organic facial, deluxe organic facial (serum mask, balm facial massage, head/neck/shoulder massage), organic Cosmos facial for men
- Express manicure, express pedicure, foot therapy (peppermint, ginger and lavender foot massage, hard skin removal, cuticle care)
- Free essential oil upgrade on back massage; optional aromatherapy oils on pregnancy massage

Current site descriptions worth reusing:
- Indian head massage: suits thinning hair, migraines and stress
- Pregnancy massage: "fully qualified and experienced pregnancy massage therapists work together with mum to ensure she is happy at all times"
- Facials: every treatment begins with a consultation; suits all skin types

## 5. Pricing and booking terms

### Pamper party pricing (per person, per treatment)

| Duration | Price | Current site's description |
|---|---|---|
| 20 minutes | £24 | Shorter treatments, or an add-on to build a longer tailored slot |
| 30 minutes | £35 | Most popular. Back massage, Indian head massage or a facial |
| 60 minutes | £65 | Full body massage, Hammam experience, or a combination such as massage plus facial |

Minimum booking time: **2 hours**. Perfect for birthdays, hen parties, baby showers and special occasions.

**Disclaimer (client's own wording):** Pamper party prices do not apply to corporate massage, wellbeing days or ongoing projects. All corporate enquiries are quoted individually.

**Booking terms (current site):** deposit required on booking; full payment due 7 days before the party. Gift vouchers available by enquiry. Packages page also says "Prices start from £60".

### Named packages on the current site (TBC: keep, simplify or drop)

| Package | Group | Time | Includes | Price |
|---|---|---|---|---|
| Amethyst | 1 to 4 people | 2 hrs | Back massage 30, facial massage 30, mani or pedi 30, Indian head 30 | £150 |
| Sapphire ("most popular") | 3 to 6 people | 3 hrs | Full body 60, luxury facial 60, reflexology 30, mani or pedi 30 | £180 |
| Diamond | 4 to 8 people | 4 hrs | Aromatherapy 30, hot stones 60, Back to Life 60, facial 30, reflexology 30, mani and pedi 30 | £240 |

Occasion packages are all "pick & mix" from the treatment list: Hen Party Pick & Mix · Girls Night In · I Love You Mum · Mum to Be (baby shower, pregnancy massage) · Time Out for 2 (two therapists treat two people at once).

## 6. Messaging

### Corporate benefits (from client's design)

Boosts wellbeing and morale · supports a healthier, more productive team · reduces stress and absenteeism · ideal for offices, events and ongoing projects.

Current site adds: rewards and recognises the team; helps staff cope with deadlines; therapists understand staff need to get back to work and leave people "lively and refreshed".

### Trust strip (client's own)

Professional & experienced team · established over 22 years · fully insured · on-site service · tailored to your needs.

### Taglines in use

"Sit back, relax, and let us take care of you" (also the current site's hero line) · "A happier, healthier you" · "Wellbeing at Work" · "Take time for you" · "Relax · Recharge · Feel Amazing" · "For people · for teams · for every occasion".

Current site's own headline: "Professional Massage Wellbeing & Pamper Services Across the East Midlands".

## 7. Social proof

Everything we can use to show that real organisations and real people book KM. Names only until the client confirms permission (see REQUIREMENTS.md open questions).

### Corporate client list

Supplied by the client on 25 Sep 2026, in her own words: "List of current and recent company's I work with for corporate, businesses universities & colleges where I provide my wellbeing massage services."

| Businesses | Universities and colleges |
|---|---|
| Mosca | Loughborough University |
| Miniclip | Leicester University |
| Homes By Honey | Loughborough College |
| Hakim Group | |
| PR Eden | |
| SDL Surveying | |
| Rank Interactive Ltd | |

Also evidenced on the current site's blog and testimonials, not on the client's list:
- RAF Lincolnshire (training day wellbeing session)
- Microlise (Eastwood, Nottingham, corporate wellbeing day)

Suggested use: a "Trusted by" strip on the home and workplace pages, with the three education names grouped so university and college buyers see their peers. Hakim Group doubles as a case study (2,000+ attendee conference) and a written testimonial, so it can lead.

**TBC:** written permission to name each publicly; whether logos may be used; whether any client would give a short quote or act as a reference.

### Google reviews
 (verbatim, all 5 stars, 7 in total)

- **Andrea Wilson**: "We use Kathleen for seated corporate massages at work and she is WONDERFUL! An exceptional masseuse as well as a genuinely lovely person. Would absolutely recommend her to anyone :)"
- **Sam Ryman**: "We use KM for corporate massages at work, Kathleen has helped so many of us with aches and pains! The best service you'll find anywhere! And such lovely people!"
- **Steff Ryman**: "Thank you so much Kathleen, your kind, caring nature made me feel so at ease. Your massages are amazing and have really helped my back. Highly recommend to anyone"
- **Amy Duffield**: "I can highly recommend Kathleen. She really cares about giving an amazing experience and is such a lovely lady too."
- **Denise Barker**: "I have the pleasure of having Kathleen come to my workplace once a month to provide massages for myself and my colleagues, courtesy of the company. I can confidently say that she gives an exceptional massage, one of the best I've ever experienced! Kathleen's skills and professionalism truly stand out, making each session a wonderful break from our busy workdays."
- **Gaye Tytherley**: "Kathleen is exceptional. Such a talented massage therapist and a genuinely wonderful lady. We use her for our corporate massages and I also personally had a pamper party. The massages are heavenly! She is totally reliable, very well priced and gives a high quality service. 100% recommend"
- **Jodie Piggin**: "Myself and my Partner booked for a 30 minute each deep tissue massage with Kathleen. Kathleen came to our cabin based at Sherwood Pines, which was booked by Forest Holiday. Kathleen was very polite, well organised and would definitely recommend. We will certainly book again."

### Other testimonials on the current Testimonials page (not Google, source TBC)

- **Hakim Group** (annual retreat 2024): "A professional, well organised service and run smoothly with great outcome from the weekend conference retreat"
- **Charlotte** (workplace wellbeing day): "She made me feel really comfortable and the massage was brilliant. I felt much more relaxed"
- **Jodie Piggin** (hen party): "Kathleen & her team of therapists were professional, friendly, knowledgeable and lots of experience"
- **Bianca Louise**, **Ramartha**, **Gertrude Sandy**, **Grethel Gayle** (Shiningford Manor), Natalie's pamper party guests, and a couples booking at Sherwood Forest Holidays. Short, positive, mostly about pain relief and the therapists being warm.

### Case studies (current blog, reusable as corporate proof)

- RAF Lincolnshire: onsite chair massages at a training day wellbeing session (post dated 26 Mar 2025)
- Hakim Group annual conference, Dec 2024, Telford International Centre, 2,000+ optical professionals (20 Mar 2025)
- Microlise, Eastwood, Nottingham: corporate wellbeing day with chair massage (27 Feb 2025)

## 8. Partners and referral channels

### Group Escape Houses

A UK-wide discovery and booking platform for large group holiday homes and add-on experiences (hen parties, birthdays, corporate retreats). They list a pamper party package at https://www.groupescapehouses.co.uk/experiences/pamper-party-package and Kathleen says they are advertising her package through it.

On 25 Sep 2026 they asked Kathleen to add this line to the KM site, with "Group Escape Houses" linked to the listing above:

> Book a pamper party for a group weekend through Group Escape Houses.

Kathleen is happy for us to change the placement or wording for SEO.

**What the listing actually says (checked 25 Sep 2026):**
- Does not mention KM Pamper Parties by name and does not link to kmpamperparties.co.uk.
- Describes a generic package: mini facial, hand massage, manicure or polish, light makeup touch-up. 3 to 4 hours, up to 16 guests, several therapists at once.
- Priced £70 to £78 per guest including VAT, by group size. KM's own per-person pricing is £24 to £65 per treatment.
- Coverage listed as Brighton, Bath, London, Cotswolds, Lake District and others. East Midlands not called out.
- Stock spa photography, no reviews.

So as it stands the link is one-way: it sends KM's visitors and link equity to the platform, and the platform gives KM no visible credit. It is still a genuine referral channel for group weekend bookings, and Kathleen wants the relationship, so the link goes in. The ask back is a named listing and a backlink (see REQUIREMENTS.md open question 14).

### Forest Holidays / Sherwood Pines

Not a confirmed partner, but a Google review says a couples booking at a Sherwood Pines cabin "was booked by Forest Holiday". Worth asking whether there is an arrangement worth naming, since it is the same holiday-let channel as Group Escape Houses but local.
