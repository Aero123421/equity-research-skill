# Coverage map

Use this file to make sure the research looked in every direction that could
change the conclusion. It has four parts:

1. Minimum check per lens
2. Mandatory lenses by request type
3. Contradiction patterns (the best leads)
4. Prioritizing leads and stopping

---

## 1. Minimum check per lens

"Minimum check" = the least you must establish before marking a lens ✅.
If you cannot establish it, mark ⚠️ or ❌ and say why.

| Lens | Minimum check | Typical deeper work |
|---|---|---|
| L1 Business | Revenue by segment/region, what drives profit, top customers/suppliers if disclosed, main competitors | Unit economics, market share trend, pricing power, switching costs, management Q&A |
| L2 Results & quality | Latest period: revenue, operating profit, net income/EPS YoY; operating cash flow vs net income; any one-offs | Margin bridge, working capital, capex vs D&A, SBC and dilution, non-GAAP reconciliation, multi-year trend |
| L3 Expectations | Company forecast/guidance (and whether it changed), consensus if findable, progress rate vs forecast (JP) | Revision history, guidance philosophy (conservative?), whisper/implied expectations from price reaction |
| L4 Valuation | P/E (and on which EPS), P/B, EV/EBITDA or P/S as appropriate, vs own history and 2–3 peers | Reverse DCF / implied growth, SOTP, scenario table |
| L5 Capital policy | Dividend policy & payout, buybacks (authorized vs executed), recent issuance/dilution, net cash/debt | Cost-of-capital disclosures (JP), cross-shareholdings, parent-subsidiary structure, capital allocation track record |
| L6 Positioning | JP: 信用買い残/売り残 & 信用倍率, 貸借倍率/逆日歩 if 貸借銘柄, 空売り残高報告 if any. US: short interest % float & days to cover, borrow cost if findable, options implied move near events | Trends over time, investor-type flows, index inclusion/rebalance demand, options OI/skew, ETF/passive ownership |
| L7 Ownership & insiders | Major shareholders and recent changes (大量保有報告, 13D/G), insider transactions (Form 4 / 役員の売買), notable institutions/activists | 13F trends, foreign ownership, cross-holdings unwinds, parent stake moves |
| L8 Catalysts | Next earnings date, known upcoming events (AGMs, lock-ups, index reviews, regulatory dates, deal milestones) | Event probability and payoff, calendar of related-company events |
| L9 Related companies | 2–3 direct peers; key customers/suppliers if disclosed; parent/listed subs | Read-across from their latest results/guidance, two-hop value chain |
| L10 Macro | The 1–3 macro variables that most move this business, and the company's disclosed sensitivity (e.g. 想定為替レート, rate sensitivity) | Scenario impact, policy calendar |
| L11 Sector data | The sector's key KPIs and the latest industry statistic | Multi-period trend, inflection signals |
| L12 News & sentiment | Last ~1–3 months of material news, analyst rating/target changes, notable short-seller or activist reports | Narrative crowding, media/SNS heat, retail interest |
| L13 Price & liquidity | Recent performance vs index and peers, reaction to last earnings, average trading value, volatility | Technical levels, gaps, volume anomalies, liquidity risk for position size |
| L14 Risks | Top disclosed risk factors, litigation/regulatory issues, going-concern or accounting flags, governance issues | Changes in risk factors vs prior year, auditor changes, restatements |

---

## 2. Mandatory lenses by request type

M = mandatory minimum check, ○ = check if quick or relevant, – = usually skip
(still list it in the coverage table as ➖ with a reason).

| Lens | Deep dive | Earnings | Price move | Event | Theme | Comparison | Macro impact | Positioning Q |
|---|---|---|---|---|---|---|---|---|
| L1 Business | M | ○ | ○ | M | M | M | M | – |
| L2 Results | M | M | ○ | ○ | ○ | M | ○ | – |
| L3 Expectations | M | M | M | ○ | ○ | M | ○ | ○ |
| L4 Valuation | M | M | ○ | M | ○ | M | – | ○ |
| L5 Capital policy | M | ○ | ○ | M | – | ○ | – | ○ |
| L6 Positioning | M | M | M | M | ○ | ○ | – | M |
| L7 Ownership | M | ○ | M | M | – | ○ | – | M |
| L8 Catalysts | M | M | M | M | ○ | ○ | M | M |
| L9 Related cos | M | M | M | M | M | M | M | ○ |
| L10 Macro | M | ○ | M | ○ | ○ | ○ | M | – |
| L11 Sector data | M | M | ○ | ○ | M | M | M | – |
| L12 News | M | M | M | M | M | ○ | ○ | M |
| L13 Price | M | M | M | M | ○ | ○ | ○ | M |
| L14 Risks | M | ○ | M | M | ○ | ○ | ○ | ○ |

