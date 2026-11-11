# NFLX — DCF assumptions and calculation audit

**Last updated:** 2026-11-11
**Currency/units:** USD billions; shares in billions; per-share values post 10-for-1 split.
**Reference price:** $63.26, November 10, 2026 regular-session close, not live.
**Source mapping:** See [README.md](README.md), especially primary FY2025 10-K, Q3 2026 10-Q and Q1/Q3 shareholder letters.

## Timing and valuation conventions

- Ten prospective rolling 12-month years from November 11, 2026, approximately Nov 2026–Nov 2036, not literal FY2026–35. End-year discounting t=1..10; no already-earned 2026 fee/FCF included as future cash flow.
- R0 $51.1B is an analyst transition revenue baseline informed by FY2026 company guidance; it is not a full starting operating-working-capital balance.
- Operating margin includes content amortization and SBC economic expense. Do not add SBC back. Constant diluted share denominator 4.2B approximates Q3 diluted 4.195B; no forecast buyback accretion added to FCF value. Treat SBC as a cash-equivalent cost rather than additionally projecting future dilution for the same awards.
- Normalized cash tax 18% of EBIT. Company actual cash tax, share-comp tax benefits, FX and discrete items can differ.
- Physical/non-content D&A 0.8% of revenue; physical capex 1.8%. Net physical reinvestment 1% revenue. Base forecast excludes a recurring special real-estate acquisition but retains ongoing physical investment.
- Content amortization modeled separately as a share of revenue; cash content payments = amortization × cash-spend ratio. Net excess content investment = cash payments − amortization, not total cash content spend subtracted a second time from EBIT.
- Other operating working capital consumes 3% of incremental revenue. Content liabilities/payments already captured in content cash ratio; do not include them again in other OWC.
- Net debt bridge uses company Q3 non-GAAP reconciliation consistently: carrying debt $15.132394B + issuance/discount costs $0.059251B + fair-value hedge adjustment $0.145158B = gross debt $15.336803B; less unrestricted cash $8.194275B and short-term investments $0.028678B = **$7.113850B**. Bridge date September 30, 2026, not November live balance sheet.
- Restricted cash is not added. WBD termination cash already flowed into reported liquidity/capital allocation; no separate $2.8B non-operating asset added. No WBD acquired assets, merger debt or synergies: that agreement terminated in February.
- Content obligations $25.2228B are not subtracted from EV as additional debt in full because ongoing cash content payments, including funding those obligations, are already modeled. This does not eliminate liquidity risk. Unknown future-title commitments may exceed disclosed minimums.
- Operating leases remain in EBIT and are not additionally debt-capitalized. No deferred-tax asset or content library premium added on top of operating value. Unrestricted cash includes some required operating liquidity, potentially making equity value mildly favorable.
- Base WACC 9.5% is a judgment: illustrative equity cost 9.8% (4% risk-free + 1.16 beta × 5% ERP), debt cost 5.25% before tax, and ~5.6% debt capital weight approximate a 9.5% WACC. These are assumptions, not verified current market inputs.

## Formulae

```text
EBIT_t = Revenue_t × EBIT_margin_t
NOPAT_t = EBIT_t × 0.82
ContentAmort_t = Revenue_t × ContentAmort_share_t
CashContent_t = ContentAmort_t × CashContent_ratio
NetContentInvestment_t = (CashContent_ratio − 1) × ContentAmort_t
Physical_D&A_t = 0.008 × Revenue_t
Physical_capex_t = 0.018 × Revenue_t
DeltaOtherOWC_t = 0.03 × (Revenue_t − Revenue_(t−1))
FCFF_t = NOPAT_t − 0.01 × Revenue_t
         − NetContentInvestment_t − DeltaOtherOWC_t
PV_explicit = sum(FCFF_t / (1 + WACC)^t), t=1..10

Revenue_11 = Revenue_10 × (1 + g)
EBIT_margin_11 = EBIT_margin_10
ContentAmort_share_11 = ContentAmort_share_10
FCFF_11 uses same formula and Revenue_10 as its prior revenue
PV_terminal = FCFF_11 / (WACC − g) / (1 + WACC)^10
EV = PV_explicit + PV_terminal
Equity = EV − 7.113850
Value_per_share = Equity / 4.2
```

