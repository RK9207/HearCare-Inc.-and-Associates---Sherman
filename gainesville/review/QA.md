# Gainesville visual section QA, November 18, 2026

Checked the adapted page at 320, 360, 393, 540, 767, 768, 1024, 1100, 1200, 1440 and 1920px. Services: four selections show exactly one panel, correct ARIA selected state, distinct decoded images, arrow/Home/End keyboard controls, selection retention across breakpoints, headline above, photo left on desktop and choices above photo on mobile. Without JavaScript all four service panels remain available.

Hearing Aids: four loaded 1448px WebP images, four visible comparison cards, no hidden style dropdown, eight manufacturer names. All shared Call CTAs have a 999px radius and Gainesville tel:+19032061692 destination. The Hearing Aids appointment action opens the existing Gainesville dialog and Escape closes it. Scoped axe WCAG 2/2.1 A/AA checks return no violations at 393/1440px. No horizontal overflow at tested widths or page-script errors. Desktop/mobile renders of both sections visually inspected.

Preservation: normalizing only the two authorized CSS/section blocks and shared Call radius confirms all other uploaded source is preserved exactly apart from normalized line endings. All Gainesville form, phone, map, location, review and existing content outside scope remain intact. No Sherman phone/form was introduced. The original upload is archived. index.html and review/gainesville-review.html match.

Limitations: browser fixtures serve exact local files for the eight illustrative images plus cached fonts, blocking unrelated network calls. The GHL host was blocked in prior checks; live GHL image availability and existing Widex product pixels are not verified. Widex reserved frame/alt text appears in the captures. No real call/SMS/lead submission, map network check, real-device test or GHL deployment occurred. This is scoped QA of the requested changes, not a new whole-page audit.


## Follow-up QA/QC and fixes, November 18, 2026

Scope: Gainesville Services and Hearing Aids only. This is a further audit after the initial adaptation.

Found and fixed:

1. At enlarged text sizes, two-column Services choices overflowed on narrow screens. Tiles now automatically use one column when the available space cannot accommodate readable two-column choices. Normal mobile widths retain two columns. Long text wraps safely. Desktop number tracks now size to their text rather than a fixed 28px.
2. Enlarged Hearing Aids contact controls could push outside tablet/mobile containers. The CTA row and action group now wrap and shrink safely, and the Call label can wrap if necessary. Pill shape and Gainesville destinations are retained.
3. Keyboard activation used preventScroll, potentially leaving focused tabs out of view. Keyboard focus can now scroll into view; scoped scroll margins account for the sticky header and bottom call area. Checked that the fourth tab is visible below the header after End.
4. The broader axe scan flagged role=tabpanel on a figure element (aria-allowed-role). Replaced the service panel figure/figcaption elements with labelled tabpanel-compatible div containers, retaining image alt text, captions and identical styling. The broader scoped scan now returns zero violations.

Verified after fixes: all four Services states/images, keyboard controls, correct ARIA relationships, no duplicate IDs, breakpoint selection retention, no-JavaScript content fallback, four hearing aid photos, eight brands, pill Call shape, local phone links and appointment dialog including Escape. Eleven standard widths from 320 to 1920px passed. Twelve additional stress cases passed: 280, 320, 393, 768, 1024 and 1440px with 200% root text sizing or WCAG-style text-spacing overrides (1.5 line height, .12em letter spacing, .16em word spacing and 2em paragraph margin). No overflow inside either section in those stress cases. Scoped WCAG A/AA checks passed at 393 and 1440px; a broader all-rules scoped axe run passed at 393px. Standard desktop/mobile captures regenerated, enlarged-text service choices and CTA visually reviewed. No layout/content redesign outside the requested sections.

The two complete Gainesville HTML copies match. The Sherman page remains unchanged. All external-image/network limitations listed above still apply; exact local assets and cached fonts were used. No real calls, SMS, leads, real-device test or GHL deployment occurred.
