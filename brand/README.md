# Brand

The CandleStack logo is the **tile**: two light candles cut out of a rounded teal square, picked
in [.github#2](https://github.com/CandleStack-FEI-STU/.github/issues/2). The other concepts stay
in [`logo-concepts/`](logo-concepts/) for reference.

## Files

| File | Use |
| --- | --- |
| [`logo.svg`](logo.svg) | Tile and the name, switches to the dark colors with `prefers-color-scheme` |
| [`logo-light.svg`](logo-light.svg), [`logo-dark.svg`](logo-dark.svg) | The same with fixed colors, for a known light or dark background (GitHub profile, slides, docs) |
| [`icon.svg`](icon.svg) | The tile alone, square, for favicons; switches theme like `logo.svg` |
| [`icon-light.svg`](icon-light.svg), [`icon-dark.svg`](icon-dark.svg) | The tile with fixed colors |
| [`favicon.ico`](favicon.ico) | 16 and 32 px, for browsers that do not take SVG favicons |
| [`icon-16.png`](icon-16.png), [`icon-32.png`](icon-32.png), [`icon-192.png`](icon-192.png), [`icon-512.png`](icon-512.png) | PNG exports of `icon-light.svg` (web app manifest, places without SVG) |
| [`apple-touch-icon.png`](apple-touch-icon.png) | 180 px, square corners: iOS rounds them itself |

A favicon in HTML:

```html
<link rel="icon" href="/favicon.ico" sizes="32x32">
<link rel="icon" href="/icon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
```

## Colors

The colors are the website tokens from
[`global.css`](https://github.com/CandleStack-FEI-STU/website/blob/main/src/styles/global.css):

| Part | Light | Dark |
| --- | --- | --- |
| Tile (`--accent`) | `#0f766e` | `#3cc7a6` |
| Candles (`--bg`) | `#fafaf9` | `#0d0f11` |
| Name (`--ink`) | `#141414` | `#ecedee` |

## Font

The name is Geist SemiBold (600) with letter spacing -0.025em, like the website header,
converted to outlines so the SVG needs no font. Geist is under the SIL Open Font License.

## Rules

- The tile is drawn on a 32 px grid with whole-pixel candles, so it stays sharp at 16 and
  32 px. Scale it in whole multiples where you can.
- Keep a clear space of at least a quarter of the tile height around the logo.
- Do not recolor, stretch, rotate or add effects; for another background pick the light or
  dark variant.
