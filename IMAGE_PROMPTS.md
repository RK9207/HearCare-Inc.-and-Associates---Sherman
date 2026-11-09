# IMAGE_PROMPTS.md — HearCare, Inc. and Associates (Sherman, TX)

**Step:** 4B, image prompt reference for Step 5
**Prepared:** November 10, 2026
**Page:** Hearing Tests & Hearing Aids in Sherman, TX (`index.html`, Step 4A first draft)
**Read with:** PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, RESEARCH.md

---

## Scope

The Step 4A draft has exactly **three** intentional image placeholders. This file covers only those three. No other section has a placeholder, and none should receive an image just to fill space. The design system keeps the difficulty, process, payment, FAQ, review, location and final sections image-free.

| Placeholder | Section | Current state in `index.html` | Source preference |
|---|---|---|---|
| IMG-HERO-01 | Hero | Designed placeholder (`.hc-ph--hero`) | AI-generated lifestyle/editorial image appropriate |
| IMG-PROVIDER-01 | Owners: "Meet the people behind HearCare" | **Real owner portrait in use** (411×411, hot-linked from hearcareinc.com); placeholder appears only if it fails to load | Real provider/team image preferred |
| IMG-PRODUCT-01 | Options: "Hearing aids fitted to your everyday life" | Designed placeholder (`.hc-ph--product`) | Either real or AI image could work |

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

### Placeholder purpose

This is the first image a visitor sees, beside the H1 "Hearing Tests & Hearing Aids in Sherman, TX." Its job is the strategy's opening move: show *why hearing matters* before the page explains *how care works*. It should let a visitor, or the adult child searching on their behalf, recognise the outcome they want: being part of an ordinary conversation again, easily and without strain.

The image must support hopeful recognition without shame or alarm, as PAGE_STRATEGY §1 sets out. It must not compete with the H1 or the call button. It also hosts the Google rating badge (4.8 · 94 reviews), which overlaps its bottom-left corner.

### Recommended source type

**AI-generated lifestyle/editorial image appropriate**

No real lifestyle photography exists for the practice. The site's own heroes are licensed Getty stock files, which are wide 2560×400 banner crops and unusable at 4:5. An AI-generated or newly licensed editorial image is appropriate, as long as it reads as a generic lifestyle scene and not as a HearCare patient or location.

### Recommended composition

- **Orientation:** 4:5 portrait. Generate at 1600×2000 or larger; the minimum delivered size is 960×1200.
- **Responsive crop:** The same file is shown at **4:3 on tablet and mobile**, using a centre crop that keeps roughly the middle 60% of the height. Keep all faces and the key interaction **between about 22% and 70% of the image height**. Do not place faces at the very top.
- **Subject placement:** Primary faces slightly right of centre or upper-centre. The image sits in the right column on desktop, so subjects facing slightly *left*, toward the headline, works best.
- **Badge zone:** The bottom-left quadrant (roughly the lowest 25% and left 45%) holds the rating badge. Keep it calm and low in detail, such as a table edge, soft fabric or out-of-focus foreground, with no hands, faces or hearing aid there.
- **Negative space:** No text sits on the image, so heavy negative space is not needed. Moderate breathing room at the top keeps the 4:3 crop from feeling cramped.
- **Desktop/mobile:** On mobile the image appears *after* the buttons, at about 350px wide. The interaction must still read at that size, so avoid very wide group shots with small faces. Two people, or three at most.
- **Frame treatment:** The page applies a 16px radius. Do not generate vignettes or rounded borders.

### Option 1 — Lifestyle outcome: kitchen-table conversation

> Editorial lifestyle photograph, 4:5 vertical. A woman in her early 70s with short silver hair and reading glasses pushed up on her head sits at a light oak kitchen table in a bright, lived-in North Texas home, leaning in slightly as she listens to her adult daughter (mid-40s) who sits across the corner of the table, mid-sentence, gesturing gently with one hand. The older woman's expression is relaxed and attentive, a small genuine smile, eyes on her daughter, clearly following the conversation without effort. A small, discreet receiver-in-canal hearing aid is just visible behind her ear in a neutral beige or silver tone, not a focal point. Two ceramic coffee mugs with no markings, a folded linen napkin. Soft late-morning window light from the left, warm natural tones with muted blue accents in her cardigan and the background kitchen textiles. Faces positioned in the upper-middle of the frame, subjects turned slightly toward the left edge; the lower-left foreground is a calm, softly out-of-focus table surface. Shot on a full-frame camera with a 50mm lens at f/2.2, shallow depth of field, natural skin texture, candid documentary feel, not posed for camera, nobody looking at the lens. Realistic, understated healthcare advertising photography, gentle contrast, no text, no logos.

