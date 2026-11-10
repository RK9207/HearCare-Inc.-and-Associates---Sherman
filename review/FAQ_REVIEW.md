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
