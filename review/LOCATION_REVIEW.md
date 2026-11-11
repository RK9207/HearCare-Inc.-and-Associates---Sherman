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


User-requested label adjustment: change only the map address-card link to “Open in Maps” and align its accessible label. Preserve its existing Google Maps destination and the separate Get Directions button.


## User-requested larger map

Increase the desktop map minimum height to 520px, tablet minimum to 460px, and mobile height to 450px. Allocate a larger desktop map share (4fr details / 7fr map) and reduce map-column padding to 16px on desktop/tablet. Preserve mobile full-width map, marker coordinates, zoom, OAP tracking, map card including Open in Maps, all links and all other page content. Existing ResizeObserver continues to resize MapLibre with its container. Source-scope checks confirm only location CSS changed; index and complete HTML artifact match before publication. The execution environment failed startup, so no new browser rendering or live map test was possible for this sizing revision; GHL screenshot review remains required. Location section is not locked.


User-requested directions-button styling: apply brand navy background/border (#004a69), white text and icon, and deeper navy hover (#003a53), scoped only to the location map’s Get Directions button. Other buttons, map card, destinations and sizing unchanged. Index and full HTML artifact match; exact replacement scope verified. No new browser-rendering claim for this color-only adjustment.


## Sherman location final approval

User: “looks good, lets move to the next section, I approve this section.” Location implementation as of 7d363a12eb3b9c2177a639ade734d3195287b46c is APPROVED / LOCKED, including the bordered details/map panel, supplied OAP/MapLibre integration, enlarged responsive map, Open in Maps card link and dark-blue Get Directions button. Preserve without further user authorization. Next proposed section: existing final contact invitation, to connect the completed visit-planning information to Call, Text and Request Appointment. Request current desktop/mobile screenshots showing the complete invitation and actions, and wait before individual review or editing. No HTML/CSS changes accompany this approval record.


## User-approved separation of hero and clinic imagery

After reviewing the real GHL screenshot, user approved removing the competing clinic background and moving the authentic storefront photo to the location section, and requested a larger foreground hero image. Restore the clean navy hero background; foreground lifestyle photo fills its desktop column (previously 90%/490px cap) with 40px top offset retained. Mobile/tablet photo uses full content width and existing spacing. Add a separate uncropped storefront figure below the existing location/map panel, with “Look for the HearCare sign” and the verified address. Keep map dimensions, original location details/directions, headline, CTA links and all other content/integrations unchanged. Clinic photo loads lazily. Awaiting rendered review.


## User-requested location rebuild for desktop and mobile

Integrate the standalone clinic photograph with office details/map into one rounded panel. Move the unchanged Find us in Sherman, TX heading above the panel, add a brief visit-planning introduction, place full uncropped storefront plus sign caption/address/hours/Call/Text on the left and the large OAP map/dark Directions action on the right. Use dark body copy, balanced borders and full-width recognizable image. Desktop address/hours sit side by side; tablet combines image/details above the map; mobile stacks heading, full-width photo, office details, actions, 450px map and Directions. Compact map address card leaves more of the route visible; keep Open in Maps label. Preserve exact map DOM, ID, proxy/center/zoom/gestures/tracking initialization, destinations, hours, contact hooks and hero/other sections. Awaiting rendered review.

Validation: eleven widths from 320–1920px passed overflow, single-photo/single-map and tap-height checks. Full-width mobile photo precedes details; map remains 450px on mobile and at least 520px on desktop. Final 390px/1440px checks confirm 52px buttons; mobile Call/Text stack to prevent number wrapping. Exact source checks preserve original address/hours list, contact/maps destinations, map DOM and all scripts, plus every other main section. Local image/tile retrieval blocked; actual storefront and OAP tile rendering require GHL preview review. No calls, messages or leads sent.
