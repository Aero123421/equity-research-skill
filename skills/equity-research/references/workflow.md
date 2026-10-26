# Workflow details

The full procedure behind the summary in SKILL.md. Read this file at the start
of any Standard, Standard-wide or Deep task; Quick questions can rely on the
summary in SKILL.md.

Contents:
1. Step 1 — Frame the request and set the budget
2. Step 2 — Pin down the security and the clock
3. Step 3 — Coverage sweep (wide)
4. Step 4 — Go deep where it matters
5. Step 5 — Disconfirmation pass
6. Step 6 — Synthesize, then check consistency
7. Step 7 — Verify the key numbers
8. Data hygiene checklist

## Step 1 — Frame the request and set the budget

Classify the request; it decides which lenses are mandatory (full matrix in
`references/coverage-map.md`):

| Type | Example | Emphasis |
|---|---|---|
| Single-stock deep dive | 「レーザーテックを調べて」 | all lenses |
| Earnings / guidance reaction | "How was NVDA's quarter?" | expectations, results quality, positioning, peers |
| Price-move explanation | 「なぜ急落した？」 | dated news, index/peer moves the same day, positioning, expectations, macro |
| Event analysis | TOB, M&A, offering, index change, lock-up | terms & probability, positioning, affected third parties |
| Theme / sector discovery | 「データセンター電源の関連銘柄」 | value chain mapping, evidence of actual exposure, sector data |
| Comparison | "TSMC vs Samsung vs Intel" | consistent definitions, valuation, KPIs |
| Macro impact | 「円高でどこが影響を受ける？」 | sensitivities, disclosed assumptions (想定為替レート), sector data |
| Positioning question | 「空売りが多い銘柄？」 | positioning data with correct definitions and lags |

Set depth and a **hard budget of tool calls (web searches + page fetches
combined)**:

| Depth | When | Tool-call budget |
|---|---|---|
| Quick | Narrow factual question | ≤ 30 |
| Standard (default) | Most single-stock, earnings, positioning and price-move questions | ≤ 80 |
| Standard-wide | Theme / sector discovery and multi-company comparisons | ≤ 120 |
| Deep | User asks for 詳しく/徹底的に/thorough research, or high stakes | ≤ 160 |

Depth decides how much you **research**. How much you **show** is decided
separately by the output mode (see `output-template.md`): research wide, answer short unless
a report is asked for.

When writing (in either mode), shorten by cutting repetition, never by dropping
these:
- the single most non-obvious finding (e.g. which product actually drove the
  order recovery);
- primary-filing figures that decide the answer (for earnings: operating
  cash flow, tax rate, SBC/one-offs, share count);
- for earnings: at least three concrete takeaways from the call or
  management commentary (guidance changes, timelines, demand comments);
- the most important market event of the last 30 days for this stock/theme;
- at least one peer, customer or supplier read-across with numbers;
- the dated next events;
- for themes: the exposure figure for each top-tier name (theme share of
  sales, theme orders, or segment numbers), and a "priced in" table (price
  with date, forward P/E or similar, 1M/YTD move) for the top 5+ names.

Iterating on an answer means adding to the evidence, not swapping one good
point for another.

Keep a running count. When you reach the budget, stop researching and write
up what you have, putting open items in "Next investigations". If a site
fails or rate-limits, try at most one alternative URL for it, then move on to
another source.

If the user's question is narrow ("what's the short interest on X?"), answer
it directly first, then add a compact "also worth knowing" block from a light
sweep — the adjacent lenses often change how to read the number they asked
for.

## Step 2 — Pin down the security and the clock

Identify company vs. listed security: exact name, market and code/ticker,
exchange/segment (プライム/スタンダード/グロース, NYSE/Nasdaq), share classes,
ADRs or dual listings, fiscal year end, accounting standard (J-GAAP / IFRS /
US GAAP), parent or listed subsidiaries. Check for recent splits, name or
ticker changes before comparing history.

Establish the clock: today's date, the latest results (period and release
date), and whether anything relevant happened in the last few days (results,
pre-announcements, guidance changes, peer results, major macro data). Do this
early — stale framing is the most common avoidable error.

**Build a dated timeline first** for "why is it moving / why is everyone
talking about it" questions, and for any small or volatile stock: list the
company's own disclosures from the last ~30 days (TDnet 適時開示 / 8-K / press
releases) next to the big price days. Most stories hinge on one or two of these
disclosures, so reading them early keeps the whole answer anchored to facts.

**Re-check time-limited facts.** Warrants (新株予約権/MSワラント), lock-ups,
tender offers, buyback programs, contracts and guidance all have status that
changes. Before relying on one, confirm its current status and date — expired,
cancelled, exercised, extended or completed — rather than carrying an older
description forward.

## Step 3 — Coverage sweep (wide)

