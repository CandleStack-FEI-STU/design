# design

Design sources for [CandleStack](https://github.com/CandleStack-FEI-STU): UI mockups and brand assets.

## Mockups

| Mockup | Source | Ticket |
| --- | --- | --- |
| Ops status page (`ops.candlestack.tech`) | [`mockups/ops/index.html`](mockups/ops/index.html) | [candlestack#8](https://github.com/CandleStack-FEI-STU/candlestack/issues/8) |

## Layout

| Path | Contents |
| --- | --- |
| `mockups/<name>/index.html` | One mockup per folder, a single self-contained HTML file |
| `brand/` | Logo sources and exports (see [.github#2](https://github.com/CandleStack-FEI-STU/.github/issues/2)) |

## Conventions

- Mockups follow the website style: Geist and Geist Mono, color tokens from
  [`website/src/styles/global.css`](https://github.com/CandleStack-FEI-STU/website/blob/main/src/styles/global.css).
- Every mockup works on desktop and on a phone (from 360 px), in light and dark theme.
- Mockups use example data only. No real hostnames of internal services, credentials or personal data.
- Changes go through a pull request, like in the other repositories.
