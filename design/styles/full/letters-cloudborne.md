# Letters — cloudborne everyday tools (full original spec)

> Verbatim reference supplied by the owner. The condensed working version is
> `../letters-cloudborne.md`. When the two differ, this file wins.

## Overview

An airy, light software-marketing style that makes administrative work feel almost weightless. Rounded sans-serif typography, powder-blue skies, white sculptural objects and softly floating interfaces balance practical explanations with a little wonder. It suits approachable productivity products with substantial capabilities to explain, using sparse compositions rather than dense technical spectacle.

### Essentials

- A promise floats above a physical metaphor: the opening uses a centered 80px/0.9 semibold headline with -0.04em tracking, a narrow support line and one dark action above white dimensional artwork.
- The page behaves like white paper opening onto sky: most content stays on white or #f5f5f5, while blue is concentrated in the opening and a rounded conversion island; saturated #2597d0 appears only in small details.
- Typography has rounded edges but a tight embrace: 44px/1.1 section headings carry -0.04em tracking, and selected headings interrupt a phrase with a small white dimensional icon tile.
- Actions resemble small polished lozenges: 48px height, 100px radius, 17px semibold text and a near-black primary fill; supporting card actions are white rather than outlined.
- Capabilities are miniature stage sets: paired 650px-wide, 646px-tall panels with 48px corners and 40px padding hold isolated white UI fragments, bottom fades and a clear text hierarchy.
- Every landing page carries a white object sculpture and a floating interface vignette: use layered cards, an envelope, a tool or an abstract workflow object with soft blue-gray shadows when no product-specific object exists.
- The ending lands back in the real product: a centered 44px promise and dark CTA sit above a pale device/interface ensemble, followed by a spacious white footer with the logo left and four compact link columns right.

## Colors

### Brand

| Name | Value | Token | Roles | Use |
| --- | --- | --- | --- | --- |
| Blue horizon | `#779bc1` | `--color-sky-top` | background | Top of the atmospheric blue gradient. |
| Open sky | `#9abfda` | `--color-sky-middle` | background | Middle sky stop at 58%. |
| Pale horizon | `#cbdfec` | `--color-sky-bottom` | background | Bottom of the sky gradient. |

### Accent

| Name | Value | Token | Roles | Use |
| --- | --- | --- | --- | --- |
| Clear blue | `#2597d0` | `--color-accent` | accent, text | Small symbols, waveform details and savings text; not the primary button color. |

### Neutral

| Name | Value | Token | Roles | Use |
| --- | --- | --- | --- | --- |
| Near black | `#070709` | `--color-ink` | text, action | Primary text and primary action fill. |
| Headline charcoal | `#151515` | `--color-heading-ink` | text | Default section-heading color. |
| Cool gray | `#60606c` | `--color-body` | text, link | Paragraphs, secondary labels and footer links. |
| Footer gray | `#868c98` | `--color-muted` | text | Small footer provenance and copyright lines. |
| Soft edge | `#f4f4f4` | `--color-edge` | border | Faint outline around supporting feature cards. |
| Feature gray | `#f5f5f5` | `--color-panel` | surface, border | Large product panels, segmented controls and testimonial hairlines. |
| Porcelain | `#fafafa` | `--color-soft-panel` | surface | Small supporting cards and the broad testimonial backing. |
| White | `#ffffff` | `--color-canvas` | background, surface, text | Page canvas, floating cards and text over sky. |

### Page-type variants

| Only for | Name | Value | Token | Roles | Use |
| --- | --- | --- | --- | --- | --- |
| pricing modules | Ice blue | `#f5fcff` | `--color-savings-wash` | surface | Tiny savings capsule. |
| testimonial sections | Pencil gray | `#bec2ca` | `--color-signature` | text | Handwritten testimonial sign-offs. |

## Typography

