# US supply/demand, positioning and ownership data

Contents:
1. Rule status board (as of 2026-10; verify)
2. Short selling and securities lending
3. Ownership and insider filings
4. Corporate supply: buybacks, offerings, lock-ups, converts
5. Options and volatility
6. Flows, leverage and sentiment
7. Index events
8. Standard positioning check for a single US stock

Always report **as-of date and release date** for lagged data. The freshest
FINRA short interest is typically 1–2 weeks old and can be ~4 weeks old just
before the next release.

---

## 1. Rule status board (as of 2026-10; verify before citing)

| Item | Status |
|---|---|
| FINRA short interest | Twice a month (mid-month and month-end settlement dates); published ≈7 business days after settlement. A 2026 FINRA proposal for weekly reporting was withdrawn (Aug 2026). |
| SEC Rule 13f-2 / Form SHO (aggregated manager short positions) | Adopted 2023; compliance delayed to **January 2028**. No public aggregated data exists yet — do not cite "Form SHO data". |
| SEC Rule 10c-1a (securities lending reporting) | Delayed: reporting from **Sep 2028**, public dissemination **Mar 2029**. No official borrow-fee data exists today. |
| 13D / 13G | 13D within 5 business days of crossing 5%; amendments within 2 business days. 13G timing depends on filer type (5 business days for passive; 45 days after quarter-end for QIIs/exempt). |
| Form 4 | Due within 2 business days; checkbox for Rule 10b5-1 plan trades. Since March 2026, directors and officers of many foreign private issuers also file Section 16 reports (Japan is not among the exempted jurisdictions; check per issuer). |
| Buyback disclosure | SEC's 2023 daily-repurchase disclosure rule was vacated; the quarterly monthly-breakdown table (10-Q Part II Item 2 / 10-K Item 5) applies. 1% excise tax on net repurchases. |
| Periodic reporting | Quarterly 10-Q remains law. An optional semiannual report was proposed (May 2026) but not adopted as of Oct 2026. |
| Russell | Semiannual reconstitution from 2026 (June and December). |
| Nasdaq-100 | Fast Entry rule for very large new listings; low-float shares capped at 3× free float (May 2026). |
| S&P 500 | 12-month seasoning and GAAP-profitability tests unchanged (June 2026). Market-cap minimum reviewed periodically — look up current value. |

---

## 2. Short selling and securities lending

### Short interest (FINRA)
- **Definition:** gross open short positions (shares) across FINRA member
  firms as of the settlement date. A balance, not a flow; gross, not net.
- **Lag:** ≈7 business days after settlement; twice a month.
- **Reading:** high/rising = bearish conviction or hedging; also squeeze fuel
  if good news arrives. Falling after a decline = shorts covering (fuel gone)
  or profit-taking.
- **Pitfalls:** confusing with daily short volume; stale by weeks; includes
  hedges (convertible arbitrage, merger arbitrage, pairs, market-maker and
  ETF hedges); "% of float" depends on the float source; split adjustments
  vary by vendor.

### Short interest % of float; days to cover
- **% of float:** short interest ÷ free float (not shares outstanding for
  low-float names). Practitioners often call >10–20% "high"; no official
  threshold.
- **Days to cover:** short interest ÷ average daily volume. Windows and
  volume definitions differ by vendor. High values (>5–10 days) amplify
  squeezes; but volume surges during a squeeze, so the ratio falls just as it
  starts. Not a forecast of time.
- Float changes with lock-ups, secondaries and index float updates — the same
  short interest can mean different percentages weeks apart.

### Daily short sale volume (FINRA Reg SHO files) — NOT short interest
- **Definition:** shares sold short each day in off-exchange (TRF/ADF/ORF)
  reported trades, with total reported volume; "short volume ratio".
- **Lag:** same day.
- **Pitfalls:** mostly market-maker liquidity provision and intraday round
  trips; ratios of 40–50% are normal for liquid names; excludes exchange
  executions; a 60% short volume ratio does **not** mean 60% of float is
  short. Use only as a change vs the stock's own baseline.

### Reg SHO threshold list and fails-to-deliver (FTD)
- **Threshold list:** persistent fails (≥10,000 shares and ≥0.5% of shares
  outstanding for five consecutive settlement days); published daily by
  exchanges.
- **FTD data (SEC):** cumulative net fail balances, published twice monthly
  with ≈2-week lag (sometimes longer).
- **Pitfalls:** fails arise from long and short sales and operational issues;
  not proof of "naked shorting". ETFs have structural fails.

### Securities lending: cost to borrow, utilization, shares on loan, HTB
- **Definitions:** cost to borrow (annualized fee), utilization (on loan ÷
  lendable supply), shares on loan, hard-to-borrow (broker designation).
