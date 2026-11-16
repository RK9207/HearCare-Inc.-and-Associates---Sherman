# QA bug 4: complete map-card office address

Reported November 16, 2026.

Map card now shows:

HearCare, Inc. and Associates  
1800 N. Travis St, Suite D  
Sherman, TX 75092

Added the missing Suite D, restored the period in N., and removed the stray comma before the line break. The review-source address also now uses the same full format. Hero, main location details and footer already contained the correct suite.

Verified at 320, 393, 753 and 1440px: full address including suite is rendered, canonical practice name retained and no horizontal overflow. Exact comparisons preserve all links, scripts, map coordinates/settings and verbatim testimonials. Existing fixes for bugs 1, 2 and 3 are included.

[Checks](bug-04/checks.json) · [Map-card proof](bug-04/map-card-393.png)
