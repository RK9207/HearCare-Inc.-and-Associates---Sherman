# Design system — HearCare, Sherman

Direction approved November 10, 2026: warm editorial healthcare; everyday connection first, authentic owners early, clear testing pathway. This specification implements the approved strategy; it is not a claim that these dimensions or components were extracted from the existing website. Read PAGE_STRATEGY.md and CONTENT_DIRECTION.md before implementation.

## Approved Step 5 Hero pattern — November 10, 2026

User-selected Option A controls the Hero only. Implemented for rendered review; not locked. Preserve other section styling and mobile Call until independently approved. The header was subsequently independently approved as recorded below.

- Full-width navy/deep-navy Hero surface, with white primary copy, sky-blue headline emphasis and a substantial adjacent lifestyle photograph. A restrained offset outline frames the photograph; no background photograph behind text.
- Use the user-selected personalized/local H1 with the prominent service/location line and concise test-first explanation from CONTENT_DIRECTION.md.
- Desktop: approximately 51% content / 49% media within the existing container, a generous gap, and a white Google-proof panel overlapping the lower-left image boundary. Keep both subjects' faces inside the crop.
- Below 1,024px: one column with message, the same proof panel in normal flow, actions, address/hours, then photograph. No duplicated proof DOM. Photo is 4:3 on mobile/tablet; no fixed Hero height.
- Hero controls use the approved rounded/pill brand treatment, at least 48px high, with sky/Ink Call and a white-outline appointment action. This local pattern does not silently restyle controls elsewhere.
- Scope Hero-specific color, type, focus and responsive rules to its classes. Ensure the white proof panel's stars, values and keyboard focus remain legible on the dark surface.
- IMG-HERO-01 is a 4:5 generated source delivered as 1,122px and 960px WebP files, with explicit dimensions, responsive sizes, high fetch priority, no lazy loading, and a meaningful illustrative alt. Crop with CSS; never stretch faces.
- The generated scene is not a HearCare clinic, patient or outcome claim. Google aggregate evidence remains U1/RESEARCH §3A, separate from the illustrative image.

These approved details supersede older Hero guidance below, including the original white-first treatment and Hero button radius. They do not authorize applying the pattern to unreviewed sections.

## First-screen priorities

The visitor must identify hearing tests, hearing aids, Sherman, an understandable benefit, and contact actions without opening navigation or an accordion. Use one H1, a short supporting statement, compact practice/location details, and a clear CTA group. Do not let decorative imagery or a tall header push the service and first CTA below a typical mobile first screen. Let the hero image follow text/actions on mobile rather than shrinking everything to fit a fixed viewport.

Tone: professional, warm, respectful, and locally grounded. Avoid luxury-spa styling, dense medical dashboards, giant product catalogs, or a page composed entirely of cards.

## Color and functional usage

| Token | Value | Role |
|---|---|---|
| Brand sky | #78bbe9 | Main Call button, mobile sticky Call action, selective accents |
| Deep navy-teal | #004a69 | Major headings, footer/final CTA backgrounds, high-contrast surfaces |
| Mid blue | #2578b2 | Links and selected supporting emphasis; underline text links |
| White | #ffffff | Main canvas and text on verified dark surfaces |
| Ink | #2c2c2c | Body text and text/icons on sky-blue buttons |
| Light surface | #f2f8fc | Proposed low-intensity section tint; derived supporting neutral, not a supplied brand color |
| Border | #d5e2ea | Proposed decorative dividers; not sufficient alone for functional control boundaries |

Primary sky buttons use Ink, not white. Navy backgrounds use white body text with sky accents. Avoid mid-blue small text on sky/tinted backgrounds unless measured contrast passes. Target WCAG AA: 4.5:1 normal text, 3:1 large text and necessary UI graphics. Use a clearly visible control border where required; decorative borders need not act as the only boundary of an input. Validate actual combinations and hover/focus states during implementation.

## Typography