- **Sources:** no official public US series today; vendors and brokers
  (indicative tables). Different sources are not comparable.
- **Reading:** rising fee + utilization near 100% = tight borrow, strong short
  demand, squeeze-prone; a sudden fee drop may mean supply returned (e.g.
  after a lock-up).
- **Pitfalls:** utilization denominator is lendable supply, not float; shares
  on loan ≠ short interest.

### Short-sale circuit breaker (Rule 201)
A ≥10% intraday drop from the prior close restricts short sales to above the
national best bid for the rest of that day and the next. A price trigger,
not a positioning signal.

---

## 3. Ownership and insider filings

### Form 13F
- Quarterly long positions in 13(f) securities by managers with ≥$100M;
  due 45 days after quarter-end.
- **Pitfalls:** excludes short positions; options reported as notional of
  the underlying (a put is not a long); 45-day to ~2.5-month staleness;
  confidential treatment can delay some positions; holder counts double count
  sub-advisers; non-US institutions largely missing.
- Use for: concentration, crowding among hedge funds, trend in ownership —
  not for current positioning.

### Schedule 13D / 13G
13D = activist/control intent; 13G = passive/QII. A new 13D from an activist
or strategic buyer is a catalyst; a 13D holder cutting below 5% is a supply
signal. "Group" formation and cash-settled swaps are interpretive grey areas.

### Form 4, Form 3/5, Form 144
- **Form 4:** within 2 business days. Transaction codes: P (open-market
  purchase), S (sale), A (award), M (option exercise), F (tax withholding),
  G (gift). Only P and S are discretionary trades; check the 10b5-1 checkbox
  and footnotes (indirect holdings).
- **Form 144:** notice of proposed sale by affiliates above 5,000 shares or
  $50,000 in three months; public at filing, so it can precede the Form 4.
  Not every filed amount is sold.
- **Interpretation:** opportunistic open-market purchases, especially cluster
  buys after a price drop, carry the most information; routine and planned
  sales carry little. Sales have many non-informational reasons (taxes,
  diversification, vesting). Do not treat all sales as bearish.

### Institutional and passive ownership; float
- Institutional ownership % can exceed 100% (double counting, re-lending).
- High passive ownership raises sensitivity to index events and broad flows.
- **Float vs shares outstanding:** float excludes insider, strategic and
  locked-up holdings; providers differ (S&P IWF, FTSE Russell). Small float =
  higher squeeze and volatility risk; float expansion (lock-up, secondary,
  ATM) = supply.

---

## 4. Corporate supply: buybacks, offerings, lock-ups, converts

- **Buybacks:** authorization (non-binding) vs execution (10-Q repurchase
  table by month; cash-flow statement). Net buyback = repurchases − issuance
  (SBC). Blackout windows from around quarter-end to the earnings release are
  company policy (10b5-1 plans can execute through them). Rule 10b-18 safe
  harbor limits (timing, price, ≤25% of ADTV). ASRs reduce share count
  upfront.
- **Offerings, shelf, ATM:** a shelf (S-3) is not an offering; ATM capacity is
  a maximum; ATM usage appears only in later 10-Q/10-K. Distinguish primary
  (company) vs secondary (holders) shares. Shorts often front-run overnight
  deals.
- **Lock-ups:** usually 90–180 days after IPO, often staged or with
  early-release triggers (price/earnings). Check prospectus (424B4) and
  amendments; actual selling shows later in Form 4/144.
- **Convertibles:** arbitrageurs buy the bond and short stock (delta hedge);
  rising short interest after a convert is often arbitrage, not bearish
  conviction. Check capped calls/call spreads.

---

## 5. Options and volatility

| Indicator | What it is | Reading | Pitfalls |
|---|---|---|---|
| Open interest (OI) | Outstanding contracts by strike/expiry | Large call OI above spot / put OI below spot show where positioning sits | Doesn't show who is long/short; one day stale; 0DTE leaves no end-of-day OI |
| Put/call ratio | Put ÷ call volume or OI; Cboe publishes equity, index, total | High equity P/C = fear/hedging (contrarian bullish at extremes); low = complacency | Index P/C is mostly hedging and structurally higher; sold puts count as volume; baselines shifted with retail/0DTE |
| Implied volatility, IV rank/percentile | Volatility priced by options; rank vs 52-week range | High IV before an event = big move priced, no direction | Rises mechanically into earnings; vendor conventions |
| Skew | OTM put IV vs call IV | Steep put skew = downside hedging demand; call skew = speculative upside demand | Definition-dependent; rises when spot falls; overwriting distorts |
| Implied earnings move | ≈ ATM straddle (expiring just after the report) ÷ spot | Compare to the stock's historical earnings moves; rich vs cheap | Straddle overstates one standard deviation (~0.8σ); other days in expiry |
| Max pain | Strike minimizing option holders' payoff | Pinning hypothesis — weak evidence | Treat as curiosity, not signal |
| Dealer gamma (GEX) | Estimated dealer net gamma from OI with assumed signs | Positive gamma dampens moves; negative amplifies | Sign assumption unobservable; vendors disagree; 0DTE invisible; hypothesis only |
| Unusual options activity | Volume ≫ OI or normal | Possible informed positioning before events | Direction ambiguous (buy vs sell, spreads, hedges); survivorship bias |
| VIX, term structure, SKEW, VVIX | Market-wide implied vol and tail pricing | Backwardation = acute stress; contango = calm | VIX not directional; SKEW not a timing tool |