Content amortization is not free cash flow. Adding it all back without cash content replenishment grossly overstates value. Company CFO−physical capex also includes financing cash costs and SBC addbacks, so it is not automatically FCFF.

## Base annual schedule

| Year | Revenue | EBIT margin | Content amortization / revenue | Content amortization | Net content investment @ 1.10x | Delta other OWC | FCFF | PV @ 9.5% |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| 1 | 57 | 33% | 33.0% | 18.810 | 1.8810 | 0.177 | 12.7962 | 11.6860 |
| 2 | 63 | 34% | 32.5% | 20.475 | 2.0475 | 0.180 | 14.7069 | 12.2657 |
| 3 | 69 | 35% | 32.0% | 22.080 | 2.2080 | 0.180 | 16.7250 | 12.7387 |
| 4 | 75 | 36% | 31.5% | 23.625 | 2.3625 | 0.180 | 18.8475 | 13.1098 |
| 5 | 81 | 37% | 31.0% | 25.110 | 2.5110 | 0.180 | 21.0744 | 13.3870 |
| 6 | 87 | 37.5% | 30.5% | 26.535 | 2.6535 | 0.180 | 23.0490 | 13.3711 |
| 7 | 93 | 38% | 30.0% | 27.900 | 2.7900 | 0.180 | 25.0788 | 13.2864 |
| 8 | 99 | 38% | 29.5% | 29.205 | 2.9205 | 0.180 | 26.7579 | 12.9461 |
| 9 | 105 | 38% | 29.0% | 30.450 | 3.0450 | 0.180 | 28.4430 | 12.5675 |
| 10 | 111 | 38% | 28.5% | 31.635 | 3.1635 | 0.180 | 30.1341 | 12.1595 |

Base illustrative ads path: $4.0, $5.5, $7.0, $8.5, $10.0, $11.5, $13.0, $14.5, $16.0, $17.5B. Subscription/other revenue = total minus ads. Ads are not added again to total revenue. This is a mix plausibility check, not a disclosed segment forecast or subscriber-level model; identical total revenue/margins produce identical FCFF irrespective of labels.

Base terminal g 3.0%; revenue_11 $114.33B; FCFF_11 $31.123623B. PV explicit $127.517932B, PV terminal $193.212668B, EV $320.730600B, equity $313.616750B, per share **$74.670655** → research fair value **~$75**. Terminal PV = 60.24% of EV.

Terminal net reinvestment = $1.1433B physical + $3.258405B content + $0.0999B other OWC = $4.501605B. NOPAT $35.625228B, reinvestment rate ~12.64%; g/reinvestment rate implies incremental ROIC ~23.74%. This is an enduring-moat assumption, not full fade to cost of capital. If competitive returns converge, valuation should fall.

## Complete scenario inputs

Tax, physical investment, other OWC, R0, shares and equity bridge unchanged across scenarios.

| Scenario | Total revenue, years 1–10 | EBIT margins, years 1–10 | Amortization share of revenue | Cash content ratio | WACC / g |
| --- | --- | --- | --- | ---: | --- |
| Bear | 54, 56, 58, 60, 62, 64, 66, 68, 70, 72 | 30%, 29%, 29%, 29%, 30%, 30%, 30%, 30%, 30%, 30% | 35% every year | 1.15x | 11% / 2% |
| Base | 57, 63, 69, 75, 81, 87, 93, 99, 105, 111 | 33%, 34%, 35%, 36%, 37%, 37.5%, 38%, 38%, 38%, 38% | 33%, 32.5%, 32%, 31.5%, 31%, 30.5%, 30%, 29.5%, 29%, 28.5% | 1.10x | 9.5% / 3% |
| Bull | 59, 67, 76, 86, 97, 108, 119, 130, 141, 152 | 34%, 36%, 38%, 40%, 41%, 42%, 42%, 42%, 42%, 42% | Same as base | 1.08x | 9% / 3.5% |

