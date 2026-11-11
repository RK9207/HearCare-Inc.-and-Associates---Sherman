> Current implementation and approval summary: [CURRENT_STATE.md](CURRENT_STATE.md). Earlier proposals and chronological notes below remain historical; later explicit user decisions take precedence.

# IMAGE_PROMPTS.md — HearCare, Inc. and Associates (Sherman, TX)

**Step:** 4B, image prompt reference for Step 5
**Prepared:** November 10, 2026
**Page:** Hearing Tests & Hearing Aids in Sherman, TX (`index.html`, Step 4A first draft)
**Read with:** PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, RESEARCH.md

---

## Scope

The Step 4A draft began with three image slots. Step 5 has replaced IMG-HERO-01 with a generated lifestyle image; the provider image and product placeholder retain their existing state. This file covers only those three slots. No other section has a placeholder, and none should receive an image just to fill space. The design system keeps the difficulty, process, payment, FAQ, review, location and final sections image-free.

| Asset | Current implementation | Next improvement |
|---|---|---|
| Hero | Approved, user-hosted AI lifestyle illustration | Preserve; not practice evidence |
| Owners | Authentic user-hosted joint portrait | Obtain higher-resolution original |
| Product | Clinic-hosted Widex SmartRIC, 232×253, labelled example | Obtain authorized high-resolution real product/in-hand photo |
| Footer logo | Removed at user request | None required |

**If Step 5 changes a section's layout, crop or visual purpose, update that entry here rather than leaving it stale.**

---

## Rules that apply to every prompt

These come from the Step 3 documents and RESEARCH.md. They override any wording in an individual prompt.