### Option 2 — Family/community warmth: porch visit

> Editorial lifestyle photograph, 4:5 vertical. On a shaded front porch of a modest single-storey brick home in a quiet North Texas neighborhood in late afternoon, a man in his mid-60s to early 70s with a trimmed grey beard, wearing a soft chambray button-up shirt, sits in a wooden rocking chair, turned toward his adult son (late 30s) who sits on the porch step beside him. They are sharing an easy laugh mid-conversation, the father's head tilted toward his son, comfortable and engaged. A small, discreet hearing aid is barely visible behind the father's ear. Warm golden-hour side light filtering through trees, soft green and brick-red background tones kept muted, blue-grey wardrobe accents. Faces in the upper-middle third, slightly right of center, both oriented toward the left of frame; the lower-left foreground is the porch floorboards and soft shadow, simple and uncluttered. 85mm lens feel at f/2.0, gentle background blur, candid moment, unposed, no one looking at the camera, natural skin and hair detail. Authentic, warm, restrained healthcare editorial style, no text, no house numbers, no logos, no signage.

### Option 3 — Social participation: small dinner with friends

> Editorial lifestyle photograph, 4:5 vertical. A woman in her late 60s with natural grey curly hair, wearing a soft navy knit top, sits at a small round table in a warmly lit neighborhood restaurant during a quiet early-evening dinner, turned toward a friend of similar age seen in three-quarter view at the right edge of frame. She is listening closely and responding with a relaxed, knowing smile, clearly following the conversation despite the gentle background activity. Background diners are fully out of focus as soft bokeh shapes, no legible menus or signs. Warm tungsten ambient light balanced with soft window light, muted navy and warm-wood palette. The woman's face sits at about 40% of the frame height, slightly right of center, gazing left toward her friend; the lower-left area is a softly blurred tabletop with a plain water glass and folded napkin. 50mm lens at f/1.8, shallow depth of field, candid documentary style, natural skin texture, no one looking at the camera, no visible hearing device emphasis. Realistic, dignified, understated healthcare advertising photography, no text, no logos.

### Recommended option

**Option 1, the kitchen-table conversation.** It most directly expresses CONTENT_DIRECTION's primary outcome, "clearer conversations and staying engaged with the people … that matter," in an everyday setting that both patients and family members recognise. The adult-child figure speaks quietly to the inferred family-member audience without making the patient passive.

It is also the easiest composition to control for the badge zone and the 4:3 mobile crop. Option 3 is the stronger choice if Step 5 wants to echo the "background noise" difficulty from section 2, but restaurant scenes risk signage and busy-background artifacts. Option 2 is the warmest local feel, but outdoor light and porch details are harder to keep consistent and free of text.

### Real-image note

Real clinic imagery is **not** preferred for this slot. The strategy specifically wants the hero to show everyday life rather than the clinic or product. If the client has authentic, consented photos of real patients in everyday settings, those would outperform AI. Without them, AI or licensed editorial stock is appropriate.

**Before publishing an AI hero:** check hands, ears and the hearing aid shape closely. Make sure the device looks like a plausible small RIC/BTE and not an earbud. Confirm the image is not described anywhere as a HearCare patient.

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
| IMG-HERO-01 | Option 1, kitchen-table conversation | AI lifestyle/editorial (or licensed editorial stock) | Faces inside the 4:3 mobile crop band; calm bottom-left badge zone; plausible hearing aid; not presented as a HearCare patient |
| IMG-PROVIDER-01 | Option 1 restoration now; Option 2 real reshoot later | **Real provider image required** | No AI likeness; get the high-res original; re-host on filesafe CDN |
| IMG-PRODUCT-01 | Option 1, in-hand scale | AI or licensed product photo | True scale; no logos or engraving; no charging case; correct RIC wire/dome |

**Suggested alt text** (to finalise in Step 5):
- IMG-HERO-01: "An older woman enjoying an easy conversation with her daughter at the kitchen table." Adjust to the chosen option.
- IMG-PROVIDER-01: "Kenneth M. Sheppard, Jr. and Jill A. Sheppard, owners of HearCare, Inc. and Associates." This is already in the page.
- IMG-PRODUCT-01: "A small modern hearing aid resting in the palm of a hand."

**Implementation notes:**
- When a placeholder `div` is replaced with an `<img>`, keep `data-img-id`, set explicit `width` and `height`, and use `object-fit: cover`.
- For the hero, add `object-position` tuned to the final image so the 4:3 crop keeps the faces.
- Use `loading="lazy"` for the provider and product images only, not the hero.
