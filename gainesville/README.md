# Gainesville page visual updates

The user's uploaded Gainesville HTML is the source of truth. The original is preserved at source/2026-11-18-user-upload.html.

Applied the reusable Services and Hearing Aids redesign from the Sherman reference at dc0a162e5d422ed259c7ce64aceaa9ee90888888. Complete HTML: index.html and review/gainesville-review.html, identical. These are separate Gainesville artifacts; the Sherman page remains unchanged.

Only Services CSS/markup/new independent selector script, Hearing Aids CSS/markup, and the shared Call CTA pill radius changed. All other uploaded content, integrations, map, office details, hero, reviews and header are preserved. New contact actions use Gainesville 903-206-1692, tel/sms +19032061692 and its existing form FVRo140VXNTnGQ3deRJi. Added wording refers to Gainesville, not Sherman.

Services: headline above, four selectable service images/descriptions, desktop left photo and right choices, mobile 2×2 choices above photo, keyboard navigation, resize retention and no-JavaScript fallback. Hearing Aids: larger Widex feature, concise benefits, four realistic style photos including revised BTE/RIC, separate Other options with local-availability/specialist caveats, existing eight brands and closing contact group. Shared Call CTAs use a 999px pill radius; the mobile sticky bar remains unchanged.

All eight new illustrative WebP photos use the user-supplied GHL URLs. They are AI-generated examples, not actual practice patients or manufacturer model photography. Image notes and accessibility labels remain in place.

Original upload SHA-256: 43923f2b5766e82f29ca1d854fdc35b55b19c6350e70917266abdec2696efcf8

For a full reusable design and asset specification, see ../review/REUSABLE_SECTION_CHANGES.md. This source change does not deploy to GHL.

Validation passed across eleven widths, all selector states, no-JavaScript fallback, photo decoding, Gainesville contact destinations, appointment dialog, scoped accessibility checks and desktop/mobile visual review. See review/QA.md for evidence and external-host limitations.

Follow-up QA/QC fixed enlarged-text reflow, wrapping CTA controls, keyboard focus visibility and valid Services tabpanel markup. See review/QA.md and review/qa/extended-qc-checks.json.


## Mobile Menu label, November 23, 2026

User requested “Menu” with a hamburger icon instead of “Explore this page” with an arrow, for both mobile versions. The saved sources already used a hamburger-only header toggle; added the visible Menu text and adjusted its pill control to fit the label plus icon. The closed control shows the hamburger; the expanded control retains its close icon. Existing aria-expanded/controls, Escape focus return, section-link dismissal, contact links and desktop navigation are preserved. Both pages passed interaction/header-fit checks at 320, 393, 768, 1024 and 1440px. HTML artifact pairs match. No deployment to GHL.
