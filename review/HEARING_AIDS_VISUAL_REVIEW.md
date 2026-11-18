# Hearing Aids visual rebuild, November 18, 2026

User authorized the previously proposed visual restructure. The navy product feature retains the approved headline, shorter benefits, existing Widex image and 2px image-frame padding. Four always-visible comparison cards use original inline SVG placement illustrations. Other options retain both suitability/availability caveats. All eight manufacturers remain. One closing contact group uses the existing phone and shared appointment form.

Checked: eleven widths (320, 360, 393, 540, 767, 768, 1024, 1100, 1200, 1440, 1920px), no horizontal overflow, four visible diagrams/cards, eight manufacturers, no hidden style disclosure, working appointment dialog and Escape close. Services GHL URLs remain intact. Both HTML artifacts match. Outside Hearing Aids markup/CSS, the page is byte-identical to the prior version. Scoped axe WCAG 2/2.1 A/AA checks return zero violations at 393 and 1440px. Diagrams and spacing visually inspected at both widths. Cached fonts and blocked unrelated requests were used in browser fixtures.

Needs GHL review: existing Widex photo pixels could not be fetched because the execution proxy rejects files.leadconnectorhq.com with CONNECT 403. Screenshots therefore show its reserved frame and alt text, not a verified image render. Its URL is unchanged. No live leads, calls or SMS were submitted. This is not real-device testing or a deployment.

Artifacts: hearing-aids-visual-393.png, hearing-aids-visual-1440.png and qa/hearing-aids-visual-checks.json. Ready for user review; no new lock inferred.
