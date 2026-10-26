# Valuation, price action and liquidity

Contents:
1. Choosing the right metric
2. Computing multiples correctly
3. Relative valuation (history and peers)
4. Implied expectations and scenarios
5. Japan- and US-specific valuation habits
6. Price action and liquidity checks
7. Common valuation mistakes

---

## 1. Choosing the right metric

| Business type | Primary metrics | Why / caveats |
|---|---|---|
| Profitable, stable | P/E (forward and trailing), EV/EBIT, FCF yield, dividend yield | Check EPS quality and one-offs |
| Capital-heavy / cyclical (steel, chemicals, shipping, semicap equipment, autos) | EV/EBITDA, P/B, mid-cycle P/E | Peak earnings → low P/E is a trap; trough earnings → high P/E can be cheap |
| Banks / insurers | P/B or P/TBV vs ROE, dividend + buyback yield; insurers: embedded value / EV-based metrics | EV/EBITDA meaningless for financials |
| REITs / real estate | P/FFO or P/AFFO, P/NAV, dividend yield, cap rate vs rates | Depreciation distorts EPS |
| High-growth, unprofitable | EV/Sales vs growth, gross margin, path to profitability, cash runway | Check dilution and SBC; Rule of 40 for SaaS |
| Holding companies / conglomerates (商社, 持株会社) | Sum of the parts (SOTP), discount to NAV | Listed subsidiaries at market value; holding discount |
| Biotech (pre-revenue) | Risk-adjusted NPV of pipeline, cash vs burn, EV vs cash | Binary event risk |
| Asset-rich low P/B (JP common) | P/B, net cash/market cap, cross-shareholdings at market | Whether management will unlock value matters more than the number |

## 2. Computing multiples correctly

- **State which earnings:** trailing 12 months, last fiscal year, company
  forecast (会社予想), or consensus forward. In Japan the commonly quoted
  "予想PER" usually uses the company forecast — say so.
- **Market cap uses shares outstanding net of treasury shares** (自己株式を
  除く). Japanese companies often hold large treasury stock; using issued
  shares overstates market cap.
- **EV = market cap + interest-bearing debt + preferred + minority interest −
  cash & equivalents** (be explicit if you include lease liabilities,
  investment securities or cross-holdings). For Japanese companies with large
  securities holdings, show EV with and without them.
- **Per-share figures must be split-adjusted** across periods.
- **Non-GAAP vs GAAP:** note which. US "adjusted EPS" often excludes SBC and
  amortization; compare like with like across peers.
- **IFRS vs J-GAAP:** IFRS 営業利益 can include other operating income/
  expenses; J-GAAP amortizes goodwill (のれん償却) while IFRS/US GAAP do not.
  Adjust before comparing.
- **Currency:** convert peers to a common currency at a stated rate and date,
  or compare ratios (currency-neutral) only.

## 3. Relative valuation

- **Own history:** current multiple vs its 5–10 year range; ask what changed
  (growth, margins, rates, governance) before calling it cheap or expensive.
- **Peers:** pick 3–6 genuinely comparable companies (same business model,
  similar growth/margins/cyclicality). Include cross-border peers when the
  real competitors are global (e.g. Japanese semicap vs US/European peers).
- **Explain the gap:** a discount needs a reason (lower ROE, governance,
  liquidity, parent overhang, cyclicality, accounting). Only an unexplained or
  closing gap is an opportunity signal.

## 4. Implied expectations and scenarios

- **Reverse DCF / implied growth:** ask what revenue growth and margin the
  current price implies. A simple sanity check: at a given P/E and required
  return, what earnings growth is needed?
- **Scenario table:** bear/base/bull with explicit EPS (or FCF) and multiple
  assumptions, plus what must be true for each. Return = (EPS change) ×
  (multiple change) + dividends. Show that multiple compression can offset
  earnings growth.
- **Rates sensitivity:** long-duration (high-growth) equities are more
  sensitive to discount-rate changes; state this as a sensitivity, not a
  prediction.
- Label all scenario inputs as assumptions. Do not present a single target
  price as fact.

## 5. Japan- and US-specific habits

**Japan**
- P/B and ROE are central since the TSE cost-of-capital initiative; check
  whether the company has disclosed a plan, targets (ROE, P/B, DOE), and
  progress. A plan alone is not execution.
- Dividend yield plus 株主優待 value matters to retail-heavy stocks; 優待
  changes move prices.
- 会社予想 conservatism differs by company; compare past initial forecasts
  with actuals before using company forecast EPS for P/E.
- Parent-subsidiary listings (親子上場) can carry a discount or a takeout
  premium expectation.

**US**
- Forward P/E on consensus EPS and EV/sales are the common language; check
  the consensus revision trend (estimates rising or falling).
- SBC-adjusted metrics: compare FCF after SBC for software/internet names.
- Buyback yield and net share count change matter as much as dividends.

## 6. Price action and liquidity checks (L13)

Minimum:
- Performance over 1M / 3M / 12M vs the relevant index (TOPIX/日経平均,
  S&P 500/Nasdaq-100/Russell 2000) and vs 2–3 peers.
- Reaction to the last earnings release (day-1 and multi-day), and to major
  news.
- Average daily trading value (売買代金) and whether liquidity is adequate for
  the user's likely size; note for small caps.
- Volatility regime: recent realized volatility vs history; options-implied
  volatility if available (US).

Deeper:
- Gaps and whether they filled; volume on up vs down days.
- Distance from 52-week high/low; key moving averages (as context, not as a
  standalone signal).
- Relative strength vs sector; whether a move was idiosyncratic or
  sector/market-wide (check the same day across peers).
- Japan: price limits (値幅制限) and ストップ高/安 can distort daily data;
  low-float stocks can move on small orders.

Interpretation discipline: describe what price/volume shows, do not infer
information that is not in the data. Technical observations are one lens, not
a conclusion.

## 7. Common valuation mistakes

- Calling a cyclical "cheap" on peak earnings.
- Comparing P/E built on company forecast with P/E built on consensus.
- Using issued shares instead of shares outstanding ex-treasury.
- Ignoring net cash for cash-rich Japanese companies (or ignoring that the
  cash may never be returned).
- Comparing IFRS operating profit with J-GAAP operating profit without
  adjustment.
- Ignoring dilution from SBC, converts, warrants (MS ワラント), or ATM
  programs.
- Treating a low P/B as automatically undervalued.
- Treating an analyst price target as an expectation of the market.