- **Open Runde** — Marketing headings, paragraphs and action labels; Regular, Medium, Semibold and Bold cuts belong to the same family. Rounded contemporary sans with friendly terminals and compact, closely tracked display settings. If unavailable, use **Nunito Sans**. Use 400–700 and preserve the tight display tracking. Font stack: "Open Runde", "Nunito Sans", sans-serif.
- **Inter** — Small footer metadata and selected navigation links. Neutral, compact interface sans. Font stack: "Inter", sans-serif.
- **The Doctor FreeVersion** (only for testimonial signatures and handwriting demonstrations) — Personal sign-offs and the unprocessed side of transformation illustrations. Thin, slanted, loosely connected handwriting. If unavailable, use **La Belle Aurore**. Keep the signature light and low contrast. Font stack: "The Doctor FreeVersion", "La Belle Aurore", cursive.

| Recipe | Font | Weight | Size | Line height | Tracking | Use |
| --- | --- | --- | --- | --- | --- | --- |
| display | Open Runde | 600 | 80px | 0.9 | -0.04em | White centered opening and sky-band titles. |
| heading | Open Runde | 600 | 44px | 1.1 | -0.04em | Centered section leads and closing promise; also the visual scale of plan prices. |
| card-heading | Open Runde | 500 | 28px | 1.2 | -0.03em | Large feature-panel titles, usually two lines and left aligned. |
| support-heading | Open Runde | 600 | 20px | 1.4 | -0.01em | Short headings on the smaller benefit cards. |
| body | Open Runde | 400 | 18px | 1.4 | -0.01em | Main supporting copy, with semibold inline phrases carrying the benefit. |
| action | Open Runde | 600 | 17px | 1.4 | -0.01em | Primary and secondary action labels. |
| detail | Open Runde | 400 | 16px | 1.4 | -0.01em | Testimonial paragraphs and pricing inclusions. |
| footer-link | Open Runde | 500 | 14px | 1.5 | -0.01em | Compact footer navigation. |
| metadata | Inter | 500 | 14px | 1.5 | -0.01em | Muted footer location and credit lines. |

### Page-type variants

| Only for | Recipe | Font | Weight | Size | Line height | Tracking | Use |
| --- | --- | --- | --- | --- | --- | --- | --- |
| testimonial sections | signature | The Doctor FreeVersion | 400 | 38px | 0.9 | -0.01em | Low-contrast handwritten sign-off at the bottom right of a quote. |

**Notes:**

- The display and section headings share -0.04em tracking despite their different sizes. Card headings loosen to -0.03em; body and small text use -0.01em.
- Semibold is a visual 600 even when provided by a separately named font cut. Keep support copy regular with only short benefit phrases emphasized.
- Headings use sentence case, not uppercase editorial labels. Tiny uppercase timing labels belong inside product demonstrations, not the marketing hierarchy.

## Layout

**Density:** Airy: wide sectional pauses frame relatively compact paragraphs and small actions.

### Spacing

| Value | Use |
| --- | --- |
| 8px | Action icon gap and compact control spacing. |
| 12px | White inset around sky sections and compact content gaps. |
| 16px | Supporting-card heading to body and footer group separation. |
| 20px | Feature badge-to-title and plan content grouping. |
| 28px | Opening headline, support and action separation. |
| 36px | Desktop feature-grid gutters. |
| 40px | Feature-card padding and major internal groups. |
| 52px | Default heading-to-feature-grid gap and content side padding. |
| 100px | Typical content-section top and bottom padding; footer top padding. |
| 120px | Sky-stage top padding and conversion-island vertical padding. |
| 152px | Larger content-section lead-in and lower breathing room. |
| 200px | Isolated typographic interlude top padding. |

### Containers and grids

- **sky-stage**: max width 1440px · side padding 12px. Nearly full-width atmospheric stage, leaving a thin white perimeter.
- **content**: max width 1440px · side padding 52px. Centered desktop content, about 1336px available for feature grids.
- **paired-features**: 2 columns · gap 36px. Equal 650px feature panels spanning the content width.
- **benefits**: 3 columns · gap 36px. Supporting cards about 421px wide beneath feature panels.
- **footer-columns**: 4 columns · gap 80px · side padding 56px. Navigation occupies the right half; a small wordmark anchors the otherwise open left half.

