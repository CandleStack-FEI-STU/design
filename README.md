# design

Design sources for [CandleStack](https://github.com/CandleStack-FEI-STU): UI mockups and brand assets.

## Mockups

| Mockup | Source | Ticket |
| --- | --- | --- |
| Ops status page (`ops.candlestack.tech`) | [`mockups/ops/index.html`](mockups/ops/index.html) | [candlestack#8](https://github.com/CandleStack-FEI-STU/candlestack/issues/8) |
| Website home: Links section (groups side by side; on phones two links per line), light and dark | [`mockups/website/links/`](mockups/website/links/) | [website#15](https://github.com/CandleStack-FEI-STU/website/pull/15) |
| Website, desktop: Home, Meetings, Meeting, Status, Team in light and dark (the approved concept) | [`mockups/website/desktop/`](mockups/website/desktop/) | |
| Website, mobile "Terminal" variant (rejected: mobile must look like desktop) | [`mockups/website/mobile-terminal-rejected/`](mockups/website/mobile-terminal-rejected/) | |

To view a mockup, download the HTML file and open it in a browser.

## Layout

| Path | Contents |
| --- | --- |
| `mockups/<name>/` | One folder per mockup, self-contained HTML files |
| `brand/` | Logo sources and exports (see [.github#2](https://github.com/CandleStack-FEI-STU/.github/issues/2)) |

## Conventions

- Mockups follow the website style: Geist and Geist Mono, color tokens from
  [`website/src/styles/global.css`](https://github.com/CandleStack-FEI-STU/website/blob/main/src/styles/global.css).
- New mockups cover desktop and phone widths (from 360 px) and both light and dark theme.
- Mockups use example data or public facts only: no credentials or personal data.
- Changes go through a pull request, like in the other repositories.
