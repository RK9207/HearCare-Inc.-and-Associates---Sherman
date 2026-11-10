# Page strategy — HearCare, Sherman

Approved direction: November 10, 2026. Step 3 is the historical baseline. The user subsequently approved the Step 5 whole-page direction and the Hero rebuild described below. Hero implementation is ready for review, not visually approved or locked; publication is not authorized.

## Authority and scope

The user approved “Hearing tests and hearing aids in Sherman, TX” and Direction A with the integrated structure discussed in chat: everyday connection first, real owners early, and a clear test-first explanation. This document captures that agreement. Implementation details in DESIGN_SYSTEM.md operationalize it; they are design specifications, not newly verified clinic facts.

Read alongside CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, RESEARCH.md, and KEYWORD_RESEARCH.md. The original brief is `Project Brief - Hearcare Inc. and Associates.md`; there is no separate PROJECT_BRIEF.md. Source IDs below refer to RESEARCH.md. Preserve its historical evidence and the original brief.

**Contact decision overrides the brief's old number:** use the website's Sherman number **903-206-2442**, `tel:+19032062442`, and `sms:+19032062442` for now. The CSMs will supply tracking numbers later. Do not use Gainesville's 903-206-1692 on this page. Keep the temporary number easy to replace consistently across visible copy and action links; verify call and SMS routing when replacements arrive.

## Approved Step 5 Decisions

| Section / scope | Action | Reason | Approval | Affected files |
|---|---|---|---|---|
| Whole-page direction | Establish design/content direction | Carry forward the supplied HearCare visual standard, reduce repetition, prioritize genuine proof, and clarify assessment versus subsequent care | User: “I approve your overall direction with the additions you suggest” | Governing guidance; implementation remains section-gated |
| Hero | Rebuild only | Navy split composition; explicit service line; Headline 4; shorter test-first explanation; everyday-conversation benefit; kitchen-table lifestyle image | User: “Layout - Option A, Copy:- Headline 4 with recommended supporting copy direction and benefits, Imagery:- your recommended” | index.html, assets/hearcare-kitchen-conversation*.webp, PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, IMAGE_PROMPTS.md |
| Header | Rebuild only | Integrate navy brand surface with the Hero; blend the existing logo; white navigation; consistent pill Call and appointment actions; responsive fit | User approved the recommended integrated navy direction: “okay, please make the changes” | index.html, PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, review artifacts |

Current tracker: **locked final sequence: 1. Hero — APPROVED / LOCKED; 2. Everyday listening difficulties — APPROVED / LOCKED; 3. Owners and Google patient proof — APPROVED / LOCKED**. Approved implementations: Hero in 6a890ab, listening difficulties in afbf526, owners/proof including the user-hosted portrait and centered mobile owner layout in ce97231. Preserve all three without material changes or repositioning unless specifically authorized. Header remains implemented with no separate final lock recorded. Selected next existing section: process — “Understand your hearing before choosing anything.” Obtain current desktop/mobile screenshots before its individual assessment or edits. Remaining: header/mobile Call final review, process, options, payment, FAQ, location, final invitation, popup and footer. No section removal, addition or page-order change has been implemented.

## Objective, visitor, and offer

- Primary conversion: a call about hearing care at the Sherman practice. Text is a visible alternative; an appointment-request popup is secondary.
- Audience: inferred local adults noticing difficulty, family members helping them, and some existing wearers evaluating options. Do not imply age restrictions or pediatric service availability.
- Main visitor question: “Can this local practice help me understand my hearing and choose appropriate next steps?”
- Desired outcome: clearer everyday conversations and continued participation in life, presented as potential benefits, not guaranteed results.
- Offer: an appointment to assess hearing and discuss recommendations. No discount, free test, price, appointment duration, guaranteed availability, or trial is approved.
- Core positioning: understand your hearing first; explore options suited to your needs, lifestyle, and budget; receive fitting guidance and ongoing support where appropriate (S4–S7, S15).

## Search intent and click-to-action continuity

