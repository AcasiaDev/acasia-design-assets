# Acasia Design System 4.0 — public assets

CDN-servable brand assets for Acasia Design System 4.0. Referenced by absolute URL from the
`acasia-design` skill so any coded project can use the real masters without uploading files.

**Source of truth is the Figma file** `Z9xIuFkgAB2N5W4hKUzxAz` (Acasia Design System 4.0). This
repo is a mirror for code consumption. If a file here disagrees with Figma, Figma wins — and the
mirror needs updating.

## Use

Serve through jsDelivr, which is a real CDN and free for public repos:

```
https://cdn.jsdelivr.net/gh/AcasiaDev/acasia-design-assets@main/<path>
```

Example:

```html
<img src="https://cdn.jsdelivr.net/gh/AcasiaDev/acasia-design-assets@main/logo/acasia-logo-green.png"
     alt="Acasia" width="250" height="100">
```

```css
@import url('https://cdn.jsdelivr.net/gh/AcasiaDev/acasia-design-assets@main/tokens-4.0.css');
```

jsDelivr caches `@main` aggressively. To force a refresh after updating a file, pin a commit SHA
or tag instead of `@main`.

## Contents

| Path | What |
|---|---|
| `tokens-4.0.css` | Semantic token sheet. Token names match the live Figma variables. |
| `logo/` | Acasia lockup + mark (PNG, forest and white). Grove and Fabric lockups (SVG, true vector). |
| `icons/svg/` | 23 product icons, SVG — use these in code |
| `icons/` | The same 23 as PNG |
| `exports/` | `paper-grain.png` brand texture, 4 mineral slot shapes |
| `fonts/` | Geist, Geist Mono, Instrument Serif TTFs — for self-hosting or server-side rendering. Web projects should load these from Google Fonts instead. |

## Not here, deliberately

**Team avatars.** The 27 team portraits are photographs of named employees and are kept out of
this public repo. They live in the Figma file (`Avatar / Team Portrait / Green 500`) and in the
internal skill bundle. Upload them into a specific project when a build actually needs them.

## Rules

These are protected masters. Never redraw, trace, recolour, flatten, regenerate, or typeset them.

- The **Acasia lockup is a raster only** — a 1000 × 400 PNG. There is no vector Acasia wordmark
  anywhere; that is a known open gap. Scale it down, never up.
- The **Grove and Fabric lockups are true vector** SVG and scale freely.
- Product icons have two expressions: **Brand** mirrors the reference artwork, **Interface** keeps
  operational screens quiet. **Product UI uses Interface.** Icon tile ground is `#F6F4EF`.
- If an asset you need is not here, report the gap. Do not substitute a lookalike from an icon
  library and do not draw a replacement.
