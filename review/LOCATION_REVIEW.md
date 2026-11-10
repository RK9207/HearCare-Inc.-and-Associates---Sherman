# Sherman location section review

User approved Layout A + headline 2, “Find us in Sherman, TX.” Implemented for rendered review, NOT LOCKED.

One bordered rounded white panel combines visit details and the map. Desktop aligns the details and map columns with a divider; mobile stacks address/hours and rounded Call/Text actions above a shorter 280px map, followed by a full-width Get Directions button. Keep Sherman, TX together and the office time range unbroken. Body details remain 18px. The exact source address, opening hours and contact destinations are preserved. No parking, accessibility, travel-time or availability claims are added.

The original Google iframe, its full src and attributes, and original directions link markup/destination are preserved exactly. No replacement map, screenshot, API key or changed place identifier is used. Map retrieval is blocked in the local preview; screenshot checks cover the surrounding layout and iframe sizing. The user’s prior GHL screenshots demonstrate the original map loading, but the shorter revised map should be reviewed in GHL for its final Google controls and pin presentation.

## Checked

- Chromium at 320, 390, 500, 768, 1024, 1440, 1920px; no section horizontal overflow.
- One original map iframe, two contact actions, original directions URL, address and exact hours retained.
- Body paragraph/address sizes compute to 18px at all checked widths.
- Mobile map fixed at 280px; map and directions fit the shared panel.
- Exact source comparison confirms only location-specific HTML/CSS changed. Locked FAQ, payment, options and earlier work, final CTA and integration scripts are unchanged.
- Complete review HTML matches index.html; whitespace check passes.
- No calls, texts, route navigation or form submissions were made. Interactive Google map loading needs GHL QA due to local network restrictions.

## Screenshots

- [Desktop](location-desktop.png)
- [Mobile](location-mobile.png)
- [Desktop transition](location-transition-desktop.png)
- [Mobile transition](location-transition-mobile.png)

Local screenshots use cached production fonts and show a blank reserved map region because the remote map request is blocked. Awaiting rendered GHL review before lock. No deployment or merge performed.
