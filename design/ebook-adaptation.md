# Translating the web styles into ebooks & digital products

Web specs are written for a 1440px viewport. Ebooks are fixed pages. Use this
to convert any style in `styles/` to print/PDF/Canva.

## Page formats

| Product | Size | Canvas px (for HTML→PDF / Canva) |
|---|---|---|
| Standard ebook / guide | 6 × 9 in | 576 × 864 CSS px |
| Workbook / printable | US Letter 8.5 × 11 in (or A4) | 816 × 1056 |
| Lead magnet / social-first guide | 1080 × 1350 (4:5) | 1080 × 1350 |
| Slide-style ebook | 1920 × 1080 | 1920 × 1080 |

Margins: 0.6–0.75 in outer, 0.75–0.9 in on the binding side for print.

## Type scale conversion (6 × 9 in page)

| Web role | Web size | Ebook size |
|---|---|---|
| Display / opening | 80–136px | 54–76px (chapter openers only) |
| Statement / chapter | 52–105px | 40–56px |
| Heading | 44–64px | 28–36px |
| Lead | 20–34px | 15–17px |
| Body | 16–20px | 12–13.5px (≈ 10–11pt) |
| Labels / eyebrows | 11–16px | 8.5–10.5px, tracked +0.2–0.35em |

Keep the *ratios and tracking* from the style file; only the absolute numbers
shrink.

## Page types every ebook needs (map them to the style's recipes)

1. **Cover** → the style's first-screen recipe (promise + signature device).
2. **Contents / What you'll learn** → service module, ruled benefit list, or
   icon rows.
3. **Chapter opener** → statement recipe, lots of empty space, one image or
   device.
4. **Content spread** → body text in a narrow measure (55–70 characters),
   pull-quote or offset lead on the side.
5. **Quote / pause page** → full-bleed dark or atmospheric field, one sentence.
6. **Worksheet / action page** → hairline-ruled fields, numbered steps, no boxes
   or shadows.
7. **Closing / next step** → the style's closing recipe (monumental invitation +
   compact contact line).

## Canva workflow (works best for the owner)

- Build pages as HTML with real fonts, render to PDF via Playwright with
  embedded static fonts (not variable fonts — Canva turns those into outlines).
- Photo areas: a flat placeholder rectangle with the angled/cut shapes layered
  ABOVE it, so a photo can be dropped in and sent to back.
- Keep shapes as separate SVG elements so they stay editable after import.
- Use Canva-available fonts or their named substitutes (DM Sans, Inter,
  Cormorant Garamond, Bodoni Moda, Montserrat, Nunito Sans).
- A Canva connector may be available in sessions; if so, designs can be
  created/imported directly instead of via PDF.
