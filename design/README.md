# Design library

The owner's taste, written down so every project starts at expert level.

## Index

| File | Mood in one line | Best for |
|---|---|---|
| `styles/firm-foundations.md` | Cream paper, navy blocks, light italic serif, angled photo cuts | Wellness / lifestyle ebooks, guides, workbooks |
| `styles/vivid-prismatic.md` | Near-black, huge regular grotesk, glass sculpture, spectral halo | Agencies, expert services, manifesto-style brands |
| `styles/slash-serif-shadows.md` | Black stage, editorial serif w/ true italic, silver objects, warm grain horizon | Premium software / services, high-ticket offers |
| `styles/origin-nature.md` | Nature photography + light serif + dark product panels | Calm, personal, "complex made simple" products, coaching, apps |
| `styles/revolut-sculpted.md` | Sky-lit lifestyle photo, rounded medium grotesk, metallic product objects | Broad consumer launches, apps, memberships |
| `styles/hyer-altitude.md` | White editorial, monumental bold grotesk, terracotta + midnight fields | Premium personal services, travel, concierge, consulting |
| `styles/letters-cloudborne.md` | Powder-blue sky, rounded sans, white paper sculptures, 48px panels | Friendly productivity tools, templates, digital downloads |

## Full original specs

Where the owner supplied the complete guide, it is stored verbatim in
`styles/full/` and takes priority over the condensed file:

- `styles/full/letters-cloudborne.md`

## What every style in this library has in common (the "expert" layer)

These are the habits that separate these references from template-looking work.
Apply them regardless of style.

1. **One dominant idea per screen/page.** Each section has a single promise, set
   very large, and everything else is clearly subordinate. Never two competing
   headlines.
2. **Hierarchy by scale, not weight soup.** Most display type is weight 300–500.
   The jump between headline and body is dramatic (often 4–8×). Body copy stays
   modest (16–20px web, 10–12pt print).
3. **Tight display tracking, relaxed body.** Big type gets negative tracking
   (-0.01 to -0.04em) and line-height ≈ 0.9–1.15. Body gets 1.35–1.6.
   (Exception: high-contrast serifs like Slash keep +0.01em.)
4. **A restrained palette with one "event" colour.** 1 canvas + 1 ink +
   2–4 greys do 90% of the work. Saturated colour lives in imagery or one
   concentrated field — never sprinkled across buttons and icons.
5. **A signature graphic device, repeated.** Glass sculpture, light seam,
   angled photo cut, dashed journey path, white paper object, warm grain band…
   Each brand has 1–2 and repeats them at the opening and the close.
6. **Small, quiet actions.** Buttons are 40–48px high, short literal labels.
   The size of the *promise* creates urgency, not the size of the button.
7. **Separation by space and hairlines, not boxes and shadows.** Long 1px rules,
   generous section padding (100–224px web), flat panels. Shadows are rare and
   very soft.
8. **Deliberate asymmetry.** Offset support copy, empty half-columns, objects
   clipped by the edge. Centered-everything is a choice, not a default.
9. **Real imagery or built geometry — never generic stock filler.** If there's
   no photo, construct the signature object in SVG/CSS.
10. **The ending is designed.** Every page closes with a monumental invitation
    plus a calm, structured footer — not a stray button.
11. **Copy cadence matches the look.** Short headline → one concrete sentence →
    literal action. No hype words, no exclamation marks.

## Method (use on every project)

1. **Brief → style.** Pick the style file(s). Note the audience and the one
   promise.
2. **Map content to section recipes** from the style file's *Page flow*. Write
   the outline before any code.
3. **Set tokens first** (colours, type recipes, spacing, radii) as CSS custom
   properties, copied from the style file.
4. **Build the signature device** using the file's *Build* recipe.
5. **Build sections**, then **render** (Playwright screenshots at 1440px and
   390px; every page for print).
6. **Audit** against the file's Essentials + Don'ts and the 11 principles
   above. Fix, re-render, then deliver.

## Mixing styles

Allowed when intentional: take *structure* from one (e.g. Hyer's page flow) and
*material* from another (e.g. Firm Foundations palette). Never mix two display
typefaces from different files, and keep a single signature device family.

## Adding new inspiration

When the owner shares a new reference (screenshot, URL, spec), create
`styles/<name>.md` with the sections: Mood · Essentials · Tokens (colour, type,
spacing, radius) · Signature devices (+ build) · Section recipes · Page flow ·
Writing · Do / Don't · Ebook translation. Then add it to the index above.
