# Thesis — Investment Research Workspace

This repository is a workspace for investment and business analysis. The agent
acts as an investment/business analyst: for every company researched, the work
product is a per-ticker folder containing the research summary.

## Repository structure

```
Thesis/
├── AGENTS.md          # this file — conventions for agents
├── INDEX.md           # catalog of all researched tickers (one row per folder)
└── <TICKER>/          # one folder per company, named by its primary stock symbol
    ├── README.md      # the research summary (see template below)
    └── ...            # optional supporting files (charts, data, notes)
```

Rules:
- Folder name is the primary listing symbol in UPPERCASE (e.g. `AAPL/`, `MSFT/`,
  `7203.T/` for non-US listings — use the common exchange suffix form).
- Every ticker folder MUST contain a `README.md` with the research summary.
- Keep `INDEX.md` updated: after creating or revising a ticker folder, add or
  update its row there.

## INDEX.md row format

Markdown table with columns: `Ticker | Company | Sector | Thesis (1 line) | Last updated`.
Sort alphabetically by ticker.

## README.md template

```markdown
# <TICKER> — <Company name>

**Sector:** <sector>
**Last updated:** <YYYY-MM-DD>

## Summary
(3–6 sentences: what the company does and the core investment thesis or concern)

## Business & Financials
- Key facts: revenue/earnings drivers, margins, growth, competitive position

## Bull case
- ...

## Bear case
- ...

## Valuation
(what the stock is priced at relative to fundamentals; key assumptions)

## Conclusion
(Clear view: attractive / neutral / avoid, with the main reason)

## Sources
- (URLs or references used for this research)
```

## Workflow for researching a company

1. If `<TICKER>/` does not exist, create it.
2. Research the company (public information, financials, news). Cite sources.
3. Write or update `<TICKER>/README.md` using the template.
4. Update `INDEX.md`.
5. Date every research pass with "Last updated" so freshness is visible.

## Conventions

- Summaries are opinionated: state a clear conclusion, not a neutral restatement
  of facts. The point of a "thesis" is to have a position.
- Use USD unless the company reports in another currency; note the currency used.
- Numbers should carry as-of dates (e.g. "FY2025 revenue $...").
- Keep files as plain Markdown; no build system, no code.