- Heading font: Montserrat, weights 600–700. Body/UI: Hind, weights 400–600. Fallbacks: Arial, sans-serif. Do not introduce a competing display face.
- Desktop H1: fluid 40–56px, line height 1.08–1.16; mobile 32–38px. Keep service and location readable with intentional wrapping, never nonbreaking text that causes overflow.
- H2: 30–38px desktop, 26–30px mobile, line height about 1.2. H3: 21–24px, line height about 1.3.
- Body: 18px minimum for main prose, line height 1.55–1.65. Supporting details may use 16px; avoid tiny credentials, legal text, or action labels.
- Buttons: 17–18px, medium/semibold. Eyebrows, if needed: 14–16px, restrained letter spacing; no full paragraphs in capitals.
- Prose width: approximately 55–70 characters; hero support narrower. Keep headings concise and descriptive. Use weight/spacing before adding more colors.
- Load only needed weights with font-display swap. Use approved official font sources or locally supplied licensed files; keep usable system fallbacks if fonts fail.

## Widths, grids, spacing, and breakpoints

- Main container: maximum 1,200px, centered; page gutters 20px mobile, 32px tablet, 40–48px desktop.
- Prose column: maximum roughly 680px. Hero text: around 560px. Do not stretch payment or FAQ answers across the full container.
- Desktop hero: approximately 55% text / 45% image with a generous gap. Owner group: portrait beside editorial text, with reviews below as a distinct subsection.
- Grid: flexible 12-column desktop arrangement when useful, two-column tablet, one-column mobile. Grid is a layout aid, not a reason to turn content into twelve cards.
- Spacing scale: 4, 8, 12, 16, 24, 32, 48, 64, 80, 96px. Section padding typically 72–96px desktop and 44–64px mobile. Compact recognition passage uses less; proof and final invitation receive more breathing room.
- Working breakpoints: 640px and 1,024px. Below 1,024px, simplify the header if full navigation and actions collide; below 640px, single-column sections. Treat these as starting points; test actual content and zoom rather than relying only on device labels.
- No fixed section heights. Allow text enlargement, font fallback, long names, and review content to reflow.

## Components and behavior

### Header and navigation

