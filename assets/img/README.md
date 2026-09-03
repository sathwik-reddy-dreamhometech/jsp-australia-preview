# Brand assets

Only `logo.svg` is present, and it is a **placeholder**. Everything below is
collected in Phase 0 (PLAN.md §10) and dropped in here.

> 🛑 **Before any of this ships:** written permission from Janasena to
> use the party name, logo and flag on an Australian domain, plus a clear
> statement of whether this site is the official Australia chapter or an
> independent supporters' group. That statement goes in Settings → affiliation
> note, and appears in the footer and on the About page.

## Required files

| File | Size | Used by | Notes |
|---|---|---|---|
| `logo.svg` | ~360×88 | masthead | Official horizontal lockup on a dark ground. Keep the viewBox so the header does not reflow. |
| `logo-dark.svg` | ~360×88 | print / light backgrounds | Optional. |
| `favicon.png` | 512×512 | browser tab, admin | Square. Referenced by `templates/header.php`. |
| `og-banner.jpg` | 1200×630 | link previews | The default share image when a page has no cover. |
| `leader.jpg` | 400×400 | homepage leader strip | Square, face centred. Referenced by `index.php`. |
| `flag.svg` | any | section dividers | Optional; the CSS draws the stripe itself. |

## Ideal icons

`ideals.icon` in the database stores a filename that resolves to
`assets/img/ideals/<file>`. Seven simple line icons, one per ideal:

| # | Ideal | Seeded filename |
|---|---|---|
| 01 | Social consciousness without caste | `scales.svg` |
| 02 | Politics without religious discrimination | `hands.svg` |
| 03 | Reverence for linguistic diversity | `script.svg` |
| 04 | Protection of traditions and culture | `temple.svg` |
| 05 | Nationalism that does not forget regionalism | `map.svg` |
| 06 | Fight against corruption and atrocities | `shield.svg` |
| 07 | Protection of the environment | `leaf.svg` |

Draw them on a common grid (24×24, 2px stroke, `currentColor`) so they sit
consistently in the black ideals band. The pages render fine without them —
the numerals carry the design.

## Image guidance

- Photographs: export at 1600px on the long edge. The upload pipeline
  re-encodes and resizes anyway, but starting large keeps quality.
- The upload pipeline strips EXIF, which removes camera GPS data. That is
  deliberate: event photos should not carry the location of the people in them.
- Event photos with identifiable people — children especially — need a
  consent process and a takedown contact before publishing. PLAN.md §9.
