# Whole-page improvement audit — November 11, 2026

Baseline: 0137f36 (latest page implementation). Audit only: no index.html, review/hero-review.html, approved copy, styles or integrations changed.

## Overall judgment

The page covers the essential decision journey: local services and relevance, listening difficulties, real owners and patient evidence, testing and conditional device care, suitable options, payment help, practical FAQs, location and contact. More sections are not the main opportunity. Prioritize clinical wording accuracy, a verified appointment/measurement journey, less repetition on mobile, and stronger authentic product/local imagery.

## Scope and evidence limits

Reviewed the current source and project brief, AGENTS.md, RESEARCH.md, KEYWORD_RESEARCH.md, PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, IMAGE_PROMPTS.md, README.md and section review notes. Current explicit user approvals supersede historical instructions and appended implementation notes. Existing GHL screenshots in the conversation establish actual asset/map appearance; fresh local rendering supplies current layout metrics.

Direct website fetches timed out for the homepage, primary service/location pages, team, fitting and repair. Site-restricted search returned indexed current-domain content for services, hearing aids, fitting, testing, pricing and Sherman location, plus older www-domain material. These results are useful comparisons, not a claim that every live page was freshly fetched successfully. Older www pages have conflicting Friday-hours statements and are not used to alter the newer location-page facts. External form content could not be retrieved. Local tests intentionally blocked external form/map scripts and unavailable image hosts; actual network performance, analytics delivery, map tiles and form fields/lead submission remain unverified. Local fonts used cached production families, and the supplied hero asset was cached. Broken local logo/portrait/product images do not establish production image failures.

## Checked local rendering

Widths: 320, 390, 768, 1200 and 1440px, viewport height 844px. No horizontal document overflow, duplicate IDs or broken internal anchors. One main H1; clear section headings. Appointment dialog opens at all widths. Its real embedded fields and success states were not exercised; no lead, call or SMS was sent.

At 390px, local document height is approximately 13,618px (about 16 viewport heights). At 1440px it is approximately 8,040px. These are local layout observations, not live performance or conversion measurements; missing externally hosted images and GHL wrappers can affect exact heights. First hero Call link begins around y=534px on mobile and y=529px on desktop. The global mobile Call bar and header appointment link provide earlier paths. There is no basis to claim the CTA is inaccessible above the fold.

The largest mobile groups are owners/reviews (~2,380px), options (~2,156px) and process (~2,099px). Together they account for around half of this local mobile page. Keep readable type; reduce redundant explanations before reducing font size or removing useful verified information.

## Priority 1 — accurate and measurable conversion path

### 1. Review inherited clinical descriptions

Evidence: index.html's test disclosure says tympanometry can show earwax buildup. The style guide describes BTE and RIC mainly as moderate-to-severe options, calls RIC wireless connectivity standard, and makes generalized battery-life statements for ITE. These came from client website material, but source provenance alone does not validate a broad clinical/device claim.

NIDCD describes BTE use across mild-to-profound loss. ASHA distinguishes otoscopy/ear canal examination from middle-ear measurement. Recommend clinician review of these two disclosures and model-dependent feature statements. Safer copy direction: explain what the test measures, make suitability depend on assessment and model, and avoid universal wireless/battery claims. Do not invent a service or claim that this practice performs an unverified examination. The relevant sections are locked or awaiting final review; seek user approval before changing them.

Sources: https://www.nidcd.nih.gov/health/hearing-aids ; https://www.asha.org/practice-portal/clinical-topics/hearing-loss ; https://www.asha.org/Practice-Portal/Professional-Issues/Adult-Hearing-Screening/ . These inform a content correction, not individualized medical advice.

### 2. Finish the real appointment-form QA

The dialog shell works. The supplied form has not yet been fully inspected in GHL. Check real field labels, required-field validation, consent/privacy text, submission state, scrolling with the phone keyboard open, error recovery and the confirmation message. Confirm that submitting creates the intended lead/notification and remains an appointment request rather than a guaranteed time-slot booking. No live submission was authorized during this audit.

### 3. Verify conversion tracking independently of map tracking

Source contains telephone/SMS/appointment data hooks and OapMaps.initTracking(map), but no explicit call/SMS/form conversion event implementation in this HTML. Host-level tracking may already exist; its absence from the file is not proof of absence in GHL.

Verify phone clicks, SMS clicks, appointment starts, successful form completions and qualified-call outcomes. Keep clicks distinct from actual leads and avoid duplicate event firing. Verify current Sherman number and future campaign replacements consistently across rendered links, call tracking and SMS capability.

### 4. Confirm essential missing appointment facts

Test fee, typical appointment length, named provider assignment, specific insurance participation and trial conditions are still not confirmed by the project sources. Obtain clinic facts before publishing numbers, named staffing promises or coverage statements. These are potentially valuable practical answers, not reasons to invent another generic FAQ.

## Priority 2 — content and visual improvements

### 5. Tighten repetition in the middle of the page

Testing first, appropriate hearing aids, personalized fit, phone setup and follow-ups appear across Hero, process, options, payment and FAQs. Some repetition supports scanning; whole explanations need not recur.

Preserve the section sequence and benefits. Make process explain the sequence; options explain appearance/comfort/usefulness; FAQ answer residual objections briefly. Keep all attributed review wording verbatim. A shorter default view with optional supporting detail is preferable to smaller type. Do not remove approved sections, shrink the user-requested map or hide necessary service/location facts without approval.

