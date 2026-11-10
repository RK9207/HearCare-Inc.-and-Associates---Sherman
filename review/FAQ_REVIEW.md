# FAQ section review

User direction: Layout A + headline 1, “Questions before your visit?” Implemented for rendered review, not locked.

## Changes

Desktop places a short introduction beside a wide, bordered seven-question accordion. Mobile stacks the introduction and full-width panels. Open headers have a pale-blue surface and navy chevron; answers have their own padding below a separator. A visible inset keyboard focus ring avoids overlap with the answer and overrides the shared outer shadow locally.

All seven topics remain. The first two now distinguish when to book a hearing test from whether testing implies hearing aids. Answers are shorter while preserving relevant facts: small-style suitability; medical-treatment alternatives; uncertain insurance benefits; model/phone compatibility; pairing guidance; follow-up, maintenance and repairs including devices purchased elsewhere; typical lifespan with proper care; accurate owner credentials and no promise of a named appointment provider. No invented price, duration, credit/coverage guarantee, or outcome claim is introduced.

Native details/summary controls remain independently expandable, initially closed, with no custom accordion JavaScript. Principal answer text stays 18px. No photo or new CTA is needed; shared contact actions and integrations are untouched.

## Checked

- Chromium at 320, 390, 500, 768, 1024, 1440, 1920px.
- Seven questions at every width; no collapsed or expanded horizontal overflow.
- Every item opens with Enter and closes with Space at each viewport (49 item/viewport checks).
- All answer paragraph/list text computes to 18px.
- Exact source comparison: only FAQ markup and FAQ-specific CSS changed. Locked work, header, other sections and integration scripts remain unchanged.
- Complete review HTML matches index.html and whitespace check passes.
- Desktop/mobile collapsed and expanded renderings inspected using cached production font families. Remote image restrictions do not affect this text-only section.
- No calls, texts or form submissions performed; external form delivery not tested.

## Screenshots

- [Desktop](faq-desktop.png)
- [Mobile](faq-mobile.png)
- [Expanded desktop](faq-expanded-desktop.png)
- [Expanded mobile](faq-expanded-mobile.png)
- [Desktop transition](faq-transition-desktop.png)
- [Mobile transition](faq-transition-mobile.png)

Review the GHL rendering before locking. No deployment or merge performed.


## User-requested scroll-following left column

User requested that the FAQ left column slide downward with scroll like parallax. Use native CSS sticky positioning at widths >=768px and viewport heights >=600px, offset below the fixed header by 32px and constrained to the FAQ grid. The intro follows the questions and stops at the section boundary, without custom scroll listeners or moving accordion controls. Keep static positioning on mobile, short viewports and reduced-motion preferences. No wording, typography, other section or integration changes. Awaiting rendered review.


Scroll verification: at 768, 1024, 1440 and 1920px, the intro holds its configured offset while scrolling and remains constrained by its FAQ parent. At 320, 390 and 500px it remains static. Emulated reduced-motion settings restore static position on all checked desktop/tablet widths. Repeated 49 item/viewport keyboard checks and overflow checks passed. The CSS uses no transforms, animations or custom scroll handlers.


## Approved preparation FAQ addition

User requested implementing the source-backed recommendation with “please do it.” Add an eighth FAQ, “How should I prepare for my hearing test?” Answer: note difficult listening situations, be ready to discuss medical history/current medications, and optionally bring a friend or family member. Source S19 in RESEARCH.md is the clinic’s preparation article. Do not imply a required-items checklist or promise a duration/fee. Existing seven answers, styling, sticky introduction, contact integrations and other sections remain unchanged. FAQ remains pending rendered approval.


Preparation follow-up validation: eight questions at all seven widths; all 56 keyboard item/viewport open/close checks passed, no collapsed/expanded overflow, answer text remains 18px, and desktop scroll-follow/boundary/reduced-motion checks still pass. Exact page-source comparison confirms only the eighth details element was added.


## FAQ final approval

User: “Looks good, I approve this section, let's move to next section.” FAQ implementation in b1017ee is APPROVED / LOCKED, including all eight topics, source-backed preparation answer, bordered native disclosures, responsive answer spacing and desktop scroll-following introduction with reduced-motion/static-mobile behavior. Preserve without further user authorization. Next proposed section: the existing Sherman location/map section, to turn answered concerns into practical visit planning before the final contact invitation. Request current desktop/mobile screenshots including map, address, hours and directions, and wait before individual review or editing. No HTML/CSS changes accompany this approval record.