Expirations: monthly options on the third Friday (holiday shifts occur);
quarterly expirations coincide with index futures expiry and S&P/Nasdaq
rebalances (triple/quad witching). VIX expires on a Wednesday ~30 days
before the next month's third Friday.

---

## 6. Flows, leverage and sentiment (market-wide)

| Indicator | Timing | Reading | Pitfalls |
|---|---|---|---|
| ETF creations/redemptions, ICI ETF net issuance | Daily (sponsors) / weekly (ICI) | Sustained inflows = demand; sector ETF flows pressure baskets | Secondary volume ≠ flow; arbitrage creations in large ETFs |
| Mutual fund flows (ICI) | Weekly estimate, monthly actual | Rotation to ETFs ≠ bearish | Structural distortions (e.g. share-class conversions to collective trusts); excludes ETFs |
| Leveraged/inverse ETF rebalancing | Daily near the close | Buys after up days, sells after down days (L(L−1) × AUM × return) | Effect has weakened; swap-based hedging |
| Retail flow proxies | Varies; mostly vendor | Momentum support and crowding signal in small caps | Model-dependent; mostly paid |
| FINRA margin debt | Monthly, ≈3rd week of next month | Leverage/risk appetite; sharp falls = deleveraging | Use vs market cap or y/y; excludes derivatives leverage |
| AAII sentiment | Weekly (Thursday) | Contrarian at extremes | Weak alone |
| CFTC Commitments of Traders (TFF) | Tuesday data, Friday release | Extreme leveraged-fund shorts in index futures can fuel squeezes | Often basis-trade legs; only futures slice |
| Off-exchange / ATS volume (FINRA OTC transparency) | Weekly, 2–4 week delay | Block activity without lit footprint (ambiguous) | Most off-exchange volume is wholesaler internalization, not "dark pools"; no direction |

---

## 7. Index events

- **S&P 500:** committee-selected; US domicile, market-cap minimum (check
  current), float (IWF ≥ 0.10), liquidity, 12-month seasoning, positive GAAP
  earnings (latest quarter and trailing four quarters). Quarterly rebalance
  after the third Friday of Mar/Jun/Sep/Dec; ad hoc changes on M&A.
  Inclusion = forced passive buying around the effective close, often
  partially reversing; deletion = forced selling.
- **Russell:** rank day → preliminary lists → effective after close (June and
  December from 2026). Moves from Russell 1000 to 2000 usually bring net
  passive buying (bigger weight in the smaller index); banding limits churn
  near the breakpoint. Pre-positioning is crowded and often reverses.
- **Nasdaq-100:** annual December reconstitution (reference: last trading day
  of November); quarterly rebalances; weight caps; Fast Entry can push the
  count above 100 temporarily.
- **MSCI:** quarterly reviews (Feb/May/Aug/Nov announcements; effective at
  month-end close).
Check the opposite flow in deleted/replaced names and arbitrageur shorts.

---

## 8. Standard positioning check for a single US stock

1. Short interest (latest settlement date and release date), % of float,
   days to cover, and the trend over the last 3–6 reports.
2. Borrow cost and utilization if available (label source; indicative).
3. Reasons shorts may be hedges: recent converts, pending M&A (arb), ETF
   heavy.
4. Options: implied move into the next event vs history; put/call and skew
   vs the stock's own norm; large OI strikes near expiry.
5. Insider activity in the last 3–6 months (open-market P/S only; 10b5-1
   flag); Form 144 notices.
6. Ownership: top holders and recent 13F changes (stale), 13D activity,
   passive share.
7. Supply calendar: lock-ups, ATM usage, shelf takedowns, buyback execution
   pace, index events.
8. Liquidity: average daily dollar volume vs float; recent volume anomalies.

Squeeze-candidate test (all should be checked, none alone is sufficient):
high % of float short, high days to cover, high and rising borrow cost /
utilization near 100%, small float, a plausible positive catalyst, call skew
or heavy near-dated call OI, and shorts that are directional rather than
hedges.