Notes:

- **Price-move explanation:** start with dated news and filings around the
  move, then check whether the move was market/sector-wide (compare peers and
  the index on the same day) before attributing it to the company. Check
  positioning (short squeeze? margin liquidation?) and index/flow events.
- **Theme discovery:** the job is to separate companies with *verified*
  exposure (disclosed revenue, contracts, capacity, customers) from companies
  merely *associated* with the theme in media lists. Include the less obvious
  layers of the value chain (materials, equipment, components, power,
  cooling, logistics, services) and potential losers.
- **Positioning questions:** always give the precise definition, the as-of
  date and the release date, and at least one complementary indicator (e.g.
  short interest + borrow cost + days to cover; 信用買い残 + 信用倍率 +
  評価損益率 + 出来高).

---

## 3. Contradiction patterns

When you see one of these, prioritize explaining it.

| Pattern | Usually check |
|---|---|
| Strong results, stock falls | Expectations (consensus/whisper too high), guidance, quality of beat (one-offs, tax, FX), positioning (crowded long, 信用買い残の重さ), sector rotation |
| Weak results, stock rises | Results vs lowered expectations, guidance/turnaround signs, short covering, buyback/capital policy news, "bad news priced in" |
| Revenue up, operating cash flow down | Receivables (DSO), contract assets, inventory build, channel stuffing, customer financing, timing/seasonality |
| Net income up, EPS flat | Share count growth (issuance, SBC, converts), minority interests, preferred dividends |
| Profit up via non-operating items | Gains on asset/cross-holding sales, FX gains, tax benefits — recurring or not? |
| Good news, rising short interest / 空売り残高 | Hedging of converts or merger arb, offering anticipation, skeptical fundamental shorts, data lag |
| Low P/B (<1) for years | ROE vs cost of equity, asset quality, cash trapped, cross-holdings, governance, parent-subsidiary conflict; any reform plan and its credibility |
| High multiple, decelerating growth | What growth is implied (reverse DCF), consensus revisions, customer concentration |
| Insider selling during "great" news | 10b5-1 plans, tax/vesting sales vs discretionary; size relative to holdings |
| Insider/company buying while price falls | Signal vs routine program; liquidity; information they might have |
| Theme stock with no theme revenue | Disclosed segment data, actual contracts, capacity; media-list association only? |
| Company guidance conservative every year (JP 期初保守的) | Historical forecast vs actual pattern before reading an upward revision as a surprise |
| Peer reported strong demand, company did not | Share loss, product mix, customer mix, timing |
| Customer cut capex, supplier still guiding up | Order backlog timing, other customers, double ordering risk |
| Margin buyers heavy (信用倍率 high) yet price rising | Fuel for a squeeze vs future selling pressure; 評価損益率; 6-month 制度信用 deadline |
| Price up on low volume / down on heavy volume | Liquidity, distribution, index flows |
| Options imply a bigger move than history | Event risk the market sees that the narrative ignores |

---

## 4. Prioritizing leads and stopping

Score each open lead roughly (High/Med/Low) on:

- **Impact:** could it change the conclusion or the valuation materially?
- **Uncertainty:** how unresolved is it right now?
- **Evidence strength:** is there a concrete trigger (filing, data point)?
- **Cost:** how many searches; is the data paywalled?

Work High-impact × High-uncertainty first. Typical order:

1. Missing latest results or filing (refresh before analyzing anything)
2. A contradiction between lenses
3. A disconfirming signal against the emerging thesis
4. An upcoming dated catalyst within the user's horizon
5. Second-order effects on/from related companies
6. Comparisons that sharpen valuation

Stop a lead when:

- two consecutive searches return nothing new,
- the answer requires paid/proprietary data you cannot access (record it as a
  gap and suggest how the user could get it),
- the remaining uncertainty would not change the conclusion, or
- the depth budget is used up.

Never fill a gap with plausible-sounding numbers. Write it as an open
question in "Next investigations".