## Corner radius

| Element | Radius |
| --- | --- |
| sky-opening | 48px |
| feature-panels | 48px |
| testimonial-cards | 40px |
| plan-cards | 32px |
| floating-ui | 18px |
| buttons | 100px |
| portrait | 50% |

## Surfaces and depth

### Shadows

| Only for | Name | Value | Use |
| --- | --- | --- | --- |
|  | dark-action | `0px 1px 2px rgba(36,36,40,0.1), 0px 3px 3px rgba(36,36,40,0.09), 0px 6px 4px rgba(36,36,40,0.05), 0px 11px 4px rgba(36,36,40,0.01), 0px 17px 5px rgba(36,36,40,0)` | Subtle grounded depth under the black pill. |
|  | quote-float | `0px 17px 37px rgba(16,55,132,0.03), 0px 67px 67px rgba(16,55,132,0.03), 0px 150px 90px rgba(16,55,132,0.02)` | Very broad cool haze beneath testimonial cards. |
| pricing modules | raised-plan | `0px 0.4px 0.4px rgba(22,106,196,0.01), 0px 1.6px 1.6px rgba(22,106,196,0.04), 0px 7px 7px rgba(22,106,196,0.17)` | Cool blue contact shadow under the featured plan. |

### Surfaces

#### Canvas · level 0

**Use:** Default marketing background.

**CSS:** `background: #ffffff`

#### Sky stage · level 0

**Use:** Opening and atmospheric conversion moments.

**CSS:** `background: linear-gradient(#779bc1 0%, #9abfda 58%, #cbdfec 100%); border-radius: 28px 28px 48px 48px; overflow: hidden`

**Observed:** The opening has smaller top corners; later sky islands use 48px on every corner.

**Transfer:** Reserve this colored environment for a few expansive focal moments.

#### Feature panel · level 1

**Use:** Large capability demonstrations.

**CSS:** `background: #f5f5f5; border-radius: 48px; padding: 40px; overflow: hidden`

**Observed:** Flat backing supports much smaller floating white interface objects, not edge-to-edge app views.

**Transfer:** Keep a neutral stage around each explanatory vignette.

#### Porcelain panel · level 1

**Use:** Supporting benefits and broad social-proof backing.

**CSS:** `background: #fafafa; border: 0.8px solid #f4f4f4; border-radius: 48px`

#### Quote paper · level 2

**Use:** Personal customer proof.

**CSS:** `background: #ffffff; border: 1px solid #f5f5f5; border-radius: 40px; box-shadow: 0px 17px 37px rgba(16,55,132,0.03), 0px 67px 67px rgba(16,55,132,0.03), 0px 150px 90px rgba(16,55,132,0.02)`

#### Floating navigation · level 3

**Use:** Fixed top navigation.

**CSS:** `background: rgba(255,255,255,0.04); border-radius: 120px; backdrop-filter: blur(4.1px)`

**Observed:** It reads almost transparent over the sky and white over the content, with restrained shadowing.

**Transfer:** Keep the bar visually thin so it does not compete with the stage.

## Components

### Navigation

**Use:** Persistent site orientation.

**CSS:** `display: flex; justify-content: space-between; align-items: center; height: 64px; padding: 8px; border-radius: 120px; background: rgba(255,255,255,0.04); backdrop-filter: blur(4.1px)`

**Observed:** Small logo left; compact link group centered; login and a filled sign-up pill right. Links are light over sky and dark over white. The sign-up pill is white on sky and dark over content.

### Primary button

**Use:** One clearly dominant conversion action.

**CSS:** `display: flex; align-items: center; justify-content: center; gap: 8px; background: #070709; color: #ffffff; border-radius: 100px; padding: 12px 24px; height: 48px; box-shadow: 0px 1px 2px rgba(36,36,40,0.1), 0px 3px 3px rgba(36,36,40,0.09), 0px 6px 4px rgba(36,36,40,0.05), 0px 11px 4px rgba(36,36,40,0.01)`

