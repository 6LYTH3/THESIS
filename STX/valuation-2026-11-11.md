# STX — DCF assumptions and calculation audit

**Last updated:** 2026-11-11
**Units:** USD billions except per-share figures; shares in billions.
**Purpose:** Reproducible independent valuation, not company guidance or Morningstar estimates.

## Timing and common conventions

- Ten prospective rolling 12-month model years from the valuation date, approximately November 2026–November 2036; not fiscal-year forecasts. Year-end cash-flow discounting, t = 1 through 10.
- Source financials and qualifications: see [README.md](README.md). No already-earned Q1 FY27 cash flow is inserted into prospective year 1.
- Model operating margins include an economic expense for SBC. Do not add SBC back to FCFF. Shares held constant at 0.233B, approximating Q2 guidance; no separate forecast buyback benefit or future SBC dilution on top of this SBC-as-cash-equivalent convention.
- Tax = 17%; D&A = 2% of revenue; capex = 5% of revenue in all three scenarios. Capex is within management's 4–6% framework, not guaranteed.
- Incremental operating working capital = 10% × change in annual revenue; starting revenue proxy R0 = $17.5B, an analyst transition baseline rather than historical audited revenue or a complete starting working-capital balance.
- WACC 10.5% base: illustrative risk-free 4% + beta 1.3 × ERP 5% ≈ 10.5% cost of equity; low market-value debt weight makes WACC close to equity cost. These are explicit assumptions, not verified current yields/beta. Sensitivity matters more than point precision.
- Balance-sheet bridge uses October 2, 2026 carrying debt $2.351B less unrestricted cash $1.258B = $1.093B. Deduct separately $0.105B BIS settlement payable, with no assumed future BIS cash outflow in FCFF. Total net claims = $1.198B.
- Restricted cash $0.112B is not added to equity. Of this $0.105B is litigation escrow; do not deduct that funded litigation amount a second time. Other operating accruals, warranties and purchase obligations are treated through operating margins/working capital/capex, not all classified as incremental debt.
- Ordinary operating lease costs remain in EBIT and are not capitalized as additional debt. No material unverified non-operating asset premium is added. Deferred tax assets are not separately added on top of normalized tax assumptions.
- Same-date bridge avoids combining October quarter-end cash with post-quarter debt. It is still a stale balance-sheet proxy for November valuation, not a precise live equity bridge.

## Formulae

```text
EBIT_t = revenue_t × operating_margin_t
NOPAT_t = EBIT_t × (1 − 0.17)
D&A_t = 0.02 × revenue_t
capex_t = 0.05 × revenue_t
delta_OWC_t = 0.10 × (revenue_t − revenue_(t−1))
FCFF_t = NOPAT_t + D&A_t − capex_t − delta_OWC_t
PV_explicit = sum(FCFF_t / (1 + WACC)^t), t = 1..10

revenue_11 = revenue_10 × (1 + terminal_g)
margin_11 = margin_10
FCFF_11 = revenue_11 × margin_10 × 0.83
          − 0.03 × revenue_11
          − 0.10 × (revenue_11 − revenue_10)
terminal_EV_10 = FCFF_11 / (WACC − terminal_g)
PV_terminal = terminal_EV_10 / (1 + WACC)^10
EV = PV_explicit + PV_terminal
equity = EV − 1.198
value_per_share = equity / 0.233
```

FCFF is before financing. Do not deduct interest from FCFF and then subtract debt again. Do not use company-reported CFO−capex directly as FCFF without financing/tax/SBC adjustments.

## Base operating schedule

| Model year | Revenue | EBIT margin | EBIT | Delta OWC | FCFF | PV at 10.5% |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| 1 | 19.000 | 48% | 9.120 | 0.150 | 6.8496 | 6.1987 |
| 2 | 21.000 | 47% | 9.870 | 0.200 | 7.3621 | 6.0294 |
| 3 | 22.500 | 45% | 10.125 | 0.150 | 7.5788 | 5.6171 |
| 4 | 24.000 | 43% | 10.320 | 0.150 | 7.6956 | 5.1617 |
| 5 | 25.200 | 42% | 10.584 | 0.120 | 7.9087 | 4.8006 |
| 6 | 26.200 | 41% | 10.742 | 0.100 | 8.0299 | 4.4110 |
| 7 | 27.300 | 40% | 10.920 | 0.110 | 8.1346 | 4.0439 |
| 8 | 28.400 | 39% | 11.076 | 0.110 | 8.2311 | 3.7030 |
| 9 | 29.500 | 38% | 11.210 | 0.110 | 8.3093 | 3.3830 |
| 10 | 30.500 | 37% | 11.285 | 0.100 | 8.3516 | 3.0771 |