### 6. Give aftercare a clearer benefit

The website services/fitting pages emphasize continuing adjustments and setup support. Current stage 4 and FAQ include them but the process paragraph bundles too many details. Surface one concise reassurance about help after fitting, with the existing detail available below. No claims of free lifetime care, warranty or unlimited adjustments.

Sources: https://hearcareinc.com/services/ ; https://hearcareinc.com/services/hearing-aid-fitting/ . Indexed website content was available; direct fetches timed out.

### 7. Replace the weak product asset

Current product source is a 232×253 clinic-hosted Widex image. It is labelled as an example and not greatly enlarged, but it remains low resolution, brand-specific and visually less polished than the hero. Prioritize a licensed high-resolution real in-hand photograph or authorized manufacturer image; rehost in GHL and retain honest scale and model-specific qualifications. Keep authentic imagery instead of generating an inaccurate device. The existing photo has been seen loading in user screenshots, so this is a quality improvement rather than a confirmed broken-image issue.

The actual owner photo is another high-value upgrade: request the original larger file while preserving both identities. Optional authentic Sherman exterior/interior photography could add local confidence when obtained and approved; do not add another stock image just to fill space.

### 8. Preserve the strong first screen and prove changes with data

Hero already identifies hearing tests/hearing aids and Sherman, states the practical benefit, shows the real phone and local facts, and supplies trust. Do not redesign its approved headline merely to repeat a keyword. Once real ad groups and ad copy arrive, verify service/location/offer continuity and consider separate test-led versus device-led variants only if campaign data supports them. KEYWORD_RESEARCH.md correctly labels all candidates unvalidated.

### 9. Add navigation access on narrow screens only if needed

The six desktop section anchors are appropriate and valid. Below 1200px the navigation is hidden by existing design, consistent with the original mobile brief. Given the long page, an optional compact “Page sections” menu may help returning readers reach pricing, FAQs or location without scrolling. This is an enhancement, not a defect or an instruction to crowd the approved mobile header. Test a menu against screen-space and accessibility needs before adopting it.

## Priority 3 — performance, polish and maintainability

### 10. Load the map after essential contact behavior

MapLibre and OAP scripts are synchronous at the end of the body before the appointment handler is registered. Slow map/script requests can delay the enhanced appointment dialog even though a basic form-link fallback remains available. Initialize core interactions first and load/initialize the map near its viewport. Preserve the enlarged map dimensions, supplied proxy, marker and tracking behavior. Recheck callback ordering and resize behavior after any change. Pin compatible dependency versions where practical; do not change the user-supplied OAP integration blindly. No network timings or Core Web Vitals were measured.

The hidden cross-origin appointment iframe is eagerly present; evaluate its real network cost and whether provider-supported loading-on-demand is safe before altering it. Google Fonts already uses display=swap and the Hero has dimensions/high fetch priority—keep those good choices.

### 11. Keep external actions semantically distinct

The map-card link labelled Open in Maps currently retains a directions-route URL. Consider a direct place/listing URL for that label while retaining the separate Get Directions route button. Preserve the same practice/place identifier. Add the known brand favicon through the GHL host if not already configured; source HTML has no favicon link, but host settings may supply one.

Refresh the displayed 4.8/90+ Google aggregate before launch; its current evidence is user-supplied screenshots, not a new live review lookup. Retain the approved 90+ presentation while verifying it remains accurate. Do not rewrite testimonials or invent review images.

### 12. Consolidate the project documents

PAGE_STRATEGY.md's early tracker still describes only the first three sections as locked and process as the current section, while later notes correctly record more approvals. IMAGE_PROMPTS.md's opening inventory still mentions placeholders, old hosts and pending Hero review; later notes supersede them. Section review files often open with “not locked” before final approval notes.

Create a clearly dated current-state summary and approval table, then preserve older decisions under an archive/history heading. Keep the original brief and historical research evidence intact. Process, latest header, footer and the appointment popup do not all have explicit final rendered sign-offs; don't infer them. Update the asset register to current URLs and the footer-logo removal. Distinguish current implementation from pending opportunities and GHL-only QA.

## What to keep

- Current overall page sequence, local emphasis and test-first conditional pathway.
- Prominent real Call/Text actions, consistent appointment destination and sticky mobile Call bar.
- Owner credentials accurately described as Licensed Fitters and Dispensers, not unsupported doctor/audiologist titles.
- Authentic owner image and verbatim attributed reviews.
- Insurer-enquiry help with coverage qualifications, payment transparency and the preparation FAQ.
- User-approved bordered designs, larger map, dark footer and automatic year.
- Existing no-guarantee approach: no fabricated price, trial terms, callback time or medical outcomes.

## Suggested order of work

First: clinician-approved wording corrections, real form/lead QA and tracking verification. Second: targeted repetition reduction plus an authentic high-resolution product photo. Third: map-loading performance, optional narrow-screen navigation, and document consolidation. No new long sections are recommended.

## Audit artifacts

- Metrics and checks: full-page-audit-checks.json
- Desktop layout: full-page-audit-desktop.png
- Mobile layout: full-page-audit-mobile.png

The screenshots deliberately show local asset/network fallback states and are not substitutes for a fresh GHL full-page test. All recommendations affecting approved sections remain proposals. No production page or approved section was changed in this audit.