**Text style:** `action` — Open Runde 600 · 17px/1.4 · tracking -0.01em

**Observed:** Content-width in the hero and closing call; almost full card width in the promoted plan.

### Secondary button

**Use:** Product-detail navigation inside neutral panels.

**CSS:** `display: flex; align-items: center; gap: 8px; background: #ffffff; color: #070709; border-radius: 100px; padding: 12px 14px 12px 24px; height: 48px`

**Text style:** `action` — Open Runde 600 · 17px/1.4 · tracking -0.01em

**Observed:** A short label precedes a 20px right chevron. It sits at the lower left of its panel. Low-emphasis pricing actions instead use the pale gray fill.

### Feature card

**Use:** A large capability with its own miniature product scene.

**CSS:** `background: #f5f5f5; border-radius: 48px; padding: 40px; display: flex; flex-direction: column; justify-content: space-between; overflow: hidden`

**Text style:** `card-heading` — Open Runde 500 · 28px/1.2 · tracking -0.03em

**Observed:** Small white icon badge at top, title next, isolated interface vignette in the middle, supporting copy or Secondary button near the bottom.

### Benefit card

**Use:** A concise supporting advantage or assurance.

**CSS:** `background: #fafafa; border: 0.8px solid #f4f4f4; border-radius: 48px; padding: 40px; display: flex; flex-direction: column; justify-content: space-between`

**Text style:** `support-heading` — Open Runde 600 · 20px/1.4 · tracking -0.01em

**Observed:** A small icon above a short title and one paragraph; typically grouped in threes. Blue icons sit in white circular carriers for assurance content.

### Testimonial card

**Use:** Human proof with a personal sign-off.

**CSS:** `background: #ffffff; border: 1px solid #f5f5f5; border-radius: 40px; padding: 100px 40px 40px; display: flex; flex-direction: column; gap: 52px`

**Text style:** `detail` — Open Runde 400 · 16px/1.4 · tracking -0.01em

**Observed:** A 120px circular portrait overlaps the top edge. Several short quote paragraphs emphasize selected clauses in darker bold text. Name and role sit low left; a pale handwritten signature sits low right. Paired cards share carousel arrows beneath.

**Transfer:** Use authentic portraits and varied paragraph lengths rather than star ratings.

### Plan card

**Use:** Choose between tiers.

**CSS:** `background: #ffffff; border-radius: 32px; padding: 24px; display: flex; flex-direction: column; gap: 20px`

**Text style:** `detail` — Open Runde 400 · 16px/1.4 · tracking -0.01em

**Observed:** Tier label, 44px price, audience line, checkmarked inclusion list and bottom action. The promoted middle card rises above its neighbors to fit a billing selector, uses a blue contact shadow, a black full-width button and tiny reassurance below. The entry tier has a pale gray button; the flexible tier is deliberately simpler.

### Segmented selector

**Use:** Switch between demonstrations or billing periods.

**CSS:** `display: flex; align-items: center; justify-content: center; gap: 4px; padding: 4px; background: #f5f5f5; border-radius: 40px; backdrop-filter: blur(6px)`

**Text style:** `action` — Open Runde 600 · 17px/1.4 · tracking -0.01em

**Observed:** Two compact options in a low gray track; the selected option becomes a white pill. Demonstration version is 292px wide and 56px tall; billing version is 298px wide and 48px tall.

### Footer link

**Use:** Compact grouped navigation at the end of every page.

**CSS:** `color: #60606c; font-size: 14px; line-height: 21px; letter-spacing: -0.1px`

**Text style:** `footer-link` — Open Runde 500 · 14px/1.5 · tracking -0.01em

**Observed:** Simple text links beneath darker group titles; rows have 12px gaps. No button containers or icon decoration.

**States:** Declared: hover color #070709 and underline; focus-visible unknown.

## Imagery and graphics

### White workflow sculpture

**Use:** Signature opening artwork beneath the main promise.

