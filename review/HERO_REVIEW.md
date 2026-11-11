# Hero — approved and locked

Approved in chat: Option A navy split layout; Headline 4, “Personalized Hearing Care, Right Here in Sherman”; recommended test-first supporting copy and everyday-conversation benefit; recommended kitchen-table image concept. The overall creative direction and website-review additions were also approved. This implementation is ready for review, not locked or launched.

## Subsequent header update

The user separately approved the integrated navy header. The current full-page HTML review copy includes this update. See [Header review](HEADER_REVIEW.md) for scope, screenshots, verification and the local logo-fetch limitation. The original Hero-only screenshots and notes below document the preceding Hero rebuild.

## Review the result

- [Desktop Hero](hero-desktop.png), 1440px viewport.
- [Mobile Hero](hero-mobile.png), 390px viewport.
- [Desktop transition into the existing next section](hero-transition-desktop.png).
- [Mobile transition into the existing next section](hero-transition-mobile.png).
- [Downloadable full-page HTML review copy](hero-review.html): download/open in a browser. The Hero now loads from the user-supplied GHL media URL; external fonts, logo, map and form retain their original services. This is a review artifact, not a production deployment.

Screenshots show the Hero without the unchanged header. The fixed mobile Call bar is hidden only during these long-layout screenshots so it does not appear midway through a stitched capture; its source code is unchanged, and hide-on-modal behavior was checked separately. The source image is an AI-generated illustrative scene, not HearCare patients, owners, or a clinic photograph.

## What changed

- Replaced the white first-draft Hero with the approved navy split composition, white/sky headline hierarchy, rounded actions, framed conversation photograph, and restrained overlapping proof panel on desktop.
- Kept a prominent “Hearing tests & hearing aids in Sherman, TX” service line with the selected headline.
- Consolidated the original long support and separate testing paragraph into the approved test-first explanation. Added the approved everyday-conversation benefit; preserved owner-operation and licensed-specialist credibility in concise form.
- Replaced IMG-HERO-01's placeholder with a generated kitchen-table photograph and two efficient responsive WebP assets. Preserved the image ID and added explicit dimensions, responsive sizes and high fetch priority.
- Moved the same review-proof panel into normal reading order before actions on mobile. Preserved 4.8/5, 94 reviews, its existing Google destination and accessible label.
- Preserved Call as primary, Request Appointment as secondary, separate Text action, contact data hooks, address and hours.
- Synchronized PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md and IMAGE_PROMPTS.md, including an approval record and current section tracker.

In the preceding Hero rebuild, no other section, header, form embed, integration script, footer or mobile Call source was changed. The subsequent separately authorized header update is documented above. No sections were removed, merged, added or reordered.

## Focused checks

| Check | Result and evidence |
|---|---|
| Responsive Hero | Checked at 320, 390, 500, 768, 1024, 1440 and 1920px. Hero loaded its image and had no detected horizontal overflow. Desktop/mobile crops were visually inspected. |
| Fonts in screenshots | Original Montserrat/Hind families loaded from a preview-only cache downloaded from the official Google Fonts repository. Production font links remain unchanged. |
| Contact actions | Hero Call and Text destinations checked against +19032062442 at all widths. Actual calls/texts were not placed. |
| Appointment shell | Hero trigger opens the existing dialog; Escape closes it, focus returns to the trigger, and the mobile Call bar is hidden while open. |
| Form delivery | Needs QA. The environment blocks the external form; fields, consent rendering, iframe keyboard behavior and lead delivery were not verified. No lead was submitted. |
| Scope/integrations | Automated comparison confirmed all HTML/CSS outside the Hero block and all integration scripts match the baseline. Existing phone/contact data hooks and form destination remain intact. |
| Accessibility basics | One H1 retained; descriptive image alt, exact accessible aggregate label, native action semantics, visible focus styling and contact targets preserved. Hero reflow also checked with 200% root text sizing; this does not replace assistive-technology QA. |
| Contrast | Measured: white/navy 9.62:1; sky/navy 4.62:1; lead/navy 8.72:1; supporting trust/navy 7.19:1; Ink/sky Call button 6.71:1. These are contrast ratios, not performance or conversion scores. |
| Image weight | Full image about 192KB; 960px version about 136KB. No Hero lazy loading. No Lighthouse/Core Web Vitals or conversion uplift claimed. |
| Evidence | Review aggregate remains screenshot-supported U1, not live-refreshed. Credentials, address and temporary phone retain project sources. No price, free test, availability or guaranteed outcome added. |

## Next gate

Ask the user to approve the rendered Hero, request adjustments, or try another direction. Do not lock it or start a new section automatically. After explicit rendered approval, select the strongest next section, explain the transition, and request that section's desktop/mobile screenshots before its individual review.

## Subsequent hierarchy refinement

