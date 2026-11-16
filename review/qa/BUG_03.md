# QA bug 3: consistent practice-name formatting

Reported November 16, 2026.

Canonical page-controlled name: **HearCare, Inc. and Associates**.

Corrections:

- Map address-card title now includes the comma.
- Map marker popup uses the same full name.
- Review-source note now says “Reviews from the Google listing for HearCare, Inc. and Associates…” instead of reproducing the Google listing’s different display-name format.

Header alt/accessible text, page title, owner introduction, address, photo alt text and copyright already used the canonical format. Short brand references to HearCare remain appropriate. Supplied logo/storefront artwork, URLs and exact testimonial quotations are unchanged.

Checked at 393, 753 and 1440px: canonical name in rendered map card, address, review note and footer; no horizontal overflow or page-script errors. Exact comparisons preserve all destination URLs and blockquotes. Marker popup string and all inline JavaScript syntax checked. No layout or other code changes.

[Rendered checks](bug-03/checks.json) · [Map card proof](bug-03/map-card-393.png)

The external Google Business Profile has not been renamed or independently reverified in this update. Its owner should review the preferred public display name separately. The attribution wording does not claim that the profile’s exact display name was changed.