**Observed:** A white open envelope holds handwritten and typeset documents with small before/after pills. More white document frames fan outward behind it. It is softly lit, mostly matte, with faint blue shadows and almost no hard contour; its lower part is clipped by the sky stage. Sparse pale specks give the blue field depth.

**Transfer:** Translate the transformation into an object suited to the new product. The minimum version is a layered white output card emerging from a simple folded container, not a giant flat dashboard.

**Build:** Use SVG polygons for an open container: pale white rear diamond, two overlapping white front triangles and a slightly darker bottom face. Place two rounded white document cards behind the front flap, one with loose gray strokes and one with short typeset lines. Add 3–5 rounded outline cards rotated outward behind it; use rgba(119,155,193,0.15) soft shadows. Place sparse 1–3px white dots at low opacity across the sky, keeping the copy area clear.

### Floating interface vignettes

**Use:** Explain capabilities within Feature cards and isolated white interludes.

**Observed:** Upload tiles, tiny document sheets, recording timers, waveforms and chat bubbles float in generous empty space. White cards have soft blue-gray contact shadows, occasional shallow perspective and pale bottom fades. Small cyan-blue details provide the only saturation; central objects remain readable while peripheral versions blur or fade.

**Transfer:** Render only the minimum interface needed to demonstrate an input, transformation and output. Keep it physically smaller than the panel and subordinate to the headline.

**Build:** Stack 2–3 white rounded rectangles with 10–18px corners; add a short title, muted lines and one #2597d0 functional detail. Use a linear mask or a panel-colored transparent-to-opaque gradient at the bottom. Offset secondary cards behind the main card and blur only those secondary layers.

### Small dimensional word tiles

**Use:** Signature punctuation embedded into selected section headings.

**Observed:** Small white square icon tiles about 48px across sit inside heading phrases, with pale cyan symbols and a little cool shadow, behaving like tangible objects among words.

**Transfer:** Use a simple domain-relevant symbol in a raised white tile; include this device in selected headings, not every line.

**Build:** Create a 48px white rounded square with a 7px corner radius, a 20px pale blue-gray glyph and a 0px 7px 7px rgba(22,106,196,0.1) shadow. Align it optically with the 44px heading and allow surrounding words to wrap naturally.

### Product ensemble

**Use:** The closing product-confidence scene.

**Observed:** A phone, a larger laptop-like interface and a tablet float side by side on white. Pale frames, nearly front-facing screens and soft shadows make the center device dominant without a dark hardware bezel.

**Transfer:** Show actual product surfaces across relevant formats. If the product has one format, use a central output view with two smaller complementary interface views; preserve the pale floating ensemble.

### Portraits and personal signatures

**Use:** Human proof and team-workflow illustrations.

**Observed:** Natural color headshots sit in circular masks, not full-bleed lifestyle photographs. Pale script signatures and small identity cards provide a personal counterpoint to clean interface geometry.

**Transfer:** Use ordinary, credible customer portraits with neutral lighting; reserve handwriting for a real personal attribution.

### Sky clouds

**Only for:** pricing modules

**Use:** Atmosphere behind white plan cards.

**Observed:** Soft naturalistic white clouds enter from the left and right, leaving the central heading and promoted plan clear. Blue deepens at the top and becomes pale toward the lower corners.

**Transfer:** Keep pricing a buoyant island rather than a spreadsheet. Clouds should frame the cards, never obscure text.

**Build:** Layer the Sky stage gradient behind two off-center cloud clusters. Each cluster combines overlapping white ellipses with irregular edges, rgba(255,255,255,0.4) wisps and 12–30px blur. Put the denser cloud masses beside the cards at mid-height; keep the central column unobstructed.

### Trust object

**Only for:** assurance sections

**Use:** One larger physical metaphor beneath assurance cards.

**Observed:** A silver shackle and glossy black circular lock body float over white with a broad diffuse shadow. The dark object is a rare strong visual counterweight to the otherwise white artwork.

**Transfer:** Use a single comprehensible protective or reliability metaphor, with one dark polished face and restrained silver depth.

