# design

Design sources for [CandleStack](https://github.com/CandleStack-FEI-STU): UI mockups and brand assets.

## Mockups

| Mockup | Source | Ticket |
| --- | --- | --- |
| Ops status page (`ops.candlestack.tech`): the real page with example data built in; hover (or tap) a day for its outages, theme toggle, any width | [`mockups/ops/index.html`](mockups/ops/index.html) | [candlestack#8](https://github.com/CandleStack-FEI-STU/candlestack/issues/8), [ops#3](https://github.com/CandleStack-FEI-STU/ops/pull/3) |
| App instrument icons, approved "Final": 32 px icons with a 10 % radius in the list (41 px rows) and the header quick search (44 px rows), 64 px on the instrument page; the phone quick-search list with a 16 px gutter. Live list and search, theme toggle, any width; the notes at the bottom hold the numbers and the proposed `QuickSearch.tsx` classes | [`mockups/instrument-icons/index.html`](mockups/instrument-icons/index.html) | [candlestack#179](https://github.com/CandleStack-FEI-STU/candlestack/issues/179) |
| Website home: Links section (groups side by side; on phones two links per line), light and dark | [`mockups/website/links/`](mockups/website/links/) | [website#15](https://github.com/CandleStack-FEI-STU/website/pull/15), [website#16](https://github.com/CandleStack-FEI-STU/website/pull/16) |
| Website, desktop: Home, Meetings, Meeting, Status, Team in light and dark (the approved concept) | [`mockups/website/desktop/`](mockups/website/desktop/) | |
| Website, mobile "Terminal" variant (rejected: mobile must look like desktop) | [`mockups/website/mobile-terminal-rejected/`](mockups/website/mobile-terminal-rejected/) | |

To view a mockup, download the HTML file and open it in a browser.

## Layout

| Path | Contents |
| --- | --- |
| `mockups/<name>/` | One folder per mockup, self-contained HTML files |
| `brand/` | Dark logo and dark icon (see [.github#2](https://github.com/CandleStack-FEI-STU/.github/issues/2)) |

## Conventions

- Mockups follow the website style: Geist and Geist Mono, color tokens from
  [`website/src/styles/global.css`](https://github.com/CandleStack-FEI-STU/website/blob/main/src/styles/global.css).
- New mockups cover desktop and phone widths (from 360 px) and both light and dark theme.
- Mockups use example data or public facts only: no credentials or personal data.
- Changes go through a pull request, like in the other repositories. The pre-commit hooks
  (`.pre-commit-config.yaml`: whitespace, secrets, typos, Markdown, workflows, comments) run in
  CI; install them once per clone with `uvx pre-commit install`.
