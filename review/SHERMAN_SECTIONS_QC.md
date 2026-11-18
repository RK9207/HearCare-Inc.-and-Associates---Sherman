# Sherman Services and Hearing Aids QA/QC, November 18, 2026

User requested the same follow-up QA/QC already performed on Gainesville. Scope is the two altered Sherman sections only.

Fixed the matching defects: Services choices now reflow to one column when enlarged text cannot fit two; desktop numbering sizes to text; long section text wraps safely. The Hearing Aids CTA row and action group now wrap/shrink within their container and the Call label can wrap while retaining its pill shape. Keyboard focus may scroll into view, with local scroll margins accounting for the sticky header/bottom bar. Replaced figure/figcaption service panel containers with tabpanel-compatible div markup to fix the broader axe aria-allowed-role violation.

Checked after changes:

- Eleven standard widths, 320 through 1920px: all four Services selections/images, exactly one active panel, keyboard arrows/Home/End, breakpoint retention, desktop image-left/mobile choices-first layout, no-JavaScript fallback and no horizontal overflow.
- All four hearing-aid photos decoded at 1448px natural width, four visible cards, eight brands, no hidden style disclosure, pill Call shape and Sherman tel:+19032062442 destinations.
- Existing Sherman appointment dialog opens from Hearing Aids and closes with Escape. Form 8wW1RhQrj7egDZ93IJlJ retained; no Gainesville form or number introduced.
- Twelve stress cases: 280/320/393/768/1024/1440px with 200% root text size or WCAG-style spacing overrides. Neither section has overflowing descendants in those tests.
- Scoped WCAG 2/2.1 A/AA axe passes at 393/1440px. Broader all-rules scoped scan passes at 393px. ARIA links, duplicate IDs and focused last-tab visibility below the sticky header checked.
- Standard desktop/mobile captures generated; Services mobile, Hearing Aids desktop and enlarged-text CTA visually inspected. No page-script errors.

Preservation: complete HTML files are byte-identical; outside Services CSS/markup/script and Hearing Aids CSS, the existing Sherman source is byte-for-byte unchanged, including original CRLF line endings. Gainesville files remain unchanged.

Limitations: exact local illustrative assets and cached fonts were used in fixtures. GHL-host image availability and existing Widex product pixels remain unverified because of the previously observed host proxy block. No live call/SMS/lead submission, real-device test, map-network QA or GHL deployment. This report covers the requested sections, not a new full-page audit.

Evidence: qa/sherman-sections-qc-checks.json, qa/sherman-sections-extended-checks.json and sherman-qc-*.png captures.
