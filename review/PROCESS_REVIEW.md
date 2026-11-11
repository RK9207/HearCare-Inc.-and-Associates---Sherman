# Process section review

User direction: Layout A with headline 4, “Know what to expect before your visit.” Implemented for rendered review; not locked pending user approval.

Two phases distinguish the hearing test and explained results from optional hearing-aid selection, fitting and ongoing support. Four numbered steps remain. Descriptions use full width below headings on mobile; body and test-detail text remain 18px. A white canvas follows the tinted proof section, with a pale-blue contact panel and rounded Call/Appointment buttons plus a distinct Text link.

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

## Visual refinement requested after GHL screenshot

Stronger navy/pale-blue phase headers, white equal-height panels, subtle shadows, outlined step numbers and internal dividers improve hierarchy. A short sky accent introduces the heading; the medical caveat gains a quiet left rule. The light contact panel aligns all three desktop actions in one row and stacks buttons on mobile. No wording, markup, heading sizes or integration changed. Exact source comparison verified only process-specific CSS changed in the page. Repeated seven-width overflow and keyboard interaction checks passed. Updated screenshots show the revision. Awaiting user review; not locked.


User requested a more visible “Which tests might be included?” disclosure. Add a pale-blue surface, stronger 2px blue border, larger title, explicit expansion hint and white chevron inside a navy circle. Preserve the native details behavior, original question and all existing test descriptions/qualifications. Style only this process disclosure; retain all other sections and integrations. Awaiting rendered review.


User requested removal of forced headline/prompt breaks. Remove process CTA prompt’s 350px width cap and allow the contact row to wrap as a group when text/buttons need space. Hero heading spans flow inline with normal wrapping; remove nonbreaking location phrasing in hero and location heading. Retain semantic address/hours line breaks, wording, font sizes, contacts and integrations. Awaiting rendered review.


## User-requested process visual redesign

Refine only the visit/process section following the supplied screenshot: replace heavy header bars with inset phase headings and small Start here / If you choose to proceed labels; use white and pale-blue phase surfaces, connected filled step markers, aligned descriptions, softer borders and restrained depth. Retain all original four-step copy, clinical caveat and prominent tests disclosure. Give the contact strip a navy gradient with light prompt, white appointment outline and existing sky Call action; preserve natural wrapping and all contact/form links. Mobile stacks the same content with comfortable spacing and dark body text on pale surfaces. Awaiting rendered review.

Validation: nine-width browser checks (320–1920px) passed with no page overflow, all four steps present, dark text on pale-blue surfaces and light CTA text. Native test disclosure pointer/keyboard controls and appointment-dialog Escape/focus restoration passed. Exact comparison confirms original copy, contact URLs and scripts/integrations preserved; only process CSS plus two phase labels changed. No real calls, texts or form submissions.