The approved strategic theme is **Hearing tests and hearing aids in Sherman, TX**. Approval is a page-direction decision, not validation of keyword performance. Actual primary/supporting campaign keywords, ad groups, search-term data, and ad copy remain NOT PROVIDED. Every phrase in KEYWORD_RESEARCH.md remains an AI candidate unless independently supplied and verified.

The first screen must show the services, Sherman, a plain-language benefit, accurate local details, and call/text plus Request Appointment actions. Step 5 approved H1: “Personalized Hearing Care, Right Here in Sherman.” Preserve explicit PPC service/location continuity with the prominent preceding line “Hearing tests & hearing aids in Sherman, TX.” Supporting copy: “Start with a hearing test and a clear explanation of your results. If hearing aids are appropriate, explore options suited to your hearing and everyday life.” Benefit: “Take the next step toward easier everyday conversations.” A hearing test does not imply that a device purchase is necessary.

Expected path: local service search → immediate service/location recognition → human relevance → credible practice and patient evidence → understandable appointment → suitable options → financial reassurance → contact.

Actual ad-to-page promise cannot be confirmed yet. On receiving ads, compare service, location, offer, price, credentials, and CTA against the page. Do not mirror an unsupported promise. Brand/style and financing themes support this page. Repair, tinnitus, hearing protection, and Gainesville need separate destinations if targeted. Do not target urgent medical needs, free/online testing, or imply audiologist credentials through the copy. “Near me” fit depends on campaign geography, which remains unconfirmed.

## Persuasion and visual arc

Begin with the everyday value of hearing conversations. Briefly acknowledge recognizable difficulties, then introduce authentic people and verified patient evidence before explaining care. Turn device capabilities into practical benefits. Resolve financial uncertainty and remaining questions before making location and contact concrete.

Warm image-led relevance → compact recognition → authentic portrait and proof → quiet process explanation → selective product detail → calm financial reassurance → concise FAQ → local map and final invitation.

Use a medium-length, scannable page. Target roughly 900–1,250 authored words excluding reviews, navigation, and embedded form content; this is a drafting budget, not a quota. Trim repetition before cutting useful answers. No full service catalog, long symptom lesson, fear-based health section, or repeated generic “why choose us” blocks.

## Final section order and roles

### 0. Persistent header and mobile Call action

- Conversion purpose / visitor question: “How can I contact them now?”
- Main message / key content: logo linked to https://hearcareinc.com/; desktop in-page navigation to Care, Our Practice, FAQs, and Location; temporary Sherman number; Request Appointment. Mobile shows logo and appointment action, with the Call action at the bottom.
- Emotional / trust role: orientation and immediate access to a real local practice.
- Visual role / treatment: approved integrated navy sticky header, original logo on its matching brand surface, white navigation and rounded Call/appointment controls; subtle separator and alignment with Hero container. On small screens, retain logo plus Request Appointment, allowing its label to wrap without truncation. Desktop navigation collapses before crowding.
- CTA: Call as the primary conversion, explicit Text alternative near contact details, Request Appointment as secondary. See design specifications for hierarchy.
- Previous / next relationship: available throughout; leads into the service/location answer in the hero.

### 1. Hero — local care for everyday conversations

- Conversion purpose: confirm relevance and let ready visitors act immediately.
- Visitor question: “Is this the right service in Sherman?”
- Main message: hearing tests and hearing aids in Sherman, with personalized next steps toward clearer conversations.
- Key content: the approved personalized/local H1 with a prominent hearing-tests/hearing-aids service/location line, concise test-first support and conversation benefit, owner-operated/licensed-practice microcopy, address/hours, and CTA group. Sources: S2, S4, S5, S7, S10–S12. The screenshot-supported 4.8/5 and 94 reviews use RESEARCH.md §3A/U1; no live refresh is claimed.
- Emotional role: hopeful recognition without shame or alarm.
- Trust role: exact location, accurate practice credentials, and Google rating badge only when verified material is supplied.
- Visual storytelling role: establish why the service matters before explaining its mechanics.
- Treatment: approved Option A, a navy text panel adjacent to a warm kitchen-table conversation photograph with a restrained overlapping white Google-proof panel on desktop. On mobile, the same proof panel appears in normal reading order before the actions, with image after local details. Preserve explicit service recognition and readable text; no text over faces. Generated lifestyle imagery illustrates everyday conversation and is not practice/patient evidence.
- CTA: Call 903-206-2442, separate Text link, Request Appointment popup.
- Previous relationship: expands the header's orientation into a service proposition.
- Next relationship: introduces a short, recognizable account of everyday difficulty.

