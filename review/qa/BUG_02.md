# QA bug 2: Samsung Galaxy Tab S8 icon and heading alignment

Reported November 16, 2026: Android Chrome, viewport 753×1037.

This is the same inherited mobile alignment defect as bug 1. The reported 753px viewport uses the below-768px layout, so the existing bug-1 fix already applies. No additional CSS or HTML changes were needed.

Verification using the production font families in Chromium:

- Original pre-fix source (781ee3c), 753×1037: all three icon/heading centers differ by approximately 6.7px.
- Current source: all three centers match exactly (0px offset), descriptions remain below their headings, no overflow.
- Also checked widths 740, 752, 754, 760 and 767px, plus the 768/800px tablet layout and 1037/1280px desktop layout. Intentional icon-above-heading tablet layout is unchanged.
- Actual Galaxy Tab S8 device retest remains with QA; desktop Chromium viewport emulation is not an Android-device test.

Use the latest complete HTML containing bug 1’s alignment fix to retest both reports.

[Before](bug-02/before-753.png) · [After](bug-02/after-753.png) · [Baseline](bug-02/baseline.json) · [Checks](bug-02/checks.json)

Fixed navigation overlays are hidden for proof captures only.
