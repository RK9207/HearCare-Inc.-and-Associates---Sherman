# Reusable Services and Hearing Aids changes

Saved November 18, 2026 at the user's request, for adapting to another page.

## Reference implementation

Repository: RK9207/HearCare-Inc.-and-Associates---Sherman, branch codex/hero-redesign.
Complete page: index.html and review/hero-review.html (byte-identical).
Reference HTML commit: dc0a162e5d422ed259c7ce64aceaa9ee90888888.

This checklist describes the final design, including later image revisions and GHL hosting. Use the latest source of the next page; adapt only the authorized sections and preserve its branding, verified services, phone/SMS links, forms, tracking and location. Do not copy Sherman-specific claims, brands, providers or contacts without checking applicability.

## Services selector

- Move the headline and short introduction above the entire layout.
- Keep all four service names visible: hearing tests; hearing aid selection & fitting; hearing aid repairs; ongoing care & adjustments.
- Make all four selectable, with one active image and description shown at a time. Preserve useful details rather than deleting them for brevity.
- Desktop: selected image/caption on the left; four numbered choice buttons on the right. Navy/white active state, pale-blue inactive state, clear focus indication.
- Mobile at 767px and below: compact 2×2 choices above the selected image. Selection survives breakpoint changes.
- Four distinct realistic illustrative service photos, each visibly labelled “Illustrative service image.” These are AI-generated examples, not actual clinic staff or patients.
- Accessible tabs: aria-controls/labelledby, selected state, roving tabindex, arrow keys, Home/End; focusable active panel. Without JavaScript all four panels remain readable and nonfunctional choices stay hidden.
- Retain the existing visit link; keep Services and Hearing Aids separate.
- GHL-hosted WebP files, not Base64. Explicit dimensions, lazy loading and async decoding.

## Hearing Aids visual guide

- Preserve “Hearing aids chosen around your life” where appropriate and the conditional premise “When hearing aids are appropriate.”
- Navy feature: larger existing Widex SmartRIC product image with a 2px image-frame padding, short introduction, three concise benefits covering appearance, personalized fit/settings and compatible phone features.
- White text on navy; dark body text on pale surfaces. Retain feature/model/phone compatibility caveats.
- Replace the text-heavy style disclosure with four always-visible image-led cards: BTE, RIC, ITE, and canal designs (ITC/CIC/IIC family).
- Realistic close-up photos of devices worn at the ear; matching warm neutral framing. No graphical ear diagrams in the final version.
- Final BTE photo uses a rear three-quarter angle, a modest housing tucked behind the ear, clear sound tube and earmold. This replaces the original oversized/artificial-looking BTE image.
- Final RIC photo shows the actual receiver and silicone dome at the canal entrance, connected to a thin wire. This replaces the earlier image whose receiver was not visible.
- ITE image shows the custom outer-ear shell. Canal image is explicitly identified as a CIC example, not a depiction of every canal style.
- All four are AI-generated illustrative photos; visible shared note: “Illustrative examples. Actual appearance varies.” Do not present them as specific manufacturer models or real patient photos.
- Full-width 4:3 photo above short copy in each card. Four columns on wide desktop, two at tablet widths, one on mobile.
- Preserve useful suitability/visibility, controls, battery-life and connectivity qualifications.
- Separate “Other options to ask about” row: extended-wear devices with current local availability/suitability caveat; middle-ear implants require specialist assessment, without claiming the practice performs surgery.
- Retain eight manufacturer names only where verified: Widex, Starkey, Unitron, Signia, Oticon, ReSound, Rexton, Phonak.
- Close with “Find an option that suits your hearing,” a Call CTA and the existing appointment action.

## Call buttons and writing preferences

- Call CTA buttons use a 999px pill radius, sky-blue fill, dark text/phone icon and existing black border. Shared class: .hc-btn--call.
- The separate full-width sticky mobile call bar stays borderless; its shape was not changed by the pill CTA update.
- Avoid sentence dashes and unnecessary forced line breaks. Keep copy easy to scan, with benefits and qualifications close together.

## Final image sources

Services (user-uploaded GHL Media Library):

- https://files.leadconnectorhq.com/file/6afd417c7c3b573a62c2f135/service-hearing-tests.webp
- https://files.leadconnectorhq.com/file/6afd417c7c3b573a62c2f12a/service-hearing-aid-fitting.webp
- https://files.leadconnectorhq.com/file/6afd417c77a01e46226d4752/service-hearing-aid-repair.webp
- https://files.leadconnectorhq.com/file/6afd417c77a01e46226d4742/service-hearing-aid-support.webp

Hearing Aid style cards (user-uploaded GHL Media Library, including revised BTE/RIC):

- https://files.leadconnectorhq.com/file/6afd49ddfdf6b54fd7b19a0a/hearing-aid-style-bte.webp
- https://files.leadconnectorhq.com/file/6afd49dda30b968e3f0b1b2f/hearing-aid-style-ric.webp
- https://files.leadconnectorhq.com/file/6afd49dd77a01e46226e2e7f/hearing-aid-style-ite.webp
- https://files.leadconnectorhq.com/file/6afd49ddfdf6b54fd7b199ff/hearing-aid-style-canal.webp

Featured Widex product:

- https://files.leadconnectorhq.com/file/6af44925fbdd54a827b67c4f/widexsmartric.jpg

Original generated WebP assets remain in assets/ and Git history. Final HTML loads user GHL URLs. Reuse across another practice should preserve the illustrative context and verify product/service relevance.

## Validation and handoff

- Check desktop/mobile layout, all four Services selections, keyboard access, breakpoint retention and no-JavaScript content.
- Check four style-card images, crops, alt text, loading, no horizontal overflow, phone destinations and shared appointment behavior.
- Previous fixture checks passed widths from 320 to 1920px and scoped WCAG A/AA axe checks. These results do not substitute for checking the adapted page.
- The environment proxy blocked GHL image-host requests; final user-hosted image loading still needs a browser/GHL review. Local exact assets were used in prior render tests.
- Keep index.html and the complete copy/paste artifact synchronized. Provide the complete pinned GitHub RAW HTML link after edits. Do not claim the GHL page is published unless actually deployed.


## Sherman section QA/QC, November 18, 2026

Applied the same verified section fixes as Gainesville: flexible Services choices/numbering for enlarged text, locally wrapped Hearing Aids contact controls, visible scrolling keyboard focus with sticky-area margins, and valid div-based tabpanel markup. Standard layout and extended text/spacing/accessibility checks passed. Sherman phone/form and all unrelated source are preserved. See review/SHERMAN_SECTIONS_QC.md for test evidence and live GHL image limitations. Future reuse should include these corrections.


## Mobile Menu label, November 23, 2026

User requested “Menu” with a hamburger icon instead of “Explore this page” with an arrow, for both mobile versions. The saved sources already used a hamburger-only header toggle; added the visible Menu text and adjusted its pill control to fit the label plus icon. The closed control shows the hamburger; the expanded control retains its close icon. Existing aria-expanded/controls, Escape focus return, section-link dismissal, contact links and desktop navigation are preserved. Both pages passed interaction/header-fit checks at 320, 393, 768, 1024 and 1440px. HTML artifact pairs match. No deployment to GHL.
