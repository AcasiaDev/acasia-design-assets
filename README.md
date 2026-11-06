# Acasia design assets

CDN-servable brand assets for the `acasia-design` skill, so any coded project can use the real
assets without uploading files. Serve through jsDelivr:

```
https://cdn.jsdelivr.net/gh/AcasiaDev/acasia-design-assets@main/<path>
```

jsDelivr caches `@main`. To force a refresh after an update, pin a commit SHA instead of `@main`.

## Current: Design System 7.2, `v7.2/`

Source of truth is the Figma file `M5nTaYA0GvMptOZoH3NnTT` (Acasia Design System 7.2), asset pack
checked 2026-11-04. If a file here disagrees with Figma, Figma wins and this mirror needs updating.

| Path | What |
|---|---|
| `v7.2/acasia-7.2.css` | Tokens (Dark default via `class="dark"`, Light), fonts, motion, text style classes |
| `v7.2/logo/` | `acasia-logo-white.png` (Dark grounds, photos) and `acasia-logo-green.png` (Light grounds), 960 × 320 |
| `v7.2/icons/line/` | 35 line icons, SVG in `currentColor` |
| `v7.2/icons/utility/` | 28 utility icons for controls, SVG in `currentColor` |
| `v7.2/avatars/` | 8 placeholders and system avatars, 492 × 492 |
| `v7.2/photos/` | 6 approved facility photos (graded) and 4 AI concepts (always labeled AI concept) |

```css
@import url('https://cdn.jsdelivr.net/gh/AcasiaDev/acasia-design-assets@main/v7.2/acasia-7.2.css');
```

### Not here, on purpose

Team portraits are photos of named employees and stay out of this public repo. Lockups,
illustrations, campus views and campaign art are not hosted either. Report a missing asset; never
redraw or substitute one.

## Retired: Design System 4.0, root folders

`tokens-4.0.css`, `logo/`, `icons/`, `exports/` and `fonts/` are the 4.0 mirror (Figma
`Z9xIuFkgAB2N5W4hKUzxAz`). They stay so older projects keep loading. Do not use them for new work.
