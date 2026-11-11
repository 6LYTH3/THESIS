# SPCX — segment FCFF valuation audit

**Last updated:** 2026-11-11
**Units:** USD billions, shares billions; reference $143.09 close November 10, not live.
**Sources:** [README.md](README.md), especially Q3 10-Q, earnings release, official webcast, October financing 8-K. All projections below are analyst assumptions.

## Contract and share-count checks

- Space revenue excludes internal launches; satellite launch costs capitalized in Connectivity PP&E. Never add a notional internal-launch revenue multiple to this valuation.
- Cloud contracts typically three years, terminable by either party with 90 days' notice. Reserved compute monthly revenue is not hardware-sale revenue or guaranteed SaaS ARR.
- Current basic shares October 15: 8.246541218 A + 5.334522491 B = 13.581063709. Weighted-average Q3 diluted 12.475 is not current diluted capitalization.
- Model denominator 14.0 = current basic + .2618 EchoStar contractual future shares + .157136291 cushion. Not a complete options/RSU treasury-stock audit; acquisition awards subject to service/forfeiture complicate exact counts. Do not describe 14B as company-disclosed fully diluted shares.
- Margins include cash-equivalent recurring SBC/retention cost. No SBC addback or buyback accretion. Dilution cushion addresses starting capitalization uncertainty, not a forecast of every future award; no further dilution is imposed for the same SBC already expensed.

## Timing, formula and tax

Ten prospective rolling 12-month periods from valuation date; year-end discounting. Year 1 $140B total revenue is a run-rate-informed analyst path, not FY2027 guidance. Base R0 = Connectivity 21, Space 7, SI 72, total 100, informed by management's end-2026 annualized December target. Not an actual historical revenue/OWC balance.

```text
Revenue[j,t] = baseRevenue[j,t] × revenueScale
Margin[j,t] = baseMargin[j,t] + marginShift
NetInvestment[j,t] = Revenue[j,t] × netInvestmentRatio[j,t] × investmentFactor
DeltaOtherOWC[j,t] = 0.03 × (Revenue[j,t] − Revenue[j,t−1])
FCFF[j,t] = Revenue[j,t] × Margin[j,t] × 0.79
            − NetInvestment[j,t] − DeltaOtherOWC[j,t]

Revenue[j,11] = Revenue[j,10] × (1 + g)
TerminalFCFF[j] uses year-10 margin, investment ratio, factors
EV[j] = sum(FCFF[j,t] / (1+WACC)^t)
        + TerminalFCFF[j] / (WACC−g) / (1+WACC)^10
Equity = sum(EV[j]) + 33.153
Value/share = Equity / 14.0
```

Normalize tax at 21%, with immediate consolidated benefit on segment losses as an approximation to tax sharing/loss carryforwards. Actual realization may be delayed; no extra deferred-tax asset added. WACC 11.5% is a judgmental required return, not a measured current beta/cost of capital. Single group WACC simplifies correlated segment/financing risks; a precision SOTP would require separate discount curves.

## Complete base input paths

Order: Connectivity, Space, SI. All ten entries correspond to years 1–10.

| Input | Connectivity | Space | SI |
| --- | --- | --- | --- |
| Revenue | 28,36,45,55,66,78,91,105,120,136 | 8,10,12,15,18,22,26,30,35,40 | 104,150,205,270,340,415,490,560,630,700 |
| EBIT margins | .38,.38,.38,.38,.38,.38,.38,.38,.38,.38 | −.10,0,.05,.10,.15,.18,.20,.22,.24,.25 | .08,.12,.16,.20,.23,.25,.27,.28,.29,.30 |
| Net investment / revenue | .20,.16,.13,.11,.09,.08,.07,.065,.06,.055 | .45,.35,.25,.20,.16,.13,.10,.08,.07,.06 | .65,.40,.28,.20,.16,.13,.11,.10,.09,.08 |

Net investment is **economic capex minus D&A**, not capex. It includes cash and financed equipment additions and replacement of short-lived satellites/GPU infrastructure. For an explicit gross-capex cross-check assume economic D&A/revenue 20% Connectivity, 12% Space, 30% SI; gross capex = these D&A amounts + net investment. These D&A rates are model assumptions, not disclosed useful lives. They imply year-one D&A $37.76B and gross economic capex $114.56B, including, not in addition to, ~$40B anticipated lease equipment. Year-ten D&A $242B and gross capex $307.88B. No assumption that GPU maintenance capex disappears.

