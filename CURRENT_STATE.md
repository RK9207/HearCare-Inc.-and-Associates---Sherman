# Current implementation and handoff — November 18, 2026

## Latest source override

On November 18, 2026, the user supplied the latest complete page and asked that it be saved for future edits. `index.html` and `review/hero-review.html` derive from the exact landing-page document extracted from that upload’s GHL custom-code container, with the subsequent user-requested Services selector described below. See [LATEST_SOURCE.md](review/LATEST_SOURCE.md) for checksums and archive provenance. This supplied version takes precedence over prior source and historical notes below. Do not automatically reapply older changes. Prior QA results require revalidation against this version; no design or content edits were made during this save.

This summary records the latest user instructions. Historical strategy/source notes remain in their original files; explicit later user decisions supersede earlier proposals. Source evidence and permissions are not interchangeable.

## Page and contact

- Repository: RK9207/HearCare-Inc.-and-Associates---Sherman; review branch codex/hero-redesign.
- Complete GHL copy-paste artifact: review/hero-review.html, identical to index.html.
- Services: hearing tests and hearing aids, Sherman, TX. Real campaign keywords/ad copy remain NOT PROVIDED; keyword candidates are unvalidated.
- Temporary approved Sherman phone: 903-206-2442; tel/sms +19032062442. Do not restore the original brief’s Gainesville number.
- Address: 1800 N. Travis St, Suite D, Sherman, TX 75092. Mon–Thu 9am–5pm; Friday by appointment only.
- One shared GHL appointment form: 8wW1RhQrj7egDZ93IJlJ. Request is not an instantly confirmed booking.

## Current sequence and approval record

On November 11, 2026 the user confirmed “everything looks good” and authorized technical QA. This is whole-page visual approval of the current layout; later changes require new user authorization. Technical corrections are documented in review/TECHNICAL_QA.md. Live integration verification remains separate.

| Section | State |
|---|---|
| Header | Approved. Two-row desktop header, 40px nav gaps, enlarged logo and mobile Explore menu. |
| Hero | Approved. Clean navy hero, enlarged lifestyle photo, current hearing-care/tests H1 and reduced top padding. |
| Listening difficulties | Explicitly approved |
| Services | Approved. Four core service groups; specialized device options live in the style comparison. |
| Owners and Google proof | Approved. Visible credentials and owner caption; verbatim reviews and historical 4.8 / 90+ proof preserved. |
| Process | Approved. Connected steps, phase headings, prominent test disclosure and navy contact strip. |
| Hearing-aid options | Approved. Labelled SmartRIC example, pill manufacturers and six-item style comparison. |
| Payment | Explicitly approved |
| FAQ | Approved. Eight topics and desktop sticky intro. |
| Location | Approved. Integrated storefront/details/OAP map panel; photo caption removed. |
| Final invitation | Explicitly approved |
| Footer | Approved. No logo, deep navy background and automatic year. |
| Appointment dialog | Centered shell passed technical checks; real GHL fields, consent, success and delivery require live QA. |

The current copy/layout is approved. This technical QA pass changes keyboard activation, accessible naming/semantics and functional link contrast only; it removes obsolete internal comments. Visible copy, testimonials, layout, iframe attributes and destinations are preserved.

## Current imagery

- Hero: original kitchen-conversation foreground photo enlarged to fill its column on the clean navy background. Clinic storefront moved to the location section.
- Owners: authentic user-hosted Kenneth/Jill joint portrait. No generated likeness.
- Product: user-hosted Widex SmartRIC example; sharper authorized real imagery remains requested.
- Header: original supplied logo. Footer: no logo at user request.
- Hero foreground URL: https://files.leadconnectorhq.com/file/6af3305fddcd97ce5aa8a0c8/hearcare-kitchen-conversation.webp
- Location storefront URL: https://files.leadconnectorhq.com/file/6af46ff41ca1c60e4d785638/clinic-image.webp
- Owners URL: https://files.leadconnectorhq.com/file/6af3642f512d2edab67fe078/hearcare-associates-kenneth-jill-sheppard.jpg
- Product URL: https://files.leadconnectorhq.com/file/6af44925fbdd54a827b67c4f/widexsmartric.jpg
- No image placeholders are intended as production content. Local blocked-image fallbacks do not establish live image failure.

## Current technical behavior

- Native FAQ/style disclosures and existing dialog; owner qualifications remain visible.
- Mobile/tablet Explore this page menu closes on selection, Escape, outside click or desktop resize; measured header offsets keep section headings clear.
- Core contact/appointment behavior registers before third-party libraries.
- Map assets load near the map viewport; supplied proxy, center, zoom, gestures, navigation, marker and OAP tracking remain.
- OAP tracking invocation is not proof of GA4 call/SMS/form conversion tracking.
- Open in Maps opens a place search; Get Directions retains the existing route destination.
- Footer year updates using the browser’s current year, with 2026 fallback.

