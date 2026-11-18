## Realistic hearing-aid style images, November 18, 2026

User requested realistic close-ups similar to the two supplied ear/device photos, replacing the four graphical diagrams. Replaced all four inline SVGs with AI-generated illustrative photographs: BTE with a thick clear sound tube/custom earmold; RIC with slim behind-ear housing/thin receiver wire; ITE custom shell; a CIC example for the ITC/CIC/IIC family. Original PNGs remain in /workspace/generated_images; WebP copies retain 1448×1086 dimensions and use no retouching. New files: assets/hearing-aid-style-bte.webp, hearing-aid-style-ric.webp, hearing-aid-style-ite.webp, hearing-aid-style-canal.webp. Asset commit b9b32397ea0f4169c620c229f2a0278bacd3dedf provides immutable GitHub raw URLs. These are illustrative scenes, not manufacturer photographs, specific model representations or actual HearCare patients. Visible note: “Illustrative examples. Actual appearance varies.” The canal card identifies its image as a CIC example. Supplied reference photos informed generation; no third-party stock photos were copied into the page.

Cards now show full-width 4:3 photos above the copy at all sizes. Desktop retains four columns, tablet two, mobile one. Explicit dimensions, lazy loading, async decoding and descriptive alt text included. Existing Widex photo, descriptions, caveats, Other options, brands, contact destinations and all other sections are unchanged.

QA: all four new images decoded at 1448px natural width in the browser fixture. Eleven widths from 320 to 1920px passed overflow/card checks. Scoped axe WCAG 2/2.1 A/AA checks passed at 393 and 1440px; appointment dialog and Escape close passed. Desktop/mobile photos and framing visually reviewed. Exact local assets and cached fonts were used; existing Widex product pixels remain unverified because the environment blocks the GHL host. No live lead/call/SMS tests or GHL deployment.


## BTE and RIC image revision, November 18, 2026

User requested a more realistic BTE fit and a visible RIC receiver. Regenerated only these two illustrative photos. BTE uses a rear three-quarter view, smaller partly occluded housing, clear sound tube and earmold. RIC shows a thin wire connected to a receiver and translucent dome at the canal entrance. Both remain 1448×1086 WebP. Originals preserved in /workspace/generated_images/hearing-aid-style-bte-remade.png and hearing-aid-style-ric-remade.png. New immutable image URLs use asset commit 1f43992f7cbddec5500f8e5ef1ccc2290086609e. ITE and canal images, layout, content and contact behavior are unchanged. These remain AI-generated illustrative examples, not verified manufacturer images.

Revision QA: 393px and 1440px image decoding, overflow, scoped axe and appointment-dialog checks passed. Both card layouts visually inspected; receiver/dome is visible in the RIC image. The only HTML changes are the two image URLs and RIC alt text. Other assets remain unchanged.


## Hearing aid image hosting update, November 18, 2026

Replaced the four comparison image URLs with the user-supplied GHL Media Library links for BTE, RIC, ITE and the canal-style CIC example. Only image sources changed; existing alt text, layout, copy and all integrations are preserved. Canonical HTML and complete copy/paste artifact are byte-identical. Normalized comparison confirms no unrelated HTML changes.

Remote check: the environment proxy rejected all four GHL image-host connections with CONNECT 403. URL mapping is verified; live image availability needs GHL/browser review.
