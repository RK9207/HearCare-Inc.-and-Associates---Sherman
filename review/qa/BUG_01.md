# QA bug 1: mobile icon and heading alignment

Reported November 16, 2026 on iPhone Safari, viewport 393×659.

The listening-difficulty panel placed the Missing words and Turning up the TV headings above their icon centers. The tablet breakpoint sets `align-items:start`; the mobile breakpoint restores the side-by-side layout but did not reset that alignment. This affects single-line and wrapping headings differently.

Fix: explicitly use `align-items:center` on the mobile list items below 768px. No HTML, copy, scripts, other styles or integrations changed.

Verification with the production font families in Chromium:

- Baseline 393px: icon/heading center offsets approximately 6.6–6.7px.
- After correction: all three centers match (0px difference) at 320, 360, 375, 390, 393, 414, 430, 500, 639 and 767px.
- Descriptions remain below the icon/heading row; no overflow.
- 768, 1024 and 1440px also checked. Tablet’s intentional icon-above-heading layout and desktop layout are preserved.
- Exact source comparison confirms only one mobile CSS declaration changed, with matching full HTML artifacts.

Actual iPhone/Safari retest remains with QA. Playwright WebKit is not installed in this environment; these measurements do not establish an iOS-device pass.

[Before](bug-01/before-393.png) · [After](bug-01/after-393.png) · [Baseline measurements](bug-01/baseline.json) · [Viewport measurements](bug-01/checks.json)

Proof screenshots hide fixed navigation/Call overlays only during capture so they do not obscure the panel; production styling is unchanged.