Step 5 header direction explicitly approved in chat: integrated navy (#004a69) sticky header with the original supplied wordmark blending into its brand surface, white navigation, sky/Ink Call pill and white-outline Request Appointment pill. Preserve logo identity and original links. Align to the same 1,200px content container as the Hero; use a restrained sky-tinted bottom separator rather than a disconnected white band. Keep Care, Our Practice, FAQs and Location anchors; add subtle hover/focus underlines.

Working heights: 88px wide desktop, 80px below 1,200px, 76px below 640px, allowing content to grow where needed. Update the shared header-height offset for sticky anchors and existing sticky-content positioning. Hide full navigation below 1,200px before it crowds the logo/actions; hide header Call below 900px, preserving Hero Call and the existing mobile Call action. Below 640px, preserve full Request Appointment wording with natural two-line wrapping on the narrowest screens. Keep targets at least 44px; do not clip the logo or alter its colors. Header changes are implemented for rendered review, not locked.

Mobile: logo plus Request Appointment; do not squeeze desktop navigation into the row. Include a skip link and semantic navigation. Use the supplied logo linked to https://hearcareinc.com/. Verify its color variant and resolution before choosing the surface. Do not recolor or distort it arbitrarily; use the documented white variant only on a suitable dark surface.

### CTA hierarchy and contact data

Primary conversion is Call. Use a filled sky button with Ink text and phone icon; secondary Request Appointment uses a clear outline/navy treatment on light surfaces. Text is a distinct labelled action, not a hidden behavior of the phone button. On dark surfaces, maintain a readable outline or white secondary action.

Temporary user-approved contact: **903-206-2442**; Call → `tel:+19032062442`; Text → `sms:+19032062442`. Centralize the contact data in the eventual implementation so CSM tracking numbers can replace display and links consistently. Do not assume future call and SMS tracking destinations will be identical; verify both when supplied.

Controls: minimum 44×44px targets, preferably 48px high for major actions, 8px radius, 16–24px horizontal padding. Provide visible hover, active, and focus-visible states. Use a two-tone focus treatment where necessary against both navy and white surfaces. Icons supplement text. Avoid pulsing, bouncing, or urgency animations.

Place CTA groups in the hero, after trust, after the process, and in the final invitation. Payment has a contextual Call/Text prompt. Header and mobile sticky action stay available; do not add a large repeated button row after every paragraph.

### Hero

Follow the approved Step 5 Hero pattern above: navy split composition, generated kitchen-table scene, explicit service line and personalized/local H1. Desktop proof overlaps the photo; mobile proof precedes actions and imagery. Aggregate values are screenshot-supported 4.8/5 and 94 reviews (RESEARCH §3A/U1), not a fresh lookup. Use a fractional star fill and exact accessible aggregate label. Owner-operated/licensed microcopy supplies additional factual trust.

Show Sherman address and hours compactly near the first contact opportunity. Do not crowd the hero with eight brand logos, long credentials, symptoms, or financial disclaimers.

### Portrait and proof

Use the documented real joint owner portrait; retain both people in the crop. Pair with names and exact professional titles. Portrait should remain an identity image, not a huge background: the identified source is only 411×411px. Obtain a larger original if the intended display needs it.

Reviews have a dedicated heading within the early proof group. Display verified Google rating/count and up to six reviews desktop, three mobile, with Read all our Google reviews linking to the brief's exact destination. Recommend three strong authentic reviews for the initial layout; six is a cap, not a quota. If only three are supplied, show three at all sizes. If using six, retain the three most useful on mobile and keep the external all-reviews link accessible; avoid an autoplay carousel.

Use quotes as text when faithfully transcribed from supplied material, with clear attribution; preserve screenshots as appropriate. Allow expanded reading for long excerpts without changing meaning. Do not manufacture a Google UI, badge, reviewer photo, or star count. Pending reviews must be labelled in internal draft notes, never rendered as fake public proof.

### Process and benefit explanations

Four numbered stages in a connected editorial sequence; short text with subtle rules or icons. On desktop use columns only if each remains readable; on mobile use a vertical sequence. Clarify that recommendations and device fitting depend on suitability. No clinically decorative waveform, unexplained audiogram, or equipment illustration pretending to document the practice.

Options section uses one purposeful product visual and two or three benefit explanations. Brands are a compact text list or approved logos, not oversized trust badges. No repetitive image/text alternation simply to fill the page.

### Cards, borders, radius, and icons

Use cards selectively for genuine review units or a financial-help callout. Prefer flat editorial layouts elsewhere. Component radii: 8px controls, 12px review/callout surfaces, up to 16px photographic frames. Preserve logo/product proportions. Shadows are subtle and optional; borders and whitespace do most grouping.

Choose one simple icon family and consistent stroke weight. Use phone, message, direction, and process icons only where they clarify function or sequence. Label interactive icons; hide purely decorative SVGs from assistive technology.

### FAQ

Single-column accordion with visible questions and a clear expand affordance. Use native details/summary or equivalent button controls with correct expanded state and relationships. Keyboard operation must work. Allow more than one answer open. No answers essential to service/location recognition should be hidden here. Full-width click targets, clear focus, comfortable text size, and quiet dividers; no photos.

### Appointment popup / GHL form

- All Request Appointment buttons open the same supplied form, not competing inline and popup variants.
- Source: https://api.onspirepulse.com/widget/form/8wW1RhQrj7egDZ93IJlJ; script: https://api.onspirepulse.com/js/form_embed.js; form ID `8wW1RhQrj7egDZ93IJlJ`; original supplied iframe ID `popup-8wW1RhQrj7egDZ93IJlJ`; provider-declared height 647px, radius 8px. The original brief is the authoritative full embed, including consent attributes.
- Preserve destination, field behavior, consent attributes, and provider semantics. Assess the supplied POPUP/alwaysShow behavior before altering it. Use supported provider click-trigger behavior where available; make only technically necessary integration changes and explain them. Do not nest a provider popup inside another modal unnecessarily or disable consent to make the form render.
- No page-load auto-open. User click initiates the popup. Keep the supplied iframe hidden until activated using the chosen supported integration.
- Suggested modal maximum width 640–720px; viewport margins 16–24px; maximum height around 90dvh with internal scroll and visible close control. Adapt to keyboard and embedded content height; never crop the submit action behind fixed overlays.
- Heading Request an Appointment; brief text distinguishing request from confirmation. Do not promise response time. Include phone fallback for rendering/network failure.
- Accessible dialog name, initial focus in the dialog shell, trapped focus while open, Escape and close control, background inertness, body-scroll management, and focus return to the triggering button. If provider-managed, verify equivalent behavior rather than assuming it.
- Cross-origin iframe content cannot be restyled arbitrarily; do not promise host-level control of its fields or read its clinical content. Observe supported readiness/success signals, not simulated success states.
- Verify display, scrolling, close/reopen, and keyboard behavior without sending a real enquiry. Any actual submission requires separate authorization.

### Map, location, footer

Use the brief's exact Google map embed for the Sherman place, with a meaningful iframe title and responsive width. Suggested map height: 360px desktop, 280px mobile; lazy-load below the fold. Keep address/hours readable independently of the iframe. Place Get Directions with direction icon below the map and use the documented Sherman directions destination, not a generic search.

Location: 1800 N. Travis St, Suite D, Sherman, TX 75092. Hours: Monday–Thursday 9am–5pm; Friday by appointment only. No parking/accessibility claims without evidence.

Final invitation follows practical location details in a deep navy band, with sky Call button and a legible Request Appointment alternative. Footer stays quieter and includes Privacy Policy, Visit Our Website, local details, and copyright per CONTENT_DIRECTION.md. No second practice's number or address to dilute Sherman relevance.

### Mobile sticky Call action

Bottom Call button with phone icon, sky #78bbe9 background, Ink #2c2c2c text, `tel:+19032062442`. Account for `env(safe-area-inset-bottom)` and reserve enough page-bottom padding so footer links and content remain accessible. Layer below the modal; hide or deactivate it while the dialog is open. Prevent collisions with cookie/consent controls and the software keyboard. Mobile header retains Request Appointment; no competing sticky bars.

## Visual storytelling system

| Section | Visual job / image role | Rhythm and density |
|---|---|---|
| Hero | Lifestyle conversation shows why care matters; text gives service/location; trust badge only with evidence | First visual peak; one dominant image, concise message |
| Everyday difficulty | No image; short observations connect the promise to recognizable life | Brief, quiet transition; compact text |
| Owners and reviews | Real portrait establishes identity; authentic reviews add patient evidence | Second visual anchor; generous spacing, portrait then distinct proof subsection |
| What happens next | Numbered sequence explains the service; no decorative equipment scene | Calm informational stretch; moderate density, clear progression |
| Options | Authorized product image explains choice; benefit copy connects it to daily use | Selective detail and asymmetry; avoid catalog density |
| Payment | No image; financial-help message supplies reassurance | Quiet text-led relief on light tint or white |
| FAQ | No image; clear questions encourage private exploration | Compact progressive disclosure, easy scanning |
| Location and final invitation | Map establishes locality; strong CTA surface signals action | Practical details, then final contrast peak |
| Popup/footer | No image; clear request and policy access | Focused action, then a quiet ending |

Use whitespace, a subtle divider, or a change in composition for transitions before reaching for a new background color. White is the default canvas; light tint gives selected informational relief; deep navy anchors the approved Hero and final invitation/footer rather than every other section. Headings should carry a coherent story even if images do not load.

On mobile preserve the same persuasion order: service/action first, short recognition, real owners/proof, process, options, payment, FAQ, local action. Do not move all authentic proof beneath long explanations. Stack review and process units legibly, reduce decorative spacing before reducing font size, and preserve complete faces and product shapes in alternate crops.

## Image sourcing and treatment

- Real owners: documented image URL in RESEARCH.md section 9. Verify resolution, ownership/approved use, and actual appearance before implementation. Do not upscale aggressively or portray them as different people through generation.
- Clinic/GBP images: not supplied. Use only verified actual practice/location imagery once available; a future exterior photo belongs near location, a genuine testing image may support the process. Do not imply that stock or generated interiors document the Sherman clinic.
- Lifestyle: one warm, bright, credible adult conversation scene in the hero. Portray agency and engagement rather than frailty or isolation. An approved image may be stock, but do not imply the people are patients or that the scene demonstrates an outcome. Existing website availability alone does not establish a reusable stock license.
- AI imagery: not required. If used later with approval/appropriate rights, restrict it to clearly illustrative lifestyle context; no fabricated owners, patients, testimonials, equipment evidence, clinic exteriors, or clinical before/after proof. An AI image is never a source for a factual claim.
- Product: authorized actual model imagery, supplied manufacturer/source names kept accurate. No manufacturer banner with embedded competing text or contact details. Do not invent specific models/features from a generated device image.
- Logo: supplied filesafe.space PNG; documented white site variant for a dark footer where appropriate. Verify URLs and variants; do not assume staging paths work.
- Crops: hero about 4:3 or 5:4 desktop, responsive crop on mobile retaining the conversation; portrait 1:1; product image contained with whitespace. Existing 2560×400 hero banners and 300px thumbnails are not automatic substitutes for a tall high-resolution hero.
- Use image elements with meaningful alt text for informative assets, empty alt for decorative imagery, explicit dimensions to limit layout shift, responsive sizes, and efficient formats. Prioritize the hero; lazy-load below-fold assets. Do not embed essential words in images.

## Accessibility, motion, and validation

Use semantic landmarks, one H1, logical headings, visible keyboard focus, descriptive links, and labelled controls. Test 200% text zoom, narrow 320px layout, and representative 375/390px, 768px, 1,024px, and 1,440px viewports. Verify no horizontal scroll or inaccessible fixed overlays. Respect reduced-motion; any transitions should be brief and nonessential. No scroll hijacking, parallax, mandatory entrance animations, or autoplay media.

During Step 4/5, inspect actual rendering rather than relying on code or open ports. Verify contact links against the temporary number; confirm all appointment triggers, iframe behavior, Escape/focus return, FAQ keyboard access, real image resolution, Google/map links, contrast, and missing asset treatment. Do not interpret rendering as successful lead delivery or improved conversion performance. Public completion depends on verified review material, asset suitability, integration checks, and explicit publication authorization.

## Approved hierarchy and button refinement

The user requested improved visual hierarchy, removal of the break after “Personalized,” and button alignment fixes. Keep “Personalized Hearing” together, allow the remaining headline to wrap responsively, and make the local phrase smaller/lighter than the primary message. Place the existing conversation benefit before the longer test-first explanation, preserving all approved wording. Use equal-width/equal-height Hero action columns on desktop, a single column on mobile, and consistent centered icon/label groups in Hero/header buttons. These refinements remain pending rendered approval; no section is locked. Preserve all destinations and integration hooks.

## Subsequent headline correction

User requested uniform color and font size throughout the entire headline and TX after Sherman. The current H1 is “Personalized Hearing Care, Right Here in Sherman, TX.” Both lines inherit the same white color, responsive font size and weight; the earlier smaller/lighter location treatment is superseded. Keep Sherman and TX together when wrapping. Other layout, copy and actions remain unchanged. Pending rendered approval.

## Hero visual refinement

The user clarified that the current Hero should be made more beautiful. Apply visual styling only: restrained navy tonal depth, a fine-bordered service capsule, an accent rule beside the existing benefit, a larger sculpted photo corner with subtle offset frame/shadow, gentle CTA depth, and a contained translucent location/hours panel. Preserve every word, heading color/font size/weight, GHL-hosted image URL, proof placement, links and integration scripts. Mobile simplifies these treatments without additional imagery. Pending rendered approval; no other section is changed or locked.

## Approved restrained refinement

User authorized simplification and specifically requested no forced mobile break after “Care,”. On mobile, headline spans are inline with natural wrapping; headline wording, uniform white color, weight and responsive size remain unchanged. Remove the service capsule, benefit rule, trust dot and offset photo outline; retain the useful location panel and review proof. Tighten mobile spacing without reducing body text size or deleting content. Use a softer photo frame and centered mobile crop at 50% / 55%. Pending rendered approval; no section is locked.

## User-requested return to previous visual design

The user preferred the prior design and requested its restoration, plus a smaller mobile headline. Restore the visual implementation from b132802 (service capsule, benefit rule, trust dot, framed photograph and location panel). Supersede the subsequent restrained-refinement direction. Preserve the original uniform white headline, wording including Sherman, TX, hosted GHL image and all actions. Only mobile headline sizing differs from that prior design: clamp(1.375rem, 7.2vw, 2.125rem), approximately 28px at 390px versus the prior 32px. Desktop sizing remains unchanged. Still awaiting rendered approval.

Latest user correction: remove the forced mobile break after “Care,” by rendering H1 segments inline below 640px. Preserve the restored visual design, smaller mobile font size, desktop headline, all wording and integrations. Natural line wrapping remains responsive.

## Compact Google proof approved by reference

User requested the supplied screenshot badge style: inline Google icon, white 4.8 rating, gold fractional stars, and 90+ Google reviews, placed below Hero contact actions on desktop/mobile. Remove the floating white badge card, preserving the existing Google destination, accessible aggregate label and screenshot provenance. No other business details from the reference are adopted. Prior photo-overlay/proof-before-actions guidance is superseded. Pending rendered approval.

## Approved everyday-difficulty rebuild — implementation for review

The user approved the asymmetric editorial recommendation with headline 4: “Recognize any of these listening difficulties?” Current placement remains immediately after the locked Hero and before owners/patient proof. Visitor question: “Do these everyday experiences sound familiar?” The left column contains the chosen headline, brief introduction and family acknowledgement; the right column contains three purposeful icon-led rows (missing words, conversations in noise, TV volume). A full-width, restrained reassurance band states that these experiences do not automatically establish hearing loss or hearing-aid need, preserves the value of identifying unnoticed changes, and keeps the #care visit-explanation link. It is not a diagnostic checklist or a new primary conversion.

Mobile stacks introduction/family context, observations, then reassurance/link. Retain comfortable prose size and simplify spacing; no photo, AI generation, separate sales CTA, generic card grid, or section reorder. The remaining mobile closing area was inspected in an actual local current-state rendering before edits, using the code and the user's screenshots together. Hero/header markup, Hero styling, contact configuration and integration scripts remain unchanged. This section is implemented for rendered review, NOT LOCKED; final approval is still required. Owners/reviews and other remaining sections have not been individually assessed or changed.

## Space-utilization refinement requested by user

The user requested better use of the available section width. Supersede the asymmetric split with a full-width heading/introduction and one continuous white surface containing three aligned editorial columns on desktop. This is a shared panel with separators, not separate repeated cards. Consolidate family acknowledgement, diagnostic reassurance and visit link in the compact closing area. On mobile, stack the icon-led examples within the shared panel, followed by closing context. Preserve all section wording, existing service link, locked Hero, header and integrations; no section reorder or removal. Implementation remains pending rendered approval.

Latest user correction: normalize the section’s closing family acknowledgement, reassurance and visit link to 18px (1.125rem), matching the main body copy. Preserve wording, emphasis and layout; supersede the smaller 16/17px closing sizes. No Hero change.

## Approved owners and Google proof rebuild — Layout A

User selected “Layout A + Headline 1 on both as recommended.” Retain **Meet the people behind HearCare** and **What patients say on Google**. Owner introduction now precedes the portrait on all viewports. Preserve the real joint portrait at a modest 300px desktop / 280px mobile display, shared visible exact licensed status, both full names and Jill's B.S. Each owner has a native keyboard-operable View qualifications disclosure retaining the complete original education/licensing/coursework facts. This consolidates repetition without concealing the essential licensed credential or implying audiologist/doctor status, years of experience, appointment staffing or guaranteed outcomes.

Use a distinct softly tinted reviews area with Google icon, screenshot-supported 4.8 aggregate and user-approved 90+ display, gold fractional stars, and three full verbatim reviews: Karyn Feltner, garey gaston and Sandra Walker. The other transcriptions remain preserved in RESEARCH.md. The dedicated Google heading, all-reviews link, listing qualifier and individual-experience disclaimer remain. This approved selection supersedes the prior six-card desktop implementation. Closing contact invitation puts Call first and Request Appointment second, preserving existing destinations/data hooks and form integration.

Current section is implemented for rendered review, NOT LOCKED. The locked Hero and recognition section, header and all other sections are unchanged. Owner image URL is unchanged; the environment could not load that external image, so final actual-photo appearance must be reviewed in GHL. No new stock/AI image or generated provider likeness is authorized or used. No page-order change or new section is introduced.

## User-requested mobile optimization

Optimize the current owners/reviews group below 640px only. Use a compact authentic portrait beside visible licensing context from 380–639px, then full-width owner disclosures and values; below 380px, stack a smaller 160px portrait and full-width credentials. Hide only the duplicate photo caption on mobile, retaining both full names and authentic image alt. Reduce spacing, retain 18px principal prose/full quotations, use comfortable disclosure targets and full-width aligned contact actions. Desktop layout, all page markup/wording/quotes/links and both locked sections are unchanged. Real GHL portrait fetch remains blocked locally and is not substituted with another image. Final GHL photo/rendering review remains required; section is not locked.

## Mobile portrait layout correction

The user rejected the compact portrait-and-licensing row shown in the GHL screenshot. Replace it below 640px with a centered 220px authentic portrait (200px below 380px), followed by full-width licensing text and vertically stacked owner profiles. Use full-width outlined native qualification controls with a clear right-aligned chevron and at least 48px height. Preserve all wording, review quotations, source image, desktop styling and locked sections. This supersedes the prior side-by-side mobile optimization. Awaiting rendered approval.

User-requested mobile centering: center the owner heading/introduction, shared license, names, qualification controls and values below 640px. Portrait remains centered. Keep expanded qualification prose and review quotations readable; main review content remains left-aligned. Desktop and locked sections unchanged.

## Approved process rebuild — Layout A, headline 4

User selected “Layout A with headline 4.” Current process H2: **Know what to expect before your visit**. Replace the connected four-column timeline with two editorial phases: **At your hearing test** (test and explained results) and **If hearing aids are appropriate** (suitable options and fitting/education/support if the visitor proceeds). Retain four numbered stages but no connector suggesting automatic device purchase or same-visit fitting. Integrate practical benefits into the descriptions rather than repeating outcome bars. Keep the quiet/confidential setting, tones/speech, recorded responses, audiogram explanation, needs/lifestyle/budget fit, custom impressions when needed, device-care/conditional charging/connectivity instruction, and follow-up adjustments.

Keep the source-backed point that some hearing-loss causes may need medical treatment. Preserve the full original test-type disclosure and its not-every-visit qualification; make its expanded text readable and keyboard accessible. A compact navy contact band keeps Call primary, Request Appointment secondary and a separate Text action, with existing values, hooks and destinations. Main prose/disclosure copy is 18px; mobile descriptions use full width under each numbered heading. White section canvas provides a quieter transition after the preceding tinted Google-proof area. No photograph or new image slot is added.

The supplied desktop/mobile screenshots and current code were assessed before edits. Current section is implemented for review, NOT LOCKED. All three approved sections, header, other sections, shared disclosure styles and integration scripts remain byte-identical outside the process scope. No page-order change, unsupported medical/pricing/availability claim or new promotion. IMAGE_PROMPTS.md remains unchanged because no image role or asset was changed.


## Process visual refinement after GHL screenshot

User requested a better design of the current unlocked process section. Preserve Layout A, headline 4 and all copy/integrations. Strengthen phase hierarchy with a navy first-phase header and pale-blue conditional header, white equal-height panels, outlined step numbers and internal dividers. Use a restrained heading accent and a medical-note rule. Replace the heavy navy contact block with a lighter surface and align Call, Appointment and Text on one desktop row; stack at mobile widths. Keep 18px body text and full-width mobile descriptions. All previously locked sections remain unchanged. Pending rendered approval.


## Options rebuild — Layout A, headline 1

User approved Layout A and “Hearing aids chosen around your life.” Use an image-led introduction with heading/copy left and product visual right; three balanced benefits below cover appropriate discreet styles, personalized fit/settings, and compatible phone features. A compact eight-manufacturer list and original expandable style guide finish the section. Mobile reading order: headline, introduction, image, full-width stacked benefits, brands and style guide. Main text and qualifications remain 18px. A tinted canvas changes rhythm after the white process section; no extra large CTA is needed. Preserve suitability/compatibility qualifications and avoid promises of universal invisibility or outcomes. All other sections are unchanged. Process approval has not been explicitly recorded; preserve its latest implementation. Options implemented for review, not locked.

Imagery: authentic in-hand photo remains preferred but is not available. Use the research-recorded clinic-hosted Widex SmartRIC image at its native 232×253 dimensions as a labelled model example, not as a universal device or feature promise. Local network fetch is blocked, so actual image loading/appearance needs GHL review. No generated device or stock source with unverified licensing is used.


## Options revision after updated GHL screenshots

User requested stronger design and content. Keep the approved headline and conditional hearing-aid premise. Replace the low-contrast image-led opening with a compact navy introduction, white headline, and a modest labelled product frame sized to the existing asset. White canvas and three editorial benefit columns focus on appearance, comfort and connection; mobile stacks them with simple dividers. Shorten repeated prose and integrate compatibility/suitability qualifications. Keep the original style guide and all eight brands, now shown as plain text in a supporting strip rather than button-like chips. Main prose stays 18px. No CTA, other section or integration changes. Existing product URL remains; its actual appearance is supported by the user’s new GHL screenshots, while remote retrieval is blocked locally. No generated product imagery. Awaiting rendered review, not locked.


## User-requested border refinement

Use one consistent #b8cfdd border treatment for the product frame, shared three-benefit enclosure, manufacturer panel and style disclosure. Desktop benefit columns have matching internal vertical dividers; mobile stacks within the same rounded enclosure with horizontal separators and no stray left borders or double edges. Open style guide gains a clear separator below its summary and padded body. Navy intro has a subtle tonal outline. Copy, typography, other sections and integrations remain unchanged. Awaiting rendered review.


User requested restoring pill-shaped circular borders around all eight manufacturer names. Restore white-filled rounded outlines with consistent 8px gaps, preserving the existing panel, text sizes and section layout.


User requested a more noticeable hearing-aid style disclosure. Rename the summary “Compare hearing aid styles,” add explanatory copy and an explicit expand instruction, use a pale-blue surface with a stronger 2px outline and a navy circular chevron. Retain native keyboard-accessible details, all expanded style content, responsive layout and existing type sizes elsewhere. No other section or integration changes.


## Options final approval

User: “Looks good, i approve this and lets move to next section.” Hearing-aid options in b2d329e is APPROVED / LOCKED, including navy introduction, labelled authentic product image, bordered benefits, pill manufacturer names and prominent style-guide disclosure. Do not modify without user authorization. Next proposed section is payment and insurance help: it follows suitable device choices by addressing cost, benefits and payment questions. Request its current desktop/mobile screenshots and wait before individual review or editing. This approval records options only; no inferred final approval or lock of the preceding process section is added.