### 2. Everyday difficulty — recognition without a symptom lecture

- Conversion purpose: connect the service to the visitor's own experience.
- Visitor question: “Does this sound like what I am experiencing?”
- Main message: missing words, struggling with background noise, or increasing the television volume are reasons to consider an evaluation (S4, S5, S13).
- Key content: three concise examples and a bridge toward understanding hearing through testing. Do not diagnose from symptoms.
- Emotional role: help visitors feel understood; preserve dignity and agency.
- Trust role: measured language instead of fear or exaggerated health consequences.
- Visual role / treatment: compact text-led passage with three short observations; no generic card grid or additional stock photo.
- CTA: none required; hero and persistent actions are nearby.
- Previous relationship: makes the hero's benefit personally relevant.
- Next relationship: raises the natural question of whom to trust with the next step.

### 3. Owners and patient proof — real people behind the care

- Conversion purpose: establish credibility before asking visitors to absorb the process.
- Visitor question: “Who is behind this practice, and what evidence can I trust?”
- Main message: owner-operated care led by Kenneth M. Sheppard, Jr. and Jill A. Sheppard, both Licensed Fitters and Dispensers of Hearing Instruments (S10–S12).
- Key content: real joint portrait; concise credentials; personalization philosophy; a dedicated, clearly titled Google Reviews subsection with supplied rating, count, review material, and Read all our Google reviews link when verified. Maximum six visible reviews desktop and three mobile.
- Emotional role: replace an anonymous healthcare decision with identifiable people and authentic patient experiences.
- Trust role: distinguish professional credentials from patient testimony. Do not promise an appointment with either owner; Sherman staffing is unknown.
- Visual role / treatment: authentic portrait as a visual anchor, followed by readable review excerpts or screenshots; no fabricated clinic scenes, credentials, stars, or review values.
- CTA: Request Appointment after the proof group; retain access to Call.
- Previous relationship: answers the trust question created by symptom recognition.
- Next relationship: credible people explain what the visit involves.
- Dependency: the dedicated reviews subsection and hero badge are required planned components, but verified Google material is pending. In an internal draft, mark missing assets honestly; do not publish placeholders or silently substitute directory ratings.

### 4. What happens next — understand before choosing

- Conversion purpose: reduce uncertainty and make contacting the practice feel manageable.
- Visitor question: “What happens if I take the next step?”
- Main message: testing informs recommendations; fitting and support follow if hearing aids are appropriate (S4–S7, S15).
- Key content: four connected stages: hearing test; results discussion; suitable options; fitting, education, and ongoing support where appropriate. Under testing, briefly explain a quiet setting, headphones with tones/speech, and a discussion of results (S5). Not every visitor proceeds to a device.
- Emotional role: calm control and understandable progress.
- Trust role: transparent process, no implied purchase obligation or guaranteed outcome.
- Visual role / treatment: numbered editorial sequence with small purposeful icons, horizontal on desktop if legible and vertical on mobile. Avoid a mandatory-path arrow suggesting all patients buy devices.
- CTA: Call and Request Appointment after the explanation.
- Previous relationship: turns practice credibility into a concrete experience.
- Next relationship: explains why recommendations and fitting are valuable in daily life.

### 5. Options fitted to everyday needs

- Conversion purpose: answer choice, appearance, comfort, and technology questions without a catalog.
- Visitor question: “Can the options fit my life, and will I understand how to use them?”
- Main message: the recommendation considers hearing needs, lifestyle, and budget; fitting and education help make appropriate technology useful (S4, S6).
- Key content: compact explanation of discreet styles subject to suitability, personalized settings, compatible phone features, instruction, and adjustments. Name the eight documented brands in a compact supporting list. Variety is evidence of choice, not proof of unbiased or superior advice.
- Emotional role: replace technology overwhelm with a sense of possibility.
- Trust role: explain benefit and limitations together; no universal invisibility, waterproofing, or guaranteed performance.
- Visual role / treatment: one authorized product image where useful, paired with two or three benefit explanations. Authentic product proportions; no manufacturer ad banners or invented devices.
- CTA: no additional large CTA needed; use a short appointment invitation if the section grows materially.
- Previous relationship: gives meaning to the process's recommendation and fitting stages.
- Next relationship: leads naturally from suitable choices to payment questions.

