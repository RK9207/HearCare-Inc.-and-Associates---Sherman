# Everyday difficulty — rebuilt for review, not locked

User approved the asymmetric editorial recommendation and headline 4: **Recognize any of these listening difficulties?**

- [Desktop section](recognition-desktop.png)
- [Mobile section](recognition-mobile.png)
- [Desktop transition from locked Hero](recognition-transition-desktop.png)
- [Mobile transition from locked Hero](recognition-transition-mobile.png)
- [Complete copy-and-paste HTML](hero-review.html), including this rebuild and the unchanged locked Hero/GHL-hosted image.

## What changed

The former three-column layout is now a compact asymmetric composition: headline, short introduction and family acknowledgement on the left; three aligned icon-led examples on the right. Mobile stacks these deliberately. Blue top rules were replaced by quiet dividers and purposeful speech/noise/TV line icons. No stock image, AI image or generic card grid was added.

Preserved the three recognizable experiences and their supporting explanations, family-member relevance, non-diagnostic reassurance, value of noticing otherwise unnoticed changes, and the existing #care visit-explanation link. Consolidated the introduction and closing text; no new price, clinical outcome, availability, promotion or primary CTA was introduced. The section remains immediately after the Hero and before owners/reviews.

## Evidence and checks

The user supplied desktop/mobile screenshots. Before editing, the full current mobile closing area was also rendered and inspected locally, resolving the bottom crop in the user's mobile screenshot. Fonts were cached from the official Google Fonts source for preview; fixed header/Call overlays are hidden only in these section-layout screenshots so they do not obscure content.

Checked at 320, 390, 500, 768, 1024, 1440 and 1920px: no section overflow; three observations and the existing #care destination retained. The link navigated to the target with clearance below the sticky header. Desktop/mobile section and Hero transition were visually inspected. At 390px, section height reduced from approximately 1043px to 978px; at 1440px, from approximately 716px to 612px, without shrinking body text. These are local layout measurements, not conversion/performance claims.

A source comparison verified all HTML/CSS outside this section is identical to the preceding commit, including locked Hero, header, remaining sections, contact data and integration scripts. No lead was submitted, and external form delivery was not tested.

PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md and IMAGE_PROMPTS.md record the approved direction and current implementation. This section remains **awaiting rendered approval**; no further section review or edits are authorized by this implementation. Ask the user to approve, adjust or request an alternative before locking it and selecting the next section.
