# Footer review

User approved Layout A and requested replacing the unresolved year with the current year. Implemented for rendered review, NOT LOCKED.

## Result

A compact darker-navy footer uses three desktop columns: practice identity, Sherman details, useful links. Mobile stacks identity/office and wraps website/privacy links in a short row. The thick white logo frame is removed. The original logo source is preserved and the image retains its natural proportions with a responsive maximum width. Footer type and tap targets remain comfortable, with a restrained copyright divider.

Visible copyright is now “© 2026 HearCare, Inc. and Associates. All rights reserved.” Both unresolved GHL tokens are removed from the footer; no year-update JavaScript is added. Address, hours, Call/SMS data hooks, homepage and privacy destinations are retained exactly. No new promotional claims or CTA is added.

## Checked

- Chromium at 320, 390, 500, 768, 1024, 1440, 1920px; no horizontal overflow.
- Correct 2026 copyright with no raw template token in footer.
- Original footer link tags/destinations preserved; original logo URL and alt text unchanged.
- Computed logo-link background transparent and padding zero.
- Exact source comparison confirms only footer markup/scoped CSS changed. Approved final invitation, location/OAP map, FAQ, payment, options and earlier sections, original scripts and form are unchanged.
- Full review artifact matches index.html; whitespace check passes.
- Cached production font families used for local rendering. External logo requests remain blocked locally, so screenshots show its alt fallback; actual logo appearance needs GHL review using the unchanged hosted asset. No replacement/generated logo is used.
- No calls, texts, external navigation or form submissions performed. Links verified by their destinations, not by sending requests.

## Screenshots

- [Desktop](footer-desktop.png)
- [Mobile](footer-mobile.png)
- [Desktop transition](footer-transition-desktop.png)
- [Mobile transition](footer-transition-mobile.png)

Awaiting rendered approval in GHL. No deployment or merge to main performed.