**Build:** Use a thick gray SVG arch behind a near-black circular body; layer translucent radial highlights, a thin lighter rim and a white rounded symbol plate. Add a broad cool shadow beneath rather than a hard drop shadow.

### Icons

**Observed:** Small marketing symbols are mostly 20px, with some 32px standalone marks. Blue outline symbols around 1.9px stroke appear within white carriers; chevrons and utility symbols are compact and often solid. Raised white icon tiles also punctuate section headings.

**Transfer:** Choose simple rounded utility symbols, generally monochrome or clear blue. Do not turn the icon system into multicolor illustrations.

## Section recipes

How recurring sections are built.

### First screen: Sky transformation opening

**Observed:** A thin 12px white frame surrounds a 1416px-wide, 876px-tall Sky stage at desktop. Navigation floats across its top. A centered white two-line display headline occupies about 568px width in the upper third, starting after 120px of stage padding. A roughly 388px-wide support paragraph follows with 28px separation, then a Primary button after another 28px. The lower half opens into air before the White workflow sculpture rises from the bottom, with its main container about 660px wide and its wider fan reaching across most of the stage. Behind-to-front layers are blue gradient, sparse specks, rear object frames, main sculpture and small label pills, with copy kept unobstructed above. Within the first 900px the complete promise, support, action and upper sculpture are visible; the sculpture is intentionally clipped at the rounded bottom, and the next section begins below.

**Transfer:** Create a short outcome-versus-friction promise and stage a white transformation object below it. Without bespoke 3D art, build the layered-card sculpture described in imagery. Feature-specific pages can use a shorter 450px title-and-subtitle sky band with no opening sculpture; pricing pages open directly with the sky-backed plan comparison.

**Avoid:** Do not substitute a left-text/right-dashboard split, fill the entire stage with a screenshot, or place the headline across the sculpture.

**Text style:** `display` — Open Runde 600 · 80px/0.9 · tracking -0.04em

### Paired capability chapter

**Observed:** A centered heading, sometimes interrupted by a Small dimensional word tile, leads into two Feature cards after a 52px gap. Panels use the paired-features grid. A second row can introduce three Benefit cards beneath, with 36px gutters and clear hierarchy between demonstration and supporting detail.

**Transfer:** Group related capabilities into two distinct outcome stories; let the smaller cards answer follow-up questions rather than repeat panel headings.

**Text style:** `heading` — Open Runde 600 · 44px/1.1 · tracking -0.04em

### Isolated product interlude

**Observed:** A compact centered 44px heading and an 18px support line sit above a small floating interface/object composition. Top padding reaches 200px, bottom padding 152px; body text highlights one benefit in darker semibold. Artwork dissolves gently into white.

**Transfer:** Use an interlude to make one important product quality memorable between denser chapters.

**Text style:** `heading` — Open Runde 600 · 44px/1.1 · tracking -0.04em

### Demonstration stage

**Observed:** A centered heading with an inline word tile sits above the Segmented selector and a large landscape demonstration frame. The landscape frame is narrower than the feature grid; a product-specific version is 963px wide with 12px corners and a diffuse cool shadow beneath.

**Transfer:** Use working video, animation or an actual product walkthrough inside the frame; keep the surrounding composition white and restrained.

### Numbered workflow rail

**Observed:** Tall rounded cards sit on a horizontal rail extending toward the right. Numbers are small white circular or rounded carriers near the upper left. The first card is sky blue with white copy and a floating identity card; subsequent cards are white with dark copy, orbital portraits and small tooltip-like panels. Titles are 28px.

**Transfer:** Use this scoped treatment for a multi-person or multi-step workflow, preserving one colored anchor and lighter adjacent steps.

### Personal proof stage

**Observed:** The Porcelain panel forms a broad 48px-corner backing. A centered heading with a dimensional tile sits over paired Testimonial cards and a faint oversized circular line. Portraits overlap the cards; understated circular arrows sit beneath.

