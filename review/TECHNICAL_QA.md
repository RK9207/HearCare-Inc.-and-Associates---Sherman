# Technical QA: HearCare Sherman

Date: November 11, 2026 (Asia/Calcutta)

Status: locally testable page checks passed after corrections. Live GHL integrations still need verification. The user approved the current visual design before this audit.

## Corrections made

1. Appointment CTAs use button semantics. Added Space-key activation so they work with both Space and Enter.
2. Functional blue links on pale-blue backgrounds measured 4.44:1, just below the 4.5:1 WCAG AA requirement. Changed the functional blue from #2578b2 to #1f6fa6, producing 5.05:1 on #f2f8fc.
3. Corrected the Google-rating and Open in Maps accessible names to include their visible wording, supporting speech-input users.
4. Added a region role to the labelled reviews container so its accessible name has valid semantics.
5. Removed obsolete internal build-note comments from the production HTML. The current project documentation remains in the repository.

Visible copy, approved layout, testimonials, phone numbers, URLs, iframe configuration/consent attributes and map settings are preserved. Only the functional blue shade changes visually.

## Checked

| Area | Result |
|---|---|
| Responsive layout | No horizontal overflow at 320, 360, 390, 500, 639, 768, 1024, 1199, 1200, 1280, 1440 and 1920px; also checked 844×390 landscape. |
| Page structure | One H1, language/viewport/title/description present, no duplicate IDs, valid internal anchor targets and ARIA label references, all local SVG references resolve. |
| Navigation | All seven destinations tested; headings remain clear of the measured sticky header. Mobile menu closes after selection and on Escape, with focus returned. |
| Disclosures | All main-page disclosures open and close by keyboard. |
| Appointment shell | Every CTA opens with Space; click activation, close button, Escape, scroll lock and focus restoration pass. Native modal prevents focus moving to background page controls; browser chrome remains reachable. Mobile/landscape dialog stays within viewport with scrollable body. |
| Form fallbacks | Hosted-form href preserved without JavaScript; unsupported-dialog fallback targets the hosted form in a new tab. |
| Accessibility scans | Axe WCAG 2 A/AA and 2.1 A/AA scans reported zero violations in the tested page and open-dialog states at 390px and 1440px after fixes. Embedded form fields were not available to scan. |
| Gradient contrast review | Conservative luminance calculations: hero white 7.36:1; hero eyebrow 5.10:1; white on navy CTA 9.62:1. This supplements axe’s incomplete gradient checks. |
| Reduced motion | Smooth scrolling disabled when reduced motion is requested; FAQ sticky behavior respects the existing reduced-motion condition. |
| Contact links | All marked Call/SMS anchors resolve to the approved +19032062442 destinations. No real calls/messages were made. |
| New-tab links | Existing target=_blank links include rel=noopener. |
| Map failure | Dependency failure shows the fallback message while Open in Maps/Get Directions remain available. |
| Map initialization contract | With mocked MapLibre/OAP APIs, verified deferred loading near viewport, single initialization, container ID, center [-96.615131, 33.6542696], zoom 13, cooperative gestures, bottom-right controls, marker and proxy. OAP tracking initialization invoked once. This does not verify real tile or tracking transport. |
| Year | Current year renders; simulated January 2027 renders 2027. |
| Performance/source | Hero remains high priority; supporting images remain lazy with dimensions/aspect ratios. Map assets remain deferred. Font requests retain display=swap. Production HTML is about 115 KiB before transport compression; cached original hero is about 187 KiB. Remote asset sizes/cache headers were not measured. |
| Runtime | No page JavaScript exceptions in the tested fixtures; inline JavaScript syntax passes; whitespace/diff checks pass. index.html and review/hero-review.html match exactly. |

## Live checks still required

The GHL preview and third-party assets could not be retrieved directly in this environment. Browser tests used the cached original hero/fonts and deliberately blocked external services, with a separate mocked map-contract test. Real services have not been certified by these tests.

- Open the latest HTML in GHL and confirm every hosted image, font, favicon and real map tile loads. Check iOS Safari as well as Chrome; automated browser testing used Chromium only.
- Complete an authorized test submission in the real embedded form: field validation, consent controls, keyboard navigation, success/thank-you state, CRM delivery and notifications. Confirm field alignment inside the GHL form builder. No lead was submitted in this audit.
- Confirm the approved number actually receives calls and SMS, especially if tracking-number substitution is enabled.
- Verify real call/SMS/form conversion events, campaign attribution and absence of duplicate reporting. OAP map tracking initialization does not establish these conversion events.
- Confirm published URL, canonical/indexing settings and SEO values in GHL. Source metadata exists; the title is 75 characters and description 169 characters, so snippets may truncate. Shortening them is optional and was not done during this technical pass.

## Evidence

- [Viewport and interaction results](qa/results.json)
- [Mobile accessibility scan](qa/axe-390.json)
- [Desktop accessibility scan](qa/axe-1440.json)
- [Open-dialog accessibility scans](qa/axe-dialog.json)
- [Contrast calculations](qa/contrast-manual.json)
- [Mocked map contract](qa/map-contract.json)
- [Future year and fallback checks](qa/extra-checks.json)
- [Motion and backdrop checks](qa/motion-backdrop.json)

Test harnesses are retained in the current workspace at /workspace/work/qa_hearcare.cjs, qa_hearcare_extra.cjs and qa_hearcare_dialog.cjs. They depend on the session’s cached assets and local Playwright/axe setup. No production analytics, forms, contacts or external application state were mutated by the tests.
