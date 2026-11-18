# Media sources for Reels and video edits

Owner's standing instruction: use these sources whenever a Reel / short-form
edit needs audio or B-roll. Reels are commercial content (fitness business),
so every file must be licensed for commercial use AND modification.

## Audio — Openverse

- API: `https://api.openverse.org/v1/` (audio endpoint: `/v1/audio/`)
- Search with commercial-safe filters:
  `https://api.openverse.org/v1/audio/?q=<mood or genre>&license_type=commercial,modification&page_size=20`
  - Useful extra params: `category=music` (or `sound_effect`), `length=short`
    (under 30s, good for SFX), `extension=mp3`.
- Allowed licences: **CC0, PDM (public domain), CC BY, CC BY-SA**.
  Reject **NC** (non-commercial) and **ND** (no derivatives — cutting/looping
  counts as modifying).
- Read each result's `license`, `license_version`, `attribution`,
  `foreign_landing_url` and `url` (download). Prefer CC0/PDM: no credit needed.

## B-roll — Internet Archive "movies" collection

- Collection: `https://archive.org/details/movies`
- Search (public-domain / CC only):
  `https://archive.org/advancedsearch.php?q=collection:movies AND (<keywords>) AND (licenseurl:*publicdomain* OR licenseurl:*creativecommons*)&fl[]=identifier&fl[]=title&fl[]=licenseurl&rows=25&output=json`
- File list for an item: `https://archive.org/metadata/<identifier>` →
  download from `https://archive.org/download/<identifier>/<file name>`
  (prefer `.mp4` / `h.264` derivatives).
- Many uploads in this collection have **no licence or are someone else's
  copyrighted footage**. Use only items whose `licenseurl` is public domain
  (CC0 / publicdomain/mark) or a commercial+modification CC licence. No
  `licenseurl` = don't use it.
- Old public-domain footage is often 4:3, low-res and black & white: crop to
  9:16, grade it, and use it as texture/cutaways, not as the main shot.

## Every time media is used

1. Download into a new folder per project; keep the source page URL.
2. Add a row to that project's `CREDITS.md`:
   `title — creator — licence — source URL`.
3. For CC BY / BY-SA, give the owner the attribution line to paste into the
   Reel caption.
4. Never use a file whose licence can't be confirmed; say so and pick another.
