# CLAUDE.md

Design sources of CandleStack (STU FEI team project): self-contained HTML mockups in `mockups/`
and brand assets in `brand/`. Read the conventions in [README.md](README.md) first.

## Rules

- Everything in English: mockups, docs, commit messages, pull requests.
- Branch from `main` as `<area>/<topic>`; one small pull request per topic. Its title becomes
  the squash commit: imperative, sentence case, no trailing period.
- No AI attribution anywhere: no `Co-Authored-By` trailers of AI tools, no "Generated with ..."
  lines, no session links in commits or pull requests. The `no-ai-signs` check fails on them;
  `.claude/settings.json` already turns Claude Code's attribution off.
- A new mockup gets its row in the README's Mockups table.

## Verify

There is no build: open the changed HTML files in a browser at desktop and phone widths, in
both themes. CI runs only the `no-ai-signs` and `linked-issue` checks.