Go through the lenses. For each, gather the minimum needed to say something
definite (the minimum check per lens is in `coverage-map.md`).

| # | Lens | Key questions |
|---|---|---|
| L1 | Business & competitive position | How it makes money, segment mix, moat, customers/suppliers |
| L2 | Results & earnings quality | Growth, margins, cash conversion, one-offs, dilution |
| L3 | Expectations | Company forecast/guidance, consensus, revisions, progress rate |
| L4 | Valuation | Multiples vs history and peers, implied growth, scenarios |
| L5 | Capital policy & governance | Buybacks, dividends, dilution, cost-of-capital response, cross-holdings, parent |
| L6 | Supply/demand & positioning | Short interest/ratio, margin balances, lending, flows, options, index demand |
| L7 | Ownership & insiders | Large holders, activists, insiders, institutions, foreign ownership |
| L8 | Events & catalysts | Dated upcoming events, pending deals, lock-ups, index reviews, regulatory decisions |
| L9 | Related companies | Peers, customers, suppliers, parent/subsidiaries, read-across |
| L10 | Macro & cross-asset | Rates, FX, commodities, policy; disclosed sensitivities |
| L11 | Industry data & sector KPIs | Industry statistics and the KPIs that matter for this business model |
| L12 | News, sentiment & narrative | Recent news, analyst actions, short-seller reports, media/SNS heat |
| L13 | Price action & liquidity | Move vs index and peers, reaction to news, volume, volatility, liquidity |
| L14 | Risks | Legal, regulatory, accounting, governance, geopolitical, going concern |

**Which reference files to read.** Always read `coverage-map.md` and
`output-template.md`. Then read only what the task needs — typically 2–3
more files:

- Japanese stock → `supply-demand-jp.md`, `disclosures-earnings.md`
- US stock → `supply-demand-us.md`, `disclosures-earnings.md`
- Earnings question → `disclosures-earnings.md` (+ positioning file)
- Event (TOB, offering, index, FDA, M&A) → `events-catalysts.md`
- Theme / related companies → `related-companies.md`, `macro-sector.md`
- Valuation or comparison → `valuation.md`
- Macro or sector question → `macro-sector.md`

For anything else, look up the specific term in the relevant file rather than
reading every file. Do not rely on memory for the definitions and publication
lags of positioning data — check the reference.

Search tactics:

- Japanese companies: search in Japanese with document and data names
  (決算短信, 有価証券報告書, 適時開示, 大量保有報告書, 信用残 日々, 貸借倍率,
  逆日歩, 空売り残高). US companies: form names (10-K, 10-Q, 8-K, DEF 14A,
  Form 4, 13F, 13D) and "short interest", "days to cover", "implied move".
- Use the company's IR pages for the latest results, presentation and Q&A.
  If IR fails, go to the filing itself: SEC EDGAR (8-K Exhibit 99.1, 10-Q) or
  the TDnet/EDINET document, rather than settling for news summaries.
- **Freshness sweep:** before marking any lens partial or missing, run one
  search for the most recent item of that type (latest peer results this
  week, latest consensus/target aggregation, latest data release). Peers often
  reported days ago with exactly the evidence you are missing.
- **Market-comparison gate (any price move or reaction):** before naming a
  cause, get same-day moves for the main index, the sector index/ETF and 2
  named peers, plus the cumulative return over the window. A market wrap
  usually answers this in one call: "stock market today <Month D, YYYY>" /
  「<M月D日> 日経平均 終値 大引け」. Confirm the stock's close with two sources.
  If you cannot get the market comparison within 3 searches, the headline
  must say the cause is not yet separated from the market move, rather than
  asserting a company-specific cause.
- **Dated events:** reserve 2–3 searches to confirm the next company event
  (earnings date from IR/TDnet/exchange calendars) and the key peer/customer
  and macro dates inside the user's horizon.
- Reserve roughly a fifth of the budget for the final sweep of lenses you have
  not touched yet (often positioning, ownership, catalysts) instead of
  spending everything on the most interesting lead.

## Step 4 — Go deep where it matters

Rank leads and spend the remaining budget on the top ones:

1. **Contradictions** between lenses (catalogue in `coverage-map.md`).
2. **Surprises** versus expectations or history.
3. **High-impact unknowns** that could flip the conclusion (an undisclosed
   major customer, a pending regulatory decision, an upcoming lock-up).
4. **Second-order effects** on related companies (`related-companies.md`).

Stop digging a lead when two consecutive searches add nothing new, when it
needs paid data you cannot access, or when the budget is spent. Record the
open question instead of guessing.

## Step 5 — Disconfirmation pass

Write your headline conclusion in one sentence. Then search for the best
evidence that **this conclusion** is wrong, and state it plainly:

- If you explain a price move, the counter is another explanation (market or
  sector move, positioning unwind, a different piece of news).
- If you conclude "not a squeeze candidate", the counter is the scenario in
  which it squeezes and what would have to happen.
- If you rank theme beneficiaries, the counter is evidence that a top-ranked
  name's exposure is smaller than claimed (or a low-ranked one larger).

Check at least: positioning (is everyone on the same side?), expectations (is
the good/bad news already in consensus?), and one related company that would
show the opposite if your conclusion were wrong.

## Step 6 — Synthesize, then check consistency

Combine into: what the market seems to be pricing in, where the evidence
supports or contradicts that, the key drivers to watch, and conditional
scenarios (what must be true for bull/base/bear). Keep probability language
honest; research priority is not a price forecast.

Before finishing, run the hygiene checklist below, then re-read your draft
once purely for consistency:
- every "see below/above" names a section that exists, or delete it;
- every tier or ranking placement meets that tier's stated test with
  evidence in the body — a top-tier name without its qualifying number
  moves down a tier;
- every "Checked" coverage row has matching content in the answer;
- components add up to the totals you state;
- each figure appears with one value and one basis everywhere;
- every comparative claim (higher/lower, outperformed, "fell less than the
  index", 大半, より割高) is recomputed from your own figures on the same
  basis; if it holds only after an adjustment (e.g. beta), state the
  adjustment, otherwise remove the claim.

## Step 7 — Verify the key numbers

Instructions alone do not stop numeric errors; this step is a separate pass.

1. **Keep a key-number ledger while you research.** List the 5–10 numbers
   and dates the conclusion actually rests on (price moves, results,
   guidance, contract sizes, share counts, positioning figures, event dates).
   For each record: value, period/as-of date, basis (連結/単体,
   GAAP/adjusted), source URL, source type (primary / reputable media /
   aggregator / blog), and whether a second source agrees.
2. **Only ledger numbers may carry the conclusion.** A number that rests on a
   single aggregator or blog is marked unverified; it can be mentioned as
   such but must not decide the answer.
3. **Verification pass after drafting.** For the top numbers in the ledger:
   - re-open the source and confirm the exact value, period and date —
     prefer the primary document (決算短信 / TDnet / EDINET / SEC filing /
     company IR) when reachable;
   - for time-limited items (warrants, lock-ups, offers, buybacks,
     contracts), search for the latest disclosure and confirm their current
     status;
   - recompute every number you derived (percent changes, multiples,
     "x times", dilution, tranche sizes) from its stated inputs — use a code
     tool if one is available;
   - fix the draft wherever the ledger changed.
4. **Independent check when possible.** If your environment can start a
   separate agent (sub-agent / task tool), give a fresh agent the ledger and
   the draft and ask it to verify each number against sources without
   having seen your research. Apply its corrections. If not, do the pass
   yourself, deliberately reading each source as if for the first time.

Reserve roughly 10–15% of the tool-call budget for this step.

## Data hygiene checklist (apply before answering)

- [ ] Company forecast/guidance vs consensus vs actual clearly distinguished;
      nothing labelled "consensus" that is not
- [ ] Period, basis (GAAP/non-GAAP, consolidated), currency and units stated
- [ ] Every positioning/ownership figure has an as-of date (and release date
      when lagged); a figure you cannot date is left out, not hedged; if the
      move you explain happened after the data date, say so
- [ ] Market-wide indicators not confused with stock-specific ones
      (空売り比率 is market-wide; 空売り残高報告 is per stock; FINRA daily short
      volume is not short interest)
- [ ] Borrow cost read as lendable-supply tightness, not short conviction
- [ ] Orders vs backlog vs pipeline vs revenue not confused (受注 / 受注残 /
      引き合い)
- [ ] Per-share data split-adjusted; share count changes considered
- [ ] Prices and key headline figures cross-checked across sources; when
      sources conflict, use the primary or majority figure, show the range,
      and never build a conclusion on a lone outlier
- [ ] Every number you derived yourself (ratios, multiples, "x times",
      tranche sizes) shows its inputs and has been recomputed
- [ ] Time-limited items (warrants, lock-ups, offers, buybacks, contracts)
      have their current status confirmed
- [ ] Price moves compared with the index, sector and peers on the same day
      (or the headline says the cause is not yet separated from the market)
- [ ] At least two confirmed dated next events
- [ ] No consensus/estimate invented when it could not be found
- [ ] Related-company links backed by evidence or labelled unverified
- [ ] Disconfirmation aimed at the headline conclusion
- [ ] Conclusion, rankings and coverage statuses consistent with the body
- [ ] Key-number ledger kept and verification pass (Step 7) done
- [ ] Output mode chosen: Normal by default, Report only when asked
- [ ] Within the tool-call budget and the length guide for the mode