Declining net investment ratios create operating leverage but still imply high mature incremental ROIC. At g=3.5%, terminal net investment + other OWC / NOPAT is about 31%, implying incremental ROIC ~11%; this is group-level and not full return-on-historical-capital measurement. Different asset lives/replacement costs can materially change cash generation.

## Base annual consolidated schedule

| Year | Revenue | EBIT after SBC | Net investment | Delta OWC | FCFF |
| --- | ---: | ---: | ---: | ---: | ---: |
| 1 | 140 | 18.160 | 76.800 | 1.200 | −63.6536 |
| 2 | 196 | 31.680 | 69.260 | 1.680 | −45.9128 |
| 3 | 262 | 50.500 | 66.250 | 1.980 | −28.3350 |
| 4 | 340 | 76.400 | 63.050 | 2.340 | −5.0340 |
| 5 | 424 | 105.980 | 63.220 | 2.520 | 17.9842 |
| 6 | 515 | 137.350 | 63.050 | 2.730 | 42.7265 |
| 7 | 607 | 172.080 | 62.870 | 2.760 | 70.3132 |
| 8 | 695 | 203.300 | 65.225 | 2.640 | 92.7420 |
| 9 | 785 | 236.700 | 66.350 | 2.700 | 117.9430 |
| 10 | 876 | 271.680 | 65.880 | 2.730 | 146.0172 |

Year-10 D&A cross-check: .20×136 + .12×40 + .30×700 = **242.0**. Terminal year revenue 906.66, EBIT 281.1888, NOPAT 222.139152, net investment 68.1858, OWC .9198, terminal FCFF **153.033552**. Net reinvestment plus OWC / NOPAT ~31.11%, g/reinvestment ~11.25% implied incremental ROIC. These accounting/economic assumptions are approximations, not a vintage-by-vintage GPU model.

| Operating value | PV years 1–10 | PV terminal | EV |
| --- | ---: | ---: | ---: |
| Connectivity | 76.185187 | 144.664004 | 220.849191 |
| Space | −5.100300 | 23.781991 | 18.681691 |
| SI | 8.953617 | 475.646142 | 484.599759 |
| Total | 80.038504 | 644.092138 | 724.130642 |

Equity 757.283642 /14 = **$54.091689**. Terminal PV/EV **88.95%**. This terminal dependence is a core risk, not a confidence signal.

## Non-operating bridge

```text
Cash and cash equivalents              51.294
Marketable securities                 38.561
Existing debt/finance lease principal −38.989
EchoStar cash/debt settlement reserve   −8.500
Remaining expected trust payments      −1.213
Grain provisional spectrum reserve     −8.000
Adjusted bridge                       +33.153
```

- Debt principal differs from $38.844B carrying value by $0.145B issuance costs. Use one consistent basis.
- Restricted cash excluded. Digital assets/TBC/equity investments not separately valued; upside there is not required for thesis. Goodwill $48.423B is not added to EV.
- EchoStar fixed equity issuance is handled in denominator, not by also subtracting $11.1B cash. At $143.09 the shares' market value differs materially from the contractual fixed-value label.
- Trust expected future payments .385 remaining 2026 + .828 in 2027 = 1.213. Additional payments if closing delayed to 2028 are not in base: contingent downside.
- Grain $8B is a provisional reserve based on secondary reporting, not independently verified acquisition accounting. $1B bridge change affects value by ~$0.0714/share. No double addition of acquired spectrum value on top of operating growth it enables.
- Reserves undiscounted for simplicity, mildly conservative to future cash timing. General ongoing spectrum/PP&E replacement investment must remain in net investment assumptions; deal reserves represent the identified one-off transactions.
- Operating lease expenses remain in EBIT; operating lease debt is not separately capitalized. All existing finance leases/debt are in bridge.

## Financing consistency and funding gap

October 24 conditional Apollo financing ~$40B, commencement expected H1 2027, is not September debt. When new equipment is obtained, include its full economic investment irrespective of whether cash initially leaves the company. This model includes it within year-one gross economic capex; do not add $40B capex again or subtract $40B debt at valuation date without the matching funding inflow.