| Scenario | PV explicit | PV terminal | EV | Equity | Value/share | vs $63.26 |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Bear | 64.832639 | 52.565647 | 117.398286 | 110.284436 | $26.258199 | -58.49% |
| Base | 127.517932 | 193.212668 | 320.730600 | 313.616750 | $74.670655 | +18.04% |
| Bull | 179.542310 | 375.264477 | 554.806787 | 547.692937 | $130.403080 | +106.14% |

No probability weights, no statistical confidence claims. Bull requires strong global growth and exceptional content productivity; bear still assumes profitable survival.

## Sensitivity tables

Hold base operating forecast and content ratio unchanged:

| WACC / g | 2.5% | 3.0% | 3.5% |
| --- | ---: | ---: | ---: |
| 8.0% | $93.24 | $99.75 | $107.71 |
| 9.5% | $71.20 | $74.67 | $78.72 |
| 11.0% | $57.06 | $59.11 | $61.44 |

Hold base forecast, WACC 9.5%, g 3%, changing cash content ratio for all years including terminal:

| Cash content / amortization | Value/share |
| --- | ---: |
| 1.05x | $78.91 |
| 1.10x | $74.67 |
| 1.15x | $70.43 |
| 1.20x | $66.19 |

The ratio test isolates investment/cash timing with EBIT unchanged; real content inflation can hurt both cash ratio and margin. The combined effect can be much worse.

## Reverse DCF at $63.26

Target equity at diluted 4.2B shares = $265.692B; plus net debt $7.113850B gives EV $272.805850B. (This is intentionally different from spot market cap using basic outstanding shares.) One-variable solutions relative to base:

- Revenue/R0 scale **0.850576x**: year 1 ~$48.48B, year 10 ~$94.41B. An algebraic sensitivity, not a forecast consistent with current near-term guidance.
- Parallel EBIT margin shift **−4.83276 percentage points**: year 1 28.17%, terminal 33.17%.
- WACC **10.53493%**, retaining g 3%.
- Cash content/amortization ratio **1.234523x** every year including terminal, keeping EBIT/margins otherwise unchanged.

Markets can reflect infinitely many combined solutions. This analysis does not identify actual investor expectations or prove mispricing.

## Reported vs recurring cash: reconciliation cautions

- FY2025 audited FCF = $10.149273B CFO − $0.688220B physical capex = $9.461053B.
- 9M2026 FCF = $10.196296B − $0.693540B = $9.502756B.
- TTM FCF = $9.461053B − $7.588746B 9M2025 + $9.502756B 9M2026 = $11.375063B. Includes termination fee and discrete tax effects.
- FY2026 FCF guidance ~$12B includes the fee. Q1 letter explicitly says upward revision $11B→$12.5B primarily reflects after-tax fee impact; Q3 $12.5B→$12B is primarily real-estate transaction closing.
- Illustrative normalization only: $12B − $2.8B × 82% + $0.729B Brazil cash payment + $0.5B property timing proxy = $10.933B. Fee tax timing is not known precisely; the $0.5B forecast change does not prove transaction size. Not a company-adjusted metric, not direct FCFF and not a DCF anchor.
- FY2026 mechanical EPS ~9M $2.90 + Q4 forecast $0.67 = $3.57 includes fee and is not exact full-year weighted-share EPS. TTM $3.46 minus illustrative after-tax fee/4.2B gives ~$2.91 and P/E ~21.7x, not official adjusted earnings.

## Risks in this model

- Ten-year margin/ads/content productivity assumptions dominate a current-quarter beat. Base year-10 38% margin and $111B revenue are substantial achievements, not conservative certainties.
- Content amortization is management-estimated. Lower amortization/revenue and rising EBIT margin must be earned through pricing, scale and slate productivity, not arbitrary accounting changes.
- Content cash ratio, amortization, regulation and physical investment may differ by market, title mix or live rights. No proprietary title-by-title ROI model is available.
- Brazil tax and other disputes can recur elsewhere even if a specific charge is non-routine; ongoing taxes/levies are retained in operating economics rather than assuming all regulatory costs vanish.
- No future acquisition synergies, gaming standalone premium or formal peer valuation is added. A new large acquisition requires a new financing/operating model.