**Transfer:** Use fewer, substantial testimonials with selective emphasis and real attribution instead of a dense logo wall.

**Text style:** `heading` — Open Runde 600 · 44px/1.1 · tracking -0.04em

### Sky plan island

**Observed:** Sky stage becomes an all-48px-corner island with 120px vertical padding, an 80px white title and three white Plan cards. Clouds frame the comparison; the central plan is taller and starts above its neighbors. In a dedicated pricing opening, cards are about 346px wide with 36px gaps; the same module recurs later in other page types.

**Transfer:** Present a clear entry, recommended and flexible tier. Keep the center emphasis structural and shadow-based rather than adding a loud banner.

**Text style:** `display` — Open Runde 600 · 80px/0.9 · tracking -0.04em

### Product-confidence close and footer

**Observed:** The long landing-page close returns to white: centered 44px two-line promise, 18px supporting paragraph, dark Primary button and a wide pale Product ensemble beneath. The footer then uses 100px top and 56px bottom padding, with logo left, four compact navigation columns right, and muted metadata along the bottom. Feature-focused pages can end at the plan island before this footer; pricing-focused pages end after personal proof rather than adding another conversion banner.

**Transfer:** Choose the appropriate final reassurance for the page purpose. Preserve the generous white footer and its asymmetrical distribution rather than forcing every page to repeat the same final CTA.

**Text style:** `heading` — Open Runde 600 · 44px/1.1 · tracking -0.04em

## Page flow

**Storyline:** Promise → tangible product proof → capability chapters → human and operational reassurance → commercial choice → product confidence and navigation.

### Broad product landing page

1. **Promise** — Sky transformation opening with white sculpture and one conversion action.
2. **Product demonstration** — Paired capability overview, followed by a tabbed landscape walkthrough.
3. **Capability chapters** — Large paired feature panels, smaller benefit rows and isolated typographic/product interludes.
4. **Workflow expansion** — Numbered horizontal rail adds multi-person use.
5. **Social proof** — Personal proof stage with portraits and handwritten sign-offs.
6. **Objection handling** — Three assurance cards and a substantial protective object.
7. **Pricing** — Cloud-backed comparison island.
8. **Closing call** — Product-confidence close with device ensemble, then white navigation footer.

**Transfer:** Adapt the length to the product. Retain the alternation between physical metaphors, real interface detail and human reassurance rather than repeating one card grid.

### Focused capability landing page

1. **Promise** — Short sky title band with a single white title and supporting line.
2. **Product demonstration** — Wide neutral feature panel combines an outcome claim, small action, floating timing cards and conversation fragments; three smaller benefit cards follow.
3. **Capability reinforcement** — Centered typographic interlude with a tiny functional interface.
4. **Education** — Centered heading and landscape walkthrough frame.
5. **Pricing** — Shared sky plan island is the final conversion section.
6. **Ending** — White grouped navigation footer immediately follows.

**Transfer:** Shorten the opening and concentrate on one capability; let the shared pricing island carry conversion without adding the device close.

### Commercial comparison page

1. **Pricing** — Sky comparison island opens immediately under navigation.
2. **Value reinforcement** — Centered benefit heading and paired capability cards.
3. **Social proof** — Personal proof stage with two substantial quotes and carousel controls.
4. **Ending** — White grouped footer follows the proof stage, without another CTA section.

**Transfer:** Lead with the decision, then justify the value through product and customer proof.

## Writing

Warmly practical and confident, with a little aspirational lift. The product promises relief from routine work, then explains the concrete mechanism in ordinary language.

**Do not copy:** Do not reuse the Letters name, logo, medical examples, customer names, testimonials, savings claims, accuracy or speed figures, pricing, geographic assurances or compliance claims. Replace them with substantiated facts about the new product. The examples below show the pattern only; write new copy for the new product.

- **Addressing the reader:** Address the reader as you and your; use we for the product team when explaining what happens behind the scenes.
- **Rhythm:** Short outcome-led headlines, often split across two lines. Support text is usually one to three compact sentences, with a selected benefit phrase in semibold; actions are brief verbs.