### 6. Payment and insurance assistance

- Conversion purpose: prevent unanswered cost concerns from stopping contact.
- Visitor question: “How do I find out what I might pay?”
- Main message: the practice can check hearing-aid insurance benefits and discuss payment options (S7).
- Key content: insurance assistance, CareCredit, major credit cards, financing availability, and Good Faith Estimate information. Distinguish hearing-aid benefits from test coverage; neither is guaranteed.
- Emotional role: reduce administrative burden and uncertainty without implying affordability for everyone.
- Trust role: acknowledge that test fees, device prices, specific plans, and financing terms are not supplied.
- Visual role / treatment: quiet text-led section with an insurance-help callout. No lifestyle image or price-comparison graphic.
- CTA: Call about benefits/payment; Text alternative. No application or guaranteed-approval promise.
- Previous relationship: addresses the practical objection raised by considering devices.
- Next relationship: clears space for the remaining individual questions in FAQ.

### 7. Focused FAQ

- Conversion purpose: resolve the final objections without expanding the page into a medical guide.
- Visitor question: “What else do I need to know before contacting them?”
- Main message: clear answers about evaluation, device suitability, visibility, phone compatibility, support, insurance, and appointment requests.
- Key content: approximately six focused answers; CONTENT_DIRECTION.md defines priorities and source boundaries. Avoid repeating whole previous sections.
- Emotional role: let the visitor explore concerns privately and at their own pace.
- Trust role: honest limits; no invented prices, duration, staffing, trial terms, or insurance coverage.
- Visual role / treatment: accessible text-led accordion, no decorative imagery.
- CTA: persistent contact actions suffice; a small contact invitation can follow the final answer.
- Previous relationship: deals with questions not settled by payment reassurance.
- Next relationship: returns the reader from questions to a real Sherman destination.

### 8. Sherman location and final invitation

- Conversion purpose: make attendance practical and turn confidence into action.
- Visitor question: “Where would I go, and how do I request a visit?”
- Main message: start by contacting the Sherman practice to understand the next step.
- Key content: 1800 N. Travis St, Suite D, Sherman, TX 75092; Monday–Thursday 9am–5pm; Friday by appointment only (S2). Supplied responsive map; Get Directions below it with direction icon. Follow with a short final invitation and call/text/request actions.
- Emotional role: a concrete, achievable next step.
- Trust role: consistent local details; no invented parking, accessibility, travel times, or same-week availability.
- Visual role / treatment: map and contact details in a contained layout, transitioning into a distinct deep navy final CTA band. No unrelated stock image.
- CTA: Call 903-206-2442, Text, Request Appointment. The final request button opens the same form as all others; do not introduce a duplicate inline form.
- Previous relationship: practical location details follow objection resolution and immediately precede the final action.
- Next relationship: popup, if requested, explains the request before fields; footer supplies policy and website access.

### 9. Appointment popup and footer

- Conversion purpose / visitor question: “How do I request an appointment, and what am I submitting?”
- Main message / key content: Request an Appointment heading, brief request-versus-confirmation explanation, supplied GHL embed, clear close control, and phone fallback. Footer: Privacy Policy, Visit Our Website, local contact, copyright.
- Emotional / trust role: visitor control, clear expectations, preserved source form and consent behavior.
- Visual role / treatment: focused modal; scrollable content on small screens; quiet footer. No auto-open, countdown, or unrelated imagery.
- CTA: use the provider's actual submit action; do not claim instant scheduling. Do not submit a real lead during testing without explicit authorization.
- Previous / next relationship: all appointment buttons converge here; closing returns focus to their trigger. Footer completes the page without a competing conversion funnel.

## Dependencies and handoff checks