## Owner/GHL items

Confirm test fee/typical appointment duration and trial terms; provide better authentic product/owner images; supply real ads/keywords and campaign tracking numbers; refresh Google proof; verify real form fields, consent, validation, delivery and confirmation; verify qualified-call/form events without duplicate conversion reporting. No real lead submitted during local tests.


## Services selector, November 18, 2026

User requested four selectable services and a relevant image on the left, with the headline and supporting copy above. Implemented for rendered review. Desktop uses a left image/caption panel and four right-hand tabs. At 767px and below, a compact two-column selector precedes the image. Active controls use navy/white, with visible keyboard focus. Each service shows its own image and original description. Keyboard arrows, Home/End and roving tab focus are supported; selection survives responsive changes. Without JavaScript all four service panels remain available. Other sections retain the latest uploaded source.

Validation: eleven widths from 320px to 1920px; all four image/tab states, keyboard interaction, resize retention and no-JavaScript fallback passed. Services-scoped axe WCAG A/AA checks passed at 393px and 1440px. Both renders were visually inspected. Local exact image assets and cached fonts were used for browser tests; this is not live-device QA or form-submission testing. Artifacts: review/qa/services-selector-checks.json and review/services-selector-393.png / services-selector-1440.png.


## Services image hosting update, November 18, 2026

Replaced all four Services image sources with the user-supplied GHL Media Library URLs. Image content, dimensions, alt text, layout and selector behavior are unchanged. GitHub asset files remain archived; the current HTML loads these four images from files.leadconnectorhq.com.


## Hearing Aids visual rebuild, November 18, 2026

Hearing Aids now uses a navy product feature with a larger existing Widex photo (2px frame padding), three compact benefit lines, four visible style cards with consistent ear/device placement diagrams, a separate two-column Other options row, the eight-manufacturer strip and a closing contact group. Desktop uses four comparison columns; tablet uses two; mobile uses stacked image/text rows, with full-width visuals below 360px. Inline SVG diagrams are original schematic illustrations, labelled not to scale; they are not manufacturer product photos. Dark body text and visible suitability caveats remain.

User authorized the proposed image-led Hearing Aids restructuring and visual style comparison. Implement only the Hearing Aids section, leaving Services, page order and all other approved sections intact. Replace the expandable text guide with visible comparisons; use accurate, simplified placement diagrams rather than invented product photos. Close with the existing phone and shared appointment-form destinations. Implementation is ready for review; do not infer a new section lock or GHL deployment.

Responsive, scoped accessibility and appointment-dialog checks passed. See review/HEARING_AIDS_VISUAL_REVIEW.md for evidence and the existing Widex-image retrieval limitation.


## Realistic hearing-aid style images, November 18, 2026

User requested realistic close-ups similar to the two supplied ear/device photos, replacing the four graphical diagrams. Replaced all four inline SVGs with AI-generated illustrative photographs: BTE with a thick clear sound tube/custom earmold; RIC with slim behind-ear housing/thin receiver wire; ITE custom shell; a CIC example for the ITC/CIC/IIC family. Original PNGs remain in /workspace/generated_images; WebP copies retain 1448×1086 dimensions and use no retouching. New files: assets/hearing-aid-style-bte.webp, hearing-aid-style-ric.webp, hearing-aid-style-ite.webp, hearing-aid-style-canal.webp. Asset commit b9b32397ea0f4169c620c229f2a0278bacd3dedf provides immutable GitHub raw URLs. These are illustrative scenes, not manufacturer photographs, specific model representations or actual HearCare patients. Visible note: “Illustrative examples. Actual appearance varies.” The canal card identifies its image as a CIC example. Supplied reference photos informed generation; no third-party stock photos were copied into the page.

Cards now show full-width 4:3 photos above the copy at all sizes. Desktop retains four columns, tablet two, mobile one. Explicit dimensions, lazy loading, async decoding and descriptive alt text included. Existing Widex photo, descriptions, caveats, Other options, brands, contact destinations and all other sections are unchanged.


## BTE and RIC image revision, November 18, 2026

User requested a more realistic BTE fit and a visible RIC receiver. Regenerated only these two illustrative photos. BTE uses a rear three-quarter view, smaller partly occluded housing, clear sound tube and earmold. RIC shows a thin wire connected to a receiver and translucent dome at the canal entrance. Both remain 1448×1086 WebP. Originals preserved in /workspace/generated_images/hearing-aid-style-bte-remade.png and hearing-aid-style-ric-remade.png. New immutable image URLs use asset commit 1f43992f7cbddec5500f8e5ef1ccc2290086609e. ITE and canal images, layout, content and contact behavior are unchanged. These remain AI-generated illustrative examples, not verified manufacturer images.