| Role | Pattern | Typical length | Examples of the pattern |
| --- | --- | --- | --- |
| Opening promise | Contrast the work the reader values with the friction removed. | 3–6 words | “Patients, not paperwork” |
| Section lead | Name a practical outcome, sometimes with the product name. | 4–9 words | “Save hours a week with [Brand]”<br>“Your data is safe” |
| Capability title | Direct verb plus useful output or improvement. | 5–10 words | “Generate personalised letters that sound like you”<br>“Upload any source to create your letter” |
| Support copy | Explain the mechanism, then state the benefit without technical ornament. | 1–3 sentences | “Refine your letter by requesting edits. You can save your edits, and we'll learn” |
| Primary action | Plain action verb with a concrete entry condition. | 3–5 words | “Sign up for free”<br>“Start 2-Week Trial” |

**Words and phrasing to use:** effortless; personalised; sound like you; seamlessly; save time; ready-to-use; get started; your team

**Avoid:** disruptive ecosystem; revolutionary paradigm; enterprise-grade synergy; technical superlatives without proof

**Rules:**

- Pair aspirational verbs with concrete capabilities, not abstract category language.
- Use selective inline emphasis to make the benefit readable at a glance.
- Describe price tiers by the reader's situation before listing inclusions.
- Write reassurance as direct statements and explain the reason immediately afterward.

## Do's and Don'ts

### Do

- Keep the opening title at 80px/0.9 with -0.04em tracking on desktop.
- Keep ordinary section leads at 44px/1.1 and subordinate feature titles at 28px/1.2.
- Use 48px panel corners with 40px padding, leaving space around the interface objects.
- Maintain the 12px white perimeter around expansive blue stages.
- Keep a 36px gutter between paired panels and between supporting benefit cards.
- Use small raised white tiles to punctuate selected heading phrases.
- Let the promoted plan rise above its neighbors while their bottoms remain aligned.
- Keep the footer's left half sparse and its right-side links compact at 14px.

### Don't

- Do not turn the powder-blue atmosphere into a dark navy technology theme.
- Do not color primary buttons blue; keep the 48px black lozenge as the dominant action.
- Do not use the 38px handwriting face for headlines, body copy or navigation.
- Do not replace the pale UI vignettes with full-bleed dark dashboards inside every panel.
- Do not apply the broad testimonial haze to every benefit card; most gray panels are flat.
- Do not use 8px card corners throughout; the large 48px silhouettes are central to the character.
- Do not add uppercase marketing eyebrows above every section; the small pills are icon-led product labels.
- Do not make the footer a dark closing band or stretch its link columns across the entire page.

## Motion and responsive

### Motion

**Observed:**

- A typewriter cursor is declared with a 1s ease infinite animation in interface demonstrations.
- Text links declare a near-black underlined hover treatment; no button or surface transitions are established.

**Transfer:**

- Use the typewriter detail only within a functional interface vignette; let the surrounding marketing composition remain visually legible at rest.

**Unknown:**

- Object-scene animation timing, scroll choreography and button transition curves are not established.

### Responsive

**Observed:**

- Width rules cluster around 810px, 1200px and 1440px.

**Transfer:**

- For narrower layouts, preserve the centered sky promise and white object below it, stack paired feature panels and keep their neutral backing.
- Reflow the footer links beneath the logo and make plan comparison readable without relying on the center card's vertical offset.

**Unknown:**

- Exact narrow-screen type sizes, spacing, navigation replacement and workflow-rail behavior are not established.

## How to use this guide

1. Start from the Essentials and the first-screen recipe; where the guide offers variants, use the default named for a new marketing page.
2. Plan the page before building: map your content onto the section recipes and page flow, then check the plan against the Do's and Don'ts.
3. Build with the tokens and component specs; recreate signature graphics with their build recipes instead of generic decoration, and use the named font substitutes if a font is unavailable.
4. Render the page at desktop and mobile widths, compare it with the Essentials and the Don'ts, and fix the differences before you finish.
