# Owners and patient proof — Layout A, awaiting rendered approval

User approved Layout A and headline 1 for both areas: **Meet the people behind HearCare** and **What patients say on Google**.

## Review

- [Desktop](trust-desktop.png)
- [Mobile](trust-mobile.png)
- [Desktop transition from the locked recognition section](trust-transition-desktop.png)
- [Mobile transition](trust-transition-mobile.png)
- [Complete copy-and-paste HTML](hero-review.html), including the unchanged locked sections.

**Portrait limitation:** the local environment cannot fetch the original owner photograph. Screenshots show the explicit unavailable-image fallback, not a substitute portrait. Its original image URL and identities remain unchanged; confirm actual rendering in GHL. The source is 411×411 and is displayed at no more than 300px desktop / 280px mobile, with no crop or generated likeness. Other external form/lead-delivery behavior remains unverified.

## Changes

- Put the heading and shorter owner introduction before the portrait, including on mobile.
- Keep both names, Jill's B.S., and the full shared licensed credential visible. Consolidate repeated licensing statements; preserve complete individual licensing, education and coursework facts in native View qualifications disclosures.
- Retain the practice values as concise supporting context. Do not claim a specific owner will conduct appointments or identify providers as audiologists/doctors.
- Give Google proof a dedicated softly tinted area, compact multicolor Google/4.8/gold-star/90+ aggregate, and three full original quotations: Karyn Feltner, garey gaston and Sandra Walker. The other recorded reviews remain in RESEARCH.md.
- Preserve individual review stars, names, wording, Google destination and listing/experience disclaimer. No quote was rewritten or converted into an outcome guarantee.
- Put Call first and Request Appointment second in a compact closing invitation. Preserve destinations, contact values, data hooks and existing modal.
- On mobile, let the reviews area use the available width rather than nesting narrow cards inside excessive outer gutters. Main prose/review quotations remain 18px.

## Focused verification

Checked at 320, 390, 500, 768, 1024, 1440 and 1920px: no section overflow, exactly three review cards, keyboard Enter opens/closes the first qualification disclosure, appointment trigger opens the existing dialog, Escape closes it and focus returns to its trigger. Selected complete desktop/mobile layouts were visually inspected; actual portrait remains to be checked in GHL. Preview uses the original fonts from an official-source local cache; fixed header/Call overlays are hidden only in section-layout screenshots.

A source comparison confirms all HTML/CSS outside the owners/reviews group is identical to the previous commit: locked Hero and recognition section, header, later sections and integration scripts are unchanged. Verbatim quote checks passed. No lead, call or text was sent. No conversion uplift, live tracking, Lighthouse or successful form delivery is claimed.

PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md and IMAGE_PROMPTS.md reflect this approved rebuild. It is implemented for review, **not locked**. Ask for approval or adjustments; do not automatically advance.

User-supplied portrait hosting update: IMG-PROVIDER-01 now uses https://files.leadconnectorhq.com/file/6af3642f512d2edab67fe078/hearcare-associates-kenneth-jill-sheppard.jpg . Only the image URL changed; authentic portrait identity, dimensions, alt text, lazy loading, crop, image ID and layout are preserved. No live image availability or new resolution is assumed.
