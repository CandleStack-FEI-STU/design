# design

Design sources for [CandleStack](https://github.com/CandleStack-FEI-STU): UI mockups and brand assets.

## Mockups

| Mockup | Source | Ticket |
| --- | --- | --- |
| Ops status page (`ops.candlestack.tech`): the real page with example data built in; hover (or tap) a day for its outages, theme toggle, any width | [`mockups/ops/index.html`](mockups/ops/index.html) | [candlestack#8](https://github.com/CandleStack-FEI-STU/candlestack/issues/8), [ops#3](https://github.com/CandleStack-FEI-STU/ops/pull/3) |
| App instrument icons, approved "Final": 32 px icons with a 10 % radius in the list (41 px rows) and the header quick search (44 px rows), 64 px on the instrument page; the phone quick-search list with a 16 px gutter. Live list and search, theme toggle, any width; the notes at the bottom hold the numbers and the proposed `QuickSearch.tsx` classes | [`mockups/instrument-icons/index.html`](mockups/instrument-icons/index.html) | [candlestack#179](https://github.com/CandleStack-FEI-STU/candlestack/issues/179) |
| App instrument list filters, approved "N3": one fixed-width Filters button (34 × 200 px) whose panel holds Type and Exchange (All exchanges, the stock exchanges, then Binance); exchanges the chosen type does not have are disabled with the reason, and nothing in the row moves. Live list, URL and Back, keyboard, theme toggle, any width; the notes at the bottom hold the sizes, the rules and the backend change (`BINANCE`) | [`mockups/exchange-filter/index.html`](mockups/exchange-filter/index.html) | [candlestack#182](https://github.com/CandleStack-FEI-STU/candlestack/issues/182) |
| App instrument list stats, approved "Final": Price, 24h change, 10 daily mini candles (112 × 32 px) and 24h volume in the 41 px rows, sorted by volume; Type and Exchange stay plain columns; a Sort by section (Volume, Top gainers, Top losers, Symbol) in the Filters panel; on phones symbol over exchange and volume, 7 candles, price over change. Real Binance sample data for crypto, live list and sorts, URL and Back, theme toggle, any width; the notes at the bottom hold the sizes, formats and colors | [`mockups/instrument-list-stats/index.html`](mockups/instrument-list-stats/index.html) | [candlestack#184](https://github.com/CandleStack-FEI-STU/candlestack/issues/184) |
| App public home, approved: the Pipeline direction of the alpha directions. Header Product / Instruments / API with Sign in, Try Backtest (placeholders) and the theme toggle; headline, the five-block pipeline diagram with flowing dots, the three layer cards with badges, the five most traded instruments in the list's style, Compare and Public experiments as "Coming soon" cards. Instruments (`#/instruments`): the approved list with a solid table and a Data since column; rows open the instrument page (`#/instrument/AAPL`), whose back link returns to the home page or to the list with its filters. Background grid twice as strong as in the app, cards solid. Example data as in the list stats mockup; theme toggle, any width, and a Phone view button that shows the page in a 390 × 844 frame | [`mockups/home/index.html`](mockups/home/index.html) | [candlestack#199](https://github.com/CandleStack-FEI-STU/candlestack/issues/199) |
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