Future debt principal payments are financing, not FCFF expenses. Interest is reflected through WACC rather than deducted again from NOPAT. Existing debt is subtracted once. Negative FCFF already reduces EV; net new borrowing to fund it is not a second deduction today. This assumes financing on fair terms with viable access; it does **not** prove sufficient liquidity.

Base undiscounted negative FCFF years 1–4 totals **$142.9354B**. Even liquidity before existing debt repayment/deal reserves $89.855B is lower. Additional financing, customer advances, slower investment or better operating performance is required. The $40B equipment commitment can cover part of needs but is conditional and creates future payments; it is not $40B unrestricted cash. A separate quarterly cash/lease amortization and covenant model would be necessary to assess solvency under detailed scenarios. Distressed funding or equity issuance below intrinsic value can impair common equity beyond this DCF.

## Scenarios: transforms of all base paths

| Scenario | Revenue and R0 scale | Parallel EBIT margin shift | Net investment factor | WACC | g | Value/share |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Bear | .65 | −.07 | 1.15 | .14 | .025 | 7.038487 |
| Base | 1 | 0 | 1 | .115 | .035 | 54.091689 |
| Bull | 1.6 | +.06 | .85 | .10 | .04 | 186.949904 |

Tax/OWC/bridge/shares unchanged. Terminal uses same scenario factors. Factors applied to **net** investment; do not claim a 15% cut in gross capex. Bear still assumes long-run recovery and financing access; not a liquidation floor. Bull year-ten revenue $1,401.6B and EBIT $518.784B is a very demanding success outcome. Uniform margin/revenue shifts simplify segment correlations, not independent bottom-up scenarios.

| Scenario | EV | Equity | Terminal share of EV |
| --- | ---: | ---: | ---: |
| Bear | 65.385815 | 98.538815 | 214.6% |
| Base | 724.130642 | 757.283642 | 88.9% |
| Bull | 2,584.145655 | 2,617.298655 | 82.4% |

Bear terminal >100% because explicit cash flows have negative PV, not a calculation error. No statistical probabilities or expected-value average are assigned.

## WACC / g sensitivity (base operations)

| WACC / g | 2.5% | 3.5% | 4.5% |
| --- | ---: | ---: | ---: |
| 10% | 65.28 | 74.38 | 86.78 |
| 11.5% | 48.65 | 54.09 | 61.08 |
| 13% | 37.24 | 40.72 | 45.01 |

4.5% perpetuity growth is an upper stress sensitivity, not a conservative anchor. All cells assume terminal capex/replacement as modeled; no exit multiple is layered on top.

## Reverse valuation

Revenue-only scaling is linear because R0, EBIT and investment/OWC scale together. With EV_base 724.130642 and fixed bridge 33.153:

`scale_required = (143.09 × 14 − 33.153) / 724.130642 ≈ 2.72x`

Year-ten revenue ~**$2.38T** at unchanged margins/investment ratios/WACC/g. Not a prediction of actual investor expectations; many combinations of higher margins, lower capital costs and different growth timing can support the same price. Using 14.5B shares changes base value to ~$52.23, highlighting denominator uncertainty.

## Reported cash / EBITDA audit

- 9M2026 simple CFO−PP&E = 13.097−48.069 = **−34.972B**.
- Alternative investing-cash adjustment: +1.372 rebates −.020 capitalized interest −.866 intangible payments = **−34.486B**. Not full company-defined FCF or economic FCFF; financed additions/SBC differ.
- Q3 adjusted EBITDA 8.809 is not FCFF: SI 4.953 includes addback of D&A 2.473, SBC .821 and acquisition SBC 1.217 from EBIT .431, plus small other items. Replacements and compensation are economic costs.
- Q3 EBIT 2.791 + interest income .873 − interest expense .675 + other income 1.025 + tax benefit .390 = net income 4.404. Includes unrealized TBC gain .561 and acquisition-related provisional deferred tax benefit .449, neither recurring operating cash.
- Historical comparable tables are as presented following common-control combination; do not relabel 2025 figures as standalone pre-xAI SpaceX. Cursor instead contributes only after August 14, 2026.

## Model limitations

No full prospectus/cap-table audit, detailed debt covenants, title-by-title contract economics, satellite/GPU vintage schedule, fair-value option valuation or explicit Tesla combination model. Forecast tax sharing, D&A percentages and working capital are simplifying assumptions. Strong terminal dependence, external financing needs and uncertain SI margins justify very high uncertainty; scenario outputs are illustrations, not precise price targets.