User requested removal of the break after Personalized, improved hierarchy and button alignment. The primary phrase now stays together; desktop sizing accommodates the full primary headline when space allows. Local emphasis is subordinate; the existing conversation benefit precedes the detailed test-first explanation. Hero action buttons use matching grid columns and equal height, with consistent icon/label centering in Hero/header controls. Copy, evidence, destinations and integration scripts are preserved. Latest screenshots and portable HTML reflect this refinement. Still awaiting rendered approval.

## Latest headline correction

The user requested one uniform headline color and font size, plus TX after Sherman. The current headline uses the same white, responsive size and weight throughout, reading “Personalized Hearing Care, Right Here in Sherman, TX.” Earlier notes about smaller/lighter location text are superseded. Seven-width Hero checks passed after this correction.

Latest delivery update: the complete HTML now uses the user-supplied GHL Hero image URL directly. Base64 embedding and the former local srcset were removed; layout and interactions are unchanged.

## Visual finish update

User requested a more beautiful Hero. Added tonal navy depth, a restrained service capsule, benefit accent, sculpted photo frame, softer proof/CTA shadows and a compact location panel. All body markup, wording, headline typography, hosted image URL and scripts are byte-identical to the preceding version. Seven-width overflow/contact/dialog checks passed. Local screenshot previews used the existing approved image file as a cache for the supplied GHL URL; live CDN availability was not reverified. Pending user visual approval.

## Restrained/mobile refinement

User approved simplification and requested removal of the mobile break after Care. Headline spans now flow inline on mobile with natural wrapping; all headline colors/sizes/weight and wording are preserved. Removed the service capsule, benefit rule, trust dot and offset outline. Tightened mobile spacing without reducing prose size or removing content. Location panel and genuine review evidence remain. Source image is unchanged, with a slightly adjusted responsive crop. No body markup, links, scripts or other sections changed; awaiting rendered approval.

## Latest: previous design restored

User preferred the previous design. Restored the b132802 visual design exactly, with only a smaller mobile H1 clamp (22px minimum, 7.2vw fluid, 34px maximum; approximately 28px at 390px). Desktop H1 and all body markup, wording, GHL image source, contact links and integrations match that previous design. The simplified treatment is superseded. Awaiting rendered approval.

Latest correction removes only the forced mobile break after Care. The restored styling and smaller mobile H1 remain intact; seven-width overflow/contact checks passed.

Latest user-approved review display: show “90+ Google reviews” in the Hero badge, accessible aggregate label and reviews section. The rating remains 4.8/5. This is conservative display wording based on the recorded 94-review screenshot evidence; preserve the historical source count in RESEARCH.md rather than rewriting that evidence.

Latest badge update matches the supplied compact reference: multicolor Google icon, white 4.8 score, gold stars and 90+ Google reviews on the navy background, below Hero contact actions in both visual and DOM order. The existing review link and accessible label are retained. Screenshot brand names, rating 5.0 and unrelated claims were not copied. Seven-width overflow/contact checks passed.

## Final user approval

The user explicitly approved the current Hero and requested moving on. Hero implementation in commit 6a890ab is APPROVED / LOCKED, superseding earlier pending-review notes. Preserve it unless the user authorizes a specific later change. Next proposed section: existing everyday difficulty, pending its current desktop/mobile screenshots before assessment. No page code changed in this approval record.


## User-authorized refined hero hierarchy

User approved the refined split-hero recommendation with “okay make the changes.” Preserve H1 wording, original size/color/weight and mobile natural wrapping; retain every text statement and image URL. Quiet the eyebrow, reduce competing callout styling, group Google proof with the owner credential beneath aligned CTAs, and simplify address/hours without a tinted panel. Refine photo proportions/crop and corner treatment; preserve both faces. Explicit white-outline default and navy-on-white hover/focus fix the faded appointment button; add matching label wrapper. Desktop padding 52/56px and mobile 30/36px. No other section, header, integration, phone or review value changed. This user-authorized revision reopens only hero presentation; awaiting rendered approval.


Refined hero verification: seven widths (320, 390, 500, 768, 1024, 1440, 1920px), no section overflow, equal CTA widths, dialog open/Escape/focus return. H1 text/color/font rules preserved exactly; no forced mobile Care break. Hover/focus explicitly uses navy text/icon on white and has no color interpolation to avoid transient low contrast. Desktop and mobile crop inspected using the cached actual hero asset; faces remain visible. All subsequent sections, header, scripts and contact destinations unchanged. Current layout requires GHL review before lock.


User requested additional breathing space after the latest desktop screenshot. Increase only hero spacing: section padding, service-label-to-headline gap, benefit/body gaps, CTA spacing, trust divider spacing, credential separation and location-line spacing, with moderated mobile increases. Preserve font sizes, all wording, images, headline wrapping rules, button colors and other sections. Awaiting rendered review.
