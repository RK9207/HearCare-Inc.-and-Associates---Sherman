# Process section review

User direction: Layout A with headline 4, “Know what to expect before your visit.” Implemented for rendered review; not locked pending user approval.

Two phases distinguish the hearing test and explained results from optional hearing-aid selection, fitting and ongoing support. Four numbered steps remain. Descriptions use full width below headings on mobile; body and test-detail text remain 18px. A white canvas follows the tinted proof section, with a navy contact band and rounded Call/Appointment buttons plus a distinct Text link.

Original test-type disclosure, its not-every-visit qualification, medical-treatment caveat, contact destinations, tracking hooks and appointment integration are preserved. No new image is needed. PAGE_STRATEGY.md, CONTENT_DIRECTION.md and DESIGN_SYSTEM.md record the approved direction.

## Checked

- Chromium rendering at 320, 390, 500, 768, 1024, 1440 and 1920px; no section overflow collapsed or expanded.
- Four numbered steps and correct tel, sms and existing appointment destinations.
- Keyboard disclosure opening/closing; appointment dialog opening, Escape closing and focus return.
- Exact source comparison confirms all content outside process markup and process-specific CSS is unchanged, including the three locked sections, header and shared integration scripts.
- Complete copy-paste artifact matches index.html.

## Review artifacts

- [Desktop](process-desktop.png)
- [Mobile](process-mobile.png)
- [Desktop transition](process-transition-desktop.png)
- [Mobile transition](process-transition-mobile.png)
- [Expanded mobile test details](process-tests-mobile.png)

Local rendering used cached production font families. Remote owner photo and logo access remain blocked locally; original hosted URLs are preserved. These process screenshots contain no replacement imagery. No calls, texts or form submissions were made. External form field loading and lead delivery require GHL QA.