- Resolved for now: phone conflict. The user's approved temporary number is 903-206-2442; tracking numbers are future replacements, not a current strategy blocker.
- Pending before public completion: verified Google rating, count, and supplied review material; approved usable imagery and logo availability; actual form behavior and successful rendering; factual and functional review.
- Unknown and omitted unless confirmed: test cost/duration, trial availability/terms, provider staffing, specific insurers/Medicare, warranties, years in practice, and clinic accessibility.
- Pending campaign validation: ad copy, actual keywords, geography, tracking/attribution requirements. Do not invent analytics IDs or record health-related form content in analytics.
- Builder must maintain a missing-input list. Drafting can proceed with explicit internal asset placeholders after builder approval; publication cannot treat them as completed proof.
- Scan test: H1 and section headlines alone should communicate local services, why they matter, credible people, understandable care, payment help, location, and next action.
- Verify header and sticky CTA behavior, actual tel/SMS destinations, appointment popup on every trigger, keyboard operation, mobile layouts, map/directions and privacy links. Check no form auto-opens. Do not claim conversion performance from design inspection.

## Next gate

These documents guide the first draft; they do not authorize building or publication. Present a separate Claude/Codex recommendation and wait for the user's builder selection before Step 4.

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

Latest user-approved review display: show “90+ Google reviews” in the Hero badge, accessible aggregate label and reviews section. The rating remains 4.8/5. This is conservative display wording based on the recorded 94-review screenshot evidence; preserve the historical source count in RESEARCH.md rather than rewriting that evidence.

## Compact Google proof approved by reference

User requested the supplied screenshot badge style: inline Google icon, white 4.8 rating, gold fractional stars, and 90+ Google reviews, placed below Hero contact actions on desktop/mobile. Remove the floating white badge card, preserving the existing Google destination, accessible aggregate label and screenshot provenance. No other business details from the reference are adopted. Prior photo-overlay/proof-before-actions guidance is superseded. Pending rendered approval.

## Hero approval and next screenshot checkpoint

User explicitly approved the current Hero. Mark it locked; no HTML or CSS changes are part of this approval record. Proposed successor remains the existing everyday-difficulty section: the Hero answers what/where/how to act; a compact recognition passage next answers whether the service relates to the visitor’s daily experience. A quieter light section provides visual relief after the navy/photo opening and sets up the owners/proof question. Obtain current desktop and mobile screenshots before analyzing or editing this selected section. No removals, additions or sequence changes have been approved or implemented.

## Approved everyday-difficulty rebuild — implementation for review

The user approved the asymmetric editorial recommendation with headline 4: “Recognize any of these listening difficulties?” Current placement remains immediately after the locked Hero and before owners/patient proof. Visitor question: “Do these everyday experiences sound familiar?” The left column contains the chosen headline, brief introduction and family acknowledgement; the right column contains three purposeful icon-led rows (missing words, conversations in noise, TV volume). A full-width, restrained reassurance band states that these experiences do not automatically establish hearing loss or hearing-aid need, preserves the value of identifying unnoticed changes, and keeps the #care visit-explanation link. It is not a diagnostic checklist or a new primary conversion.

Mobile stacks introduction/family context, observations, then reassurance/link. Retain comfortable prose size and simplify spacing; no photo, AI generation, separate sales CTA, generic card grid, or section reorder. The remaining mobile closing area was inspected in an actual local current-state rendering before edits, using the code and the user's screenshots together. Hero/header markup, Hero styling, contact configuration and integration scripts remain unchanged. This section is implemented for rendered review, NOT LOCKED; final approval is still required. Owners/reviews and other remaining sections have not been individually assessed or changed.

## Space-utilization refinement requested by user

The user requested better use of the available section width. Supersede the asymmetric split with a full-width heading/introduction and one continuous white surface containing three aligned editorial columns on desktop. This is a shared panel with separators, not separate repeated cards. Consolidate family acknowledgement, diagnostic reassurance and visit link in the compact closing area. On mobile, stack the icon-led examples within the shared panel, followed by closing context. Preserve all section wording, existing service link, locked Hero, header and integrations; no section reorder or removal. Implementation remains pending rendered approval.