Terminal g 2.5%; revenue_11 $31.2625B; FCFF_11 $8.586589B. PV explicit $46.425603B; PV terminal $39.546486B; EV $85.972089B; equity $84.774089B; value/share **$363.84**, rounded research fair value **$365**. Terminal value = 46.0% of EV.

Terminal net reinvestment = 3% × revenue_11 + incremental OWC ≈ $1.014125B. NOPAT_11 ≈ $9.600714B, reinvestment rate ≈ 10.56%; g / reinvestment rate implies incremental ROIC ≈ **23.7%**. This is a significant enduring moat assumption. The model fades margin but does not fully fade ROIC to WACC; if full competitive convergence occurs, reduce value.

## Scenario inputs — complete annual paths

All common conventions above remain fixed, including R0 $17.5B.

| Scenario | Revenue, years 1–10 | EBIT margins, years 1–10 | WACC | g |
| --- | --- | --- | ---: | ---: |
| Bear | 17, 16, 17, 18, 19, 20, 21, 22, 23, 24 | 40%, 30%, 30%, 31%, 32%, 32%, 32%, 32%, 32%, 32% | 12% | 2% |
| Base | 19, 21, 22.5, 24, 25.2, 26.2, 27.3, 28.4, 29.5, 30.5 | 48%, 47%, 45%, 43%, 42%, 41%, 40%, 39%, 38%, 37% | 10.5% | 2.5% |
| Bull | 21, 24, 27, 30, 33, 35, 37, 39, 41, 43 | 52%, 52%, 51%, 50%, 49%, 48%, 47%, 46%, 45%, 44% | 10% | 3% |

| Scenario | PV explicit | PV terminal | EV | Equity | Value/share |
| --- | ---: | ---: | ---: | ---: | ---: |
| Bear | 25.3891 | 18.4152 | 43.8043 | 42.6063 | $182.86 |
| Base | 46.4256 | 39.5465 | 85.9721 | 84.7741 | $363.84 |
| Bull | 69.6108 | 81.0578 | 150.6686 | 149.4706 | $641.50 |

No probability weighting. Scenario values are not statistical limits. Even bear assumes a profitable surviving HDD industry, not total technological obsolescence.

## Base forecast sensitivity

| WACC / g | 2.0% | 2.5% | 3.0% |
| --- | ---: | ---: | ---: |
| 9.0% | $429.62 | $447.43 | $468.20 |
| 10.5% | $353.35 | $363.84 | $375.72 |
| 12.0% | $299.90 | $306.52 | $313.87 |

## Reverse DCF at $501.62

Target equity at diluted 233M shares = $116.87746B; plus $1.198B net claims gives target EV **$118.07546B**. One-variable solutions, not forecasts:

- Multiply all base annual revenues AND R0 by approximately **1.3734** while preserving margin path, WACC and g: year 1 ≈ $26.09B, year 10 ≈ $41.89B. Scaling R0 is necessary to preserve the working-capital proportions in this algebraic sensitivity.
- Alternatively add approximately **13.32 percentage points** to every annual margin and the terminal margin: year 1 ≈ 61.32%, terminal ≈ 50.32%.
- Alternatively reduce WACC to approximately **8.29%**, holding the base operating forecast and g fixed.

There are infinitely many combined solutions. These examples expose expectations; they do not prove which assumptions investors actually hold.

## Main model risks

- Long-run margins are a judgment. Historical margins alone need not predict a structurally improved HDD market; conversely high latest margins need not persist.
- Net capex 3% of revenue plus working-capital investment may be insufficient if HAMR tooling/cycle times or competition require more capital. No plant-by-plant investment forecast is available.
- Base year 1 margin 48% is below near-term adjusted Q2 guidance but intentionally includes SBC economics and a cycle reserve. A detailed quarterly forecast could differ materially.
- Tax, OWC and SBC conventions simplify real cash timing. Unrestricted cash may include operating cash needs, so adding all of it is mildly favorable to equity value.
- Approximately $1B additional net claims would reduce fair value by $4.29/share, all else equal. Balance-sheet bridge uncertainty is much smaller than margin/duration uncertainty here.