- **No fabricated practice evidence.** An AI image must never be presented as the HearCare office, the Sherman location, its staff, or Kenneth or Jill Sheppard. AI imagery is acceptable only as generic lifestyle or product illustration.
- **No AI likeness of the owners.** Never generate or "re-imagine" Kenneth or Jill. The only allowed AI use on their portrait is faithful restoration or upscaling of the real photo (IMG-PROVIDER-01, Option 1).
- **Outcome imagery stays modest.** Show ordinary, engaged conversation. Do not show euphoric "miracle" reactions, before/after drama, or anything implying guaranteed results.
- **No fear imagery.** No isolation, distress, dementia cues, hospital beds or falls.
- **No unsupported product claims.** Do not show charging cases or docks, because rechargeable models are unconfirmed. Do not show hearing aids near water, because most are not waterproof. Do not imply that every device is invisible.
- **No text, logos or brand marks** on devices, clothing, mugs, signage or screens. The page names eight manufacturers and must not visually favour one.
- **No audiometer close-ups, waveforms, audiograms on screens, or clinical equipment** presented as the practice's own.
- **Audience realism.** The primary subjects are adults roughly 60–80, with family members roughly 30–55 where relevant. Use a mix of ethnicities across the page, appropriate to North Texas. Real skin texture, grey or silver hair, reading glasses where natural, everyday clothing.
- **Palette harmony with DESIGN_SYSTEM.md.** The page uses sky blue (#78bbe9), deep navy-teal (#004a69), white and ink (#2c2c2c). Favour soft daylight, warm neutrals and muted blues in wardrobe and setting. Avoid saturated reds, oranges or neon.

**Universal negative prompt** (append to every generation where the tool supports it):
`text, words, letters, logos, brand names, watermark, signage, phone screen content, hospital bed, IV, stethoscope, lab equipment, audiometer screen, waveform graphics, exaggerated smile, open-mouth laughing at camera, posing at camera, thumbs up, perfect plastic skin, airbrushed, uncanny eyes, extra fingers, distorted hands, distorted ears, malformed hearing aid, oversized hearing aid, earbuds, headphones, charging case, glossy stock-photo lighting, HDR, oversaturated colors`

---

## IMG-HERO-01 — Hero

### Approved purpose and implementation — November 10, 2026

The user selected Option A (navy split layout), Headline 4 (“Personalized Hearing Care, Right Here in Sherman”), recommended test-first support/benefit copy, and the recommended kitchen-table concept. This image supplies everyday human relevance beside the explicit service line “Hearing tests & hearing aids in Sherman, TX.” Hero implementation is awaiting rendered approval; it is not locked.

**Source:** AI-generated generic editorial lifestyle illustration created for this approved Hero. It is not an actual HearCare patient, provider, office, or documented treatment outcome. No visible hearing device is shown, avoiding any implied specific product feature or unsupported device geometry.

**Assets:** `assets/hearcare-kitchen-conversation.webp` (1122×1402) and `assets/hearcare-kitchen-conversation-960.webp` (960×1200), both portrait approximately 4:5 sources. Original generated PNG remains outside the repository. The original portrait-placeholder instructions are superseded.

### Composition and crop

- Two women, an older adult and an adult family member, engaged in an ordinary kitchen-table conversation. Silver hair, muted blue/off-white wardrobe, warm daylight and a calm domestic background; nobody posed toward camera.
- Desktop: photograph occupies the right side of the split composition. CSS cover crop is centered near 51% horizontal / 46% vertical; preserve both faces when height changes. The restrained white review panel overlaps the lower-left photo/table area without obscuring faces.
- Tablet/mobile: 4:3 display crop, centered near 50% / 46%. The proof panel moves into normal flow before the contact actions, so it cannot obscure mobile subjects.
- Rounded upper-left corner and a subtle offset outline belong to the page styling, not baked into the image. No words, logos, badges, frames or ratings are embedded in the image.
- The image follows message, proof, actions and location details in mobile reading order. `data-img-id="IMG-HERO-01"` is preserved; explicit width/height, srcset/sizes, decoding async and high fetch priority are supplied. Do not lazy-load this image.
- Alt: “An older woman and an adult woman talking together at a kitchen table.” Do not identify them as patients or claim an improved hearing outcome.

### Generation direction used

Photorealistic 4:5 editorial lifestyle photograph of a dignified silver-haired woman around 70 in a muted blue cardigan, sitting at a light oak kitchen table and engaged in conversation with an adult daughter around 43 in an off-white blouse. Natural attentive expressions, daughter mid-sentence making a gentle gesture, realistic skin texture and hands, subjects seated close together around the table corner, with both complete heads near the central 65% of the frame and faces around 40–48% of the portrait height for responsive crops. Warm daylight, muted navy and pale oak interior, two unmarked ceramic mugs, calm lower-left tabletop for desktop proof overlap. No visible hearing device, text, branding, clinic, medical equipment, exaggerated reaction or outcome claim.

### Review and handoff

Inspect both faces, hands, mugs and crops at actual desktop/mobile sizes before approving the Hero. The user's direction approval is not final rendered approval. If later layout changes materially affect the crop or proof placement, synchronize this entry. Keep the provider and product slot guidance separate and unchanged.

---

## IMG-PROVIDER-01 — Owners: "Meet the people behind HearCare"

### Placeholder purpose

This image puts real, identifiable people behind an anonymous healthcare decision. It answers the visitor's question, "Who is behind this practice, and can I trust them?" It sits beside the names, exact credentials ("Licensed Fitter and Dispenser of Hearing Instruments") and the practice's listen-first approach, directly above the Google reviews.

Its credibility depends entirely on being **genuine**. PAGE_STRATEGY §3 and DESIGN_SYSTEM require the documented real joint portrait, with both people kept in the crop.

### Recommended source type

**Real provider/team image preferred**

### Recommended composition

- **Orientation:** 1:1 square. Displayed at up to 360px wide on desktop, 280px on tablet and 320px on mobile, with a 16px radius. **Deliver at least 720×720** (1080×1080 ideal) for sharp high-density screens. The current source is only 411×411.
- **Subject placement:** Both owners fully inside the frame, centred as a pair, heads in the upper 45% of the square, with shoulders and some upper torso visible. No cropping through heads or between the two people.
- **Negative space:** Modest even margins on all sides. The page uses `object-fit: cover` on a square, so any non-square original must be recropped deliberately, not left to the browser.
- **Background:** Plain light grey or soft neutral, as in the current portrait, or a softly defocused real office interior. Avoid busy backgrounds that compete with the credentials text.
- **Desktop/mobile:** The caption below the image names both people. On mobile the portrait stacks above the heading, so it must read clearly at about 320px.

### Option 1 — Faithful restoration of the existing portrait (image-to-image only)

*Use only as an image-to-image restoration or upscaling task on the real file `hearcare-associates-kenneth-jill-sheppard.jpg`. Do not run as text-to-image.*

> Restore and upscale this exact photograph to 1440×1440 pixels. Preserve both people's facial features, identity, expressions, hairstyles, skin tone, wrinkles, glasses and proportions exactly as they appear; do not beautify, slim, smooth, de-age or alter any feature. Preserve their white lab coats, clothing details and pose. Keep the original light grey background, simply cleaned of compression artifacts and banding. Recover natural fine detail in hair and fabric, reduce JPEG noise, keep natural skin texture, keep the original color balance with true-to-life skin tones. No added elements, no text, no logos, no background replacement, no stylization. Output must remain a faithful, photographic likeness suitable for a professional healthcare website.

### Option 2 — New real joint portrait (photographer shot brief)

*Shot brief for a real photo session with Kenneth and Jill Sheppard. Not for AI generation of their likeness.*

> Professional environmental portrait, square 1:1, of the two practice owners standing side by side, shoulders slightly angled toward each other, relaxed and approachable with natural closed-mouth or soft smiles, looking toward the camera. Wardrobe: clean professional attire in solid colors, such as navy, soft blue or white, with lab coats optional to match the existing site look; no logos, name badges or busy patterns. Location: inside the real Sherman office at 1800 N. Travis St, against a clean wall or a softly defocused consultation-room background with no visible equipment screens, paperwork, signage or patient information. Lighting: large soft key light from the front-left with gentle fill, natural even skin tones, no harsh shadows. Camera: 85mm portrait lens at f/4 so both faces are sharp, background softly out of focus. Frame both heads in the upper half of the square with comfortable margins on all sides; also capture a wider 4:5 and 3:2 version for future layout flexibility. Natural retouching only: no skin smoothing beyond minor blemish cleanup, no reshaping.

### Option 3 — Real candid in-practice moment (photographer shot brief)

*Shot brief for a real session. Use only with a consenting real patient, family member or staff stand-in, with signed photo releases. Not for AI generation.*

> Candid documentary-style photograph, square 1:1 with extra room for a 4:5 alternate, inside the real Sherman office. Jill or Kenneth Sheppard is seated at a desk or small round table, turned toward an older adult client (or a consenting stand-in) and an accompanying family member, in a calm explanatory moment: listening, or pointing gently to a printed sheet held at an angle so no data is readable. The owner's face is clearly visible and in focus; the visitor is seen in three-quarter or over-the-shoulder view, with no identifiable patient information anywhere. Soft natural window light or warm soft-box light, muted blues and warm neutrals, uncluttered surfaces with no product boxes, brand displays, screens or signage. 35–50mm lens at f/2.8, natural expressions, not posed toward camera. This shows the practice's listen-first approach in its real setting; credentials stay in the page text, not in the image.

### Recommended option

**Option 1 now, with Option 2 scheduled.** The current photo is the documented, approved, authentic portrait, and restoring it faithfully solves the resolution problem without changing the strategy. Ideally the client supplies the original high-resolution file instead of an upscale.

A fresh real portrait (Option 2) is the best long-term asset. It can be shot in the Sherman office, which adds local authenticity, and it lets Step 5 choose a wider crop. Option 3 is valuable but depends on releases and careful privacy control, so treat it as a later enhancement and not a launch requirement.

### Real-image note

**REAL PROVIDER / CLINIC IMAGE REQUIRED. AI generation of these people is not acceptable.**

This image is evidence that the named, licensed owners exist and stand behind the practice. An AI-generated or "re-imagined" likeness would be a fabricated provider image and would undermine the whole trust section. The only acceptable AI step is faithful upscaling or cleanup of the real photograph (Option 1), checked side by side against the original for any change in features.

**Actions before launch:**
1. Ask the CSM for the original high-resolution portrait.
2. Re-host it on the filesafe CDN instead of hot-linking hearcareinc.com.
3. Keep `data-img-id="IMG-PROVIDER-01"` on the `<img>`.

---

## IMG-PRODUCT-01 — Options: "Hearing aids fitted to your everyday life"

### Placeholder purpose

This is the single product visual DESIGN_SYSTEM allows on the page. It helps visitors who arrive with brand or style questions and visitors worried about appearance. Its job is to make modern hearing aids feel **small, approachable and personal**, supporting the copy beside it: discreet styles *where they suit your hearing*, a fit and sound set for you, and help with phones and technology.

It answers the stigma objection ("Will people see them?") without overstating invisibility. It must not become a brand advertisement or a "giant product catalog." On desktop it stays fixed beside the three explanatory passages.

### Recommended source type

**Either real or AI image could work**

Licensed manufacturer imagery is accurate but usually branded and promotional. The site's Widex SmartRIC image is 232×253, too small, and Widex-specific. A clean, unbranded AI or licensed still life is acceptable, as long as the device looks like a realistic modern receiver-in-canal or behind-the-ear hearing aid.

### Recommended composition

- **Orientation:** 4:3 landscape. Generate at 1600×1200 or larger; the minimum is 1200×900.
- **Subject placement:** Product or hand slightly left of or at centre, with the device large enough to read at about 440px display width on desktop and about 350px on mobile.
- **Negative space:** Generous, calm background around the subject. No copy sits on the image, but the quiet space matches the editorial, uncluttered layout.
- **Crop considerations:** Displayed at 4:3 everywhere, with no responsive recrop. Keep the device and hand at least 10% from all edges.
- **Desktop/mobile:** On desktop the image sits beside the text in a 5/12 column, so it should hold up as a quieter companion to the text, not a hero. On mobile it stacks above the heading, so the device must still be clearly identifiable when small.
- **Scale honesty:** Show realistic size. Avoid macro shots that make the device look large, and avoid sizing that implies it is invisible.

### Option 1 — In-hand scale

> Product lifestyle photograph, 4:3 landscape. Close view of an older adult's open palm (age around 65–75, natural skin texture, a few visible veins and fine lines, short clean nails, a simple wedding band) gently holding a single modern receiver-in-canal hearing aid in a soft champagne-silver finish with a thin clear wire and small dome, shown at true real-world scale so its small size is obvious. The hand is slightly left of center, entering from the lower-left, with the hearing aid resting naturally between palm and fingers. Background: a softly out-of-focus home interior in warm whites and pale sky-blue tones, with gentle window light from the right. Macro-adjacent 100mm lens feel at f/4, the device sharp, the hand softly lit, natural shadows. No branding, engraving, logos or text on the device; no charging case; no packaging. Calm, clean, realistic healthcare product photography, natural color, not glossy, not advertising-perfect.

### Option 2 — Calm still life with everyday care items

> Editorial product still life, 4:3 landscape, top-down at a slight 30-degree angle. A pair of small modern receiver-in-canal hearing aids in a neutral beige-silver finish rest beside a small open matte grey hard-shell storage case and a slim cleaning brush on a pale natural linen surface, next to a folded pair of reading glasses for everyday context and scale. Arrangement is relaxed and slightly asymmetric, grouped left of center with generous calm space to the right. Soft diffused daylight from the upper left, gentle natural shadows, muted palette of warm off-white, soft sky blue (#78bbe9-adjacent) and deep navy accents from the glasses case. 60mm macro lens feel at f/5.6 so the devices are crisply defined while edges soften. No text, logos, engraving or brand marks anywhere; no charging dock or charging case; no batteries packaging; no water. Clean, believable, understated healthcare product photography.

### Option 3 — Worn and discreet: profile close-up

> Editorial close-up portrait detail, 4:3 landscape. Side profile from the shoulders up of a man in his late 60s with short natural grey hair, neatly trimmed sideburns and a soft navy crew-neck sweater, turned toward the left of frame as if listening to someone off-camera, with a relaxed, attentive expression. A small modern receiver-in-canal hearing aid in a hair-matching silver-grey sits behind his ear, with only its slim body and the thin clear wire subtly visible, realistically sized; it is noticeable on close inspection but discreet. The ear and hearing aid sit slightly right of center in sharp focus; the face is in soft partial focus toward the left. Background: a softly defocused warm home interior in off-white and muted blue. Soft natural window light from the left, gentle contrast. 85mm lens at f/2.2, shallow depth of field. Natural skin texture, realistic ear anatomy, correct device placement. No text, no logos, no visible branding on the device, no headphones or earbuds.

### Recommended option

**Option 1, the in-hand scale shot.** It directly answers "how big are they?" and "will people see them?" without claiming invisibility. The human hand keeps the image personal and in line with the page's everyday-life tone rather than a catalogue look. One device is also easier to keep brand-neutral and anatomically plausible than a worn device.

Option 2 adds a useful care-and-support cue (case and brush) that echoes the fitting education and maintenance copy, and is the safest AI generation. Option 3 is the most persuasive for the appearance objection but the hardest to get right: AI often misplaces receiver wires and distorts ears, so use it only after close artifact review.

### Real-image note

Real clinic imagery is **not required** here. A licensed manufacturer or stock product photo is equally valid **if** it shows no logo, is not tied to a single promoted brand, and is cleared for use. Check with the client before using manufacturer assets, since brand logos and imagery are manufacturer IP (RESEARCH §3, §9).

If the practice can photograph an actual device it fits, in a staff member's hand at the Sherman office, that would be preferable for authenticity. Remove branding or angle it away.

**Before publishing an AI version:** verify the dome and receiver wire geometry, a realistic size, no invented text or engravings, and no charging hardware.

---

## Handoff summary for Step 5

| Placeholder | Recommended | Source | Key risk to check |
|---|---|---|---|
| IMG-HERO-01 | Implemented kitchen-table conversation; awaiting rendered approval | AI lifestyle/editorial; responsive local WebP files | Preserve both faces; proof overlaps only on desktop; no patient/clinic/outcome attribution |
| IMG-PROVIDER-01 | Option 1 restoration now; Option 2 real reshoot later | **Real provider image required** | No AI likeness; get the high-res original; re-host on filesafe CDN |
| IMG-PRODUCT-01 | Option 1, in-hand scale | AI or licensed product photo | True scale; no logos or engraving; no charging case; correct RIC wire/dome |

**Suggested alt text** (to finalise in Step 5):
- IMG-HERO-01: "An older woman and an adult woman talking together at a kitchen table." Implemented; illustrative, with no patient or outcome attribution.
- IMG-PROVIDER-01: "Kenneth M. Sheppard, Jr. and Jill A. Sheppard, owners of HearCare, Inc. and Associates." This is already in the page.
- IMG-PRODUCT-01: "A small modern hearing aid resting in the palm of a hand."

**Implementation notes:**
- When a placeholder `div` is replaced with an `<img>`, keep `data-img-id`, set explicit `width` and `height`, and use `object-fit: cover`.
- Hero crop is now implemented with responsive CSS and reviewed at representative widths; preserve both faces if its layout changes.
- Use `loading="lazy"` for the provider and product images only, not the hero.

## User-supplied GHL hosting update

The user uploaded the approved AI-created Hero image to GHL and explicitly requested its insertion. Current IMG-HERO-01 source: https://files.leadconnectorhq.com/file/6af3305fddcd97ce5aa8a0c8/hearcare-kitchen-conversation.webp . The HTML now uses this hosted URL directly, without Base64 or the former local srcset. Existing dimensions, crop, alt, image ID and priority are preserved. Local WebP files remain archival assets; they are not the active image source. The scene remains an AI-created illustration, not practice/patient evidence.

Latest visual refinement retains the GHL-hosted IMG-HERO-01 source. Desktop CSS uses object-position 51% / 75% to give the conversation more emphasis; tablet/mobile retain 50% / 46%. The frame has a larger curved corner and restrained depth. No image regeneration or factual attribution change.

Restrained refinement supersedes the prior frame note: no offset outline; softer 100px upper-left desktop corner and 40px mobile corner. Mobile/tablet crop now uses 50% / 55%, preserving both faces. Source URL and image meaning remain unchanged.

User-requested restoration returns the photo frame/crop to b132802: 140px upper-left desktop corner, subtle offset outline, desktop position 51% / 75%, mobile/tablet 50% / 46%. The same GHL-hosted image is retained. This supersedes the restrained-refinement frame note.

Google proof now sits below the Hero actions as a compact inline row, not over the photograph. No badge exclusion zone is needed on the photo. Existing hosted image and crop remain unchanged.

Everyday-difficulty section rebuilt under user approval as an image-free asymmetric editorial section. Small functional line icons represent the three listening situations; no photo slot or new image generation is needed. IMG-HERO-01 and its locked implementation are unchanged.

Owner/proof Layout A approved: IMG-PROVIDER-01 remains the authentic 411×411 joint portrait, shown at up to 300px desktop / 280px mobile with both owners retained and no AI alteration. It now follows the introductory heading/copy on mobile. No new image or replacement likeness is used. Source URL unchanged; actual image rendering remains to be reviewed in GHL because local access failed.

User-supplied portrait hosting update: IMG-PROVIDER-01 now uses https://files.leadconnectorhq.com/file/6af3642f512d2edab67fe078/hearcare-associates-kenneth-jill-sheppard.jpg . Only the image URL changed; authentic portrait identity, dimensions, alt text, lazy loading, crop, image ID and layout are preserved. No live image availability or new resolution is assumed.

Mobile optimization: authentic GHL portrait is up to 140px beside license text at 380–639px, and up to 160px stacked below 380px. Both faces remain intact via unchanged contain rendering. Duplicate mobile caption is hidden; the full names remain visible in profiles. Desktop portrait unchanged.

User rejected the small side-by-side mobile portrait. IMG-PROVIDER-01 now remains centered above full-width credentials: 220px maximum, 200px on screens below 380px, with original contain rendering and unchanged GHL source. No new image or crop.


## Options Layout A implementation update

User approved Layout A + headline 1. This supersedes the old sticky image/above-heading mobile positioning: introduction left/image right, then three benefits across the full desktop width; headline before image on mobile. An authentic in-hand photograph is preferred. Pending that asset, the research-recorded clinic product URL https://hearcareinc.com/wp-content/uploads/2026/08/widexsmartric.jpg is used as a labelled Widex SmartRIC example, at native 232×253 resolution without magnification. Do not infer other models or capabilities from the image. Local network blocks retrieval; image appearance and availability require GHL review. No generated product is used.


## Options revision after updated GHL screenshots

User requested stronger design and content. Keep the approved headline and conditional hearing-aid premise. Replace the low-contrast image-led opening with a compact navy introduction, white headline, and a modest labelled product frame sized to the existing asset. White canvas and three editorial benefit columns focus on appearance, comfort and connection; mobile stacks them with simple dividers. Shorten repeated prose and integrate compatibility/suitability qualifications. Keep the original style guide and all eight brands, now shown as plain text in a supporting strip rather than button-like chips. Main prose stays 18px. No CTA, other section or integration changes. Existing product URL remains; its actual appearance is supported by the user’s new GHL screenshots, while remote retrieval is blocked locally. No generated product imagery. Awaiting rendered review, not locked.


User-supplied transparent footer logo: https://files.leadconnectorhq.com/file/6af40cdbddcd97ce5ac404ec/logo-hearcare-transparent.png . Replace only the footer image src; preserve its alt text, homepage link, responsive dimensions, navy background and all other page logos. No generated or edited logo is used.


User requested removing the footer logo. Remove only its linked image, retain the practice/service description, office details, utility links and automatic year, and reset the description’s top margin so no logo gap remains. The header logo and all other images remain unchanged.
