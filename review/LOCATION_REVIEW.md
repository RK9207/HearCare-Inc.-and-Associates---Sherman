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


## User-supplied OAP map replacement

User explicitly supplied a MapLibre GL v4 / OAP map to replace the Google iframe. This supersedes the original embed-preservation requirement for this map only. Insert supplied dependency URLs, proxy, center [-96.6151310,33.6542696], zoom 13, cooperative gestures, red marker, labelled popup, bottom-right navigation and OapMaps.initTracking. Scope card/popup CSS to the location map, preserve the bordered location panel and existing full-width directions action, and add the supplied map-card directions link. Mobile height is now 350px as supplied. Initialization handles normal DOM loading and already-ready documents, guards duplicate initialization, and resizes to layout changes. Keep directions usable with an explicit message if map initialization fails. No change to phone/form hooks, other sections or original appointment script. Local CDN access is blocked; distinguish real failure/layout checks from stubbed integration checks and require actual map/tracking review in GHL. Awaiting rendered review, not locked.


### OAP replacement validation

- Seven blocked-CDN layouts (320–1920px): one new map container, no old Google iframe, no horizontal overflow or uncaught script errors, fallback message and both directions actions available.
- Two stubbed API contract checks (390/1440px): one map construction with the supplied proxy/coordinates/zoom/cooperative gestures, bottom-right navigation, marker/popup setup, OAP tracking invocation, resize observer path, and working existing appointment dialog. These are wiring checks, not evidence of real WebGL rendering, tile availability or analytics delivery.
- Exact source comparison verifies only the location map CSS/markup plus its new stylesheet and scripts changed. Other sections and original appointment/contact script are unchanged.
- Complete HTML artifact matches index.html; inline map JavaScript passes syntax checking.
- Live CDN fetch attempts returned proxy 403 in this workspace. Actual tiles, WebGL controls and tracking delivery remain Needs QA in GHL.

Current OAP fallback layout previews (deliberately blocked dependencies): [desktop](location-oap-fallback-desktop.png), [mobile](location-oap-fallback-mobile.png). Earlier location screenshots above document the prior Google-embed version. No fake map tiles or substituted map screenshots are used.