## Listening-difficulties final approval and next checkpoint

User: “I would like to approve this section, lets move to the next section.” Lock the listening-difficulties implementation in afbf526, including the shared three-column desktop panel, stacked mobile examples and consistent 18px closing copy. No HTML/CSS change accompanies this record. Proposed successor is the existing owners/patient-proof group: recognition answers “Does this sound familiar?”; named licensed owners and genuine patient experiences address “Who can I trust for the next step?” The real portrait provides a visual anchor after the quiet recognition panel, with reviews supporting the contact decision before process explanations. Request current full desktop/mobile screenshots of the owners and review areas, then wait before individual assessment or edits.

## Approved owners and Google proof rebuild — Layout A

User selected “Layout A + Headline 1 on both as recommended.” Retain **Meet the people behind HearCare** and **What patients say on Google**. Owner introduction now precedes the portrait on all viewports. Preserve the real joint portrait at a modest 300px desktop / 280px mobile display, shared visible exact licensed status, both full names and Jill's B.S. Each owner has a native keyboard-operable View qualifications disclosure retaining the complete original education/licensing/coursework facts. This consolidates repetition without concealing the essential licensed credential or implying audiologist/doctor status, years of experience, appointment staffing or guaranteed outcomes.

Use a distinct softly tinted reviews area with Google icon, screenshot-supported 4.8 aggregate and user-approved 90+ display, gold fractional stars, and three full verbatim reviews: Karyn Feltner, garey gaston and Sandra Walker. The other transcriptions remain preserved in RESEARCH.md. The dedicated Google heading, all-reviews link, listing qualifier and individual-experience disclaimer remain. This approved selection supersedes the prior six-card desktop implementation. Closing contact invitation puts Call first and Request Appointment second, preserving existing destinations/data hooks and form integration.

Current section is implemented for rendered review, NOT LOCKED. The locked Hero and recognition section, header and all other sections are unchanged. Owner image URL is unchanged; the environment could not load that external image, so final actual-photo appearance must be reviewed in GHL. No new stock/AI image or generated provider likeness is authorized or used. No page-order change or new section is introduced.

## User-requested mobile optimization

Optimize the current owners/reviews group below 640px only. Use a compact authentic portrait beside visible licensing context from 380–639px, then full-width owner disclosures and values; below 380px, stack a smaller 160px portrait and full-width credentials. Hide only the duplicate photo caption on mobile, retaining both full names and authentic image alt. Reduce spacing, retain 18px principal prose/full quotations, use comfortable disclosure targets and full-width aligned contact actions. Desktop layout, all page markup/wording/quotes/links and both locked sections are unchanged. Real GHL portrait fetch remains blocked locally and is not substituted with another image. Final GHL photo/rendering review remains required; section is not locked.

## Mobile portrait layout correction

The user rejected the compact portrait-and-licensing row shown in the GHL screenshot. Replace it below 640px with a centered 220px authentic portrait (200px below 380px), followed by full-width licensing text and vertically stacked owner profiles. Use full-width outlined native qualification controls with a clear right-aligned chevron and at least 48px height. Preserve all wording, review quotations, source image, desktop styling and locked sections. This supersedes the prior side-by-side mobile optimization. Awaiting rendered approval.

User-requested mobile centering: center the owner heading/introduction, shared license, names, qualification controls and values below 640px. Portrait remains centered. Keep expanded qualification prose and review quotations readable; main review content remains left-aligned. Desktop and locked sections unchanged.

## Owners/proof final approval and next checkpoint

User: “Okay, I approve this section. Let’s move to the next section.” Mark the complete owner/Google proof group in ce97231 APPROVED / LOCKED, including the centered mobile owner presentation, hosted authentic portrait, qualification disclosures, three verbatim reviews and Call-first invitation. No HTML/CSS changes accompany this approval record. Proposed successor remains the existing process section: credible people and patient experiences address trust; the process then answers what happens when the visitor takes the next step. Shift toward a calm, understandable care explanation and inspect its visual transition against the locked proof group. Request current full desktop/mobile screenshots, including steps, test-details disclosure and contact actions; wait before individual assessment or editing.
