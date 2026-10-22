# SeoulClinicIndex — Design Mockup v2

**Design mockup for review. Not the built site.** All clinic names, figures and copy on these screens are illustrative. No appointment, enquiry or payment can be made here.

## Screens

| File | Screen |
|---|---|
| `index.html` | 01 Home |
| `clinics.html` | 02 Clinic list |
| `clinic-detail.html` | 03 Clinic detail (fully verified) |
| `clinic-detail-minimal.html` | 04 Clinic detail (minimal, not indexed) |
| `neighborhood.html` | 05 Neighborhood guide |
| `procedure.html` | 06 Procedure page |
| `palette.html` | 07 Palette benchmark — six candidates, measured against nine comparable sites |

Open `index.html` for the entry screen, `palette.html` for the colour study.

## Palettes

`assets/base.css` holds the design tokens for the default palette. `assets/themes.css` holds five alternatives, applied by `<html data-theme="...">`. `assets/palette-switch.js` puts a switcher in the top nav so every screen can be flipped through in place; the choice is kept in `localStorage` and in the `?theme=` query parameter, so a specific palette can be linked directly.

| Key | Palette | Brand | Accent | Ground |
|---|---|---|---|---|
| A | Teal (previous default) | `#0E6B70` | `#0E6B70` | `#F2F5F4` |
| B | Navy & Brass | `#1B3557` | `#A8802F` | `#F4F3EF` |
| C | Crimson & Gold | `#8E1F32` | `#B08637` | `#F7F4F1` |
| D | Slate & Coral | `#2E4A63` | `#D2603F` | `#F4F4F2` |
| E | Aubergine & Sand | `#4A2F52` | `#C08A3E` | `#F6F3F1` |
| F | Ink & Gold | `#1A1F2E` | `#C9A962` | `#F2EEE6` |

**Recommendation: F · Ink & Gold.** `palette.html` carries the benchmark table it was chosen from, with the source of every hex value.

## Screenshots

`screenshots/` — 18 captures, 6 screens × desktop full / desktop fold / mobile 390px.

`screenshots/palettes/` — the six candidate palettes rendered on the home screen, the palette study page, and the full six-screen set in the recommended Ink & Gold palette.

## Notes

- Prices shown are illustrative, in the same shape the real site will use: a clinic's own published rate and its range, never a derived average or a total including travel and stay.
- Coverage is shown honestly on every screen: how many registry records exist, how many are live, and how many are fully verified.
- Where a clinic cannot yet take an enquiry, the button says "Ask about this area" instead of promising a direct line.
- The palette switcher is a review tool. The real site ships one fixed palette.
