# 日本株の需給・ポジション・保有データ (Japanese supply/demand and positioning)

Contents:
1. Change log 2024–2026 (as of 2026-10; verify when it matters)
2. 空売り (short selling)
3. 信用取引 (margin trading)
4. 日証金・貸借 (JSF lending)
5. 投資部門別・先物 (investor-type flows and derivatives)
6. 保有・大量保有・自社株買い (ownership and corporate supply)
7. 指数・機関フロー (index and institutional flows)
8. イベント需給 (event-driven supply)
9. 市場センチメント (market-wide sentiment gauges)
10. 個別銘柄の標準需給チェック (standard positioning check)

Always state **as-of date (申込日/基準日) and release date**. Say whether a
figure is market-wide or per stock, and 制度信用/一般信用 where relevant.

---

## 1. Change log 2024–2026

- **銘柄別信用取引残高 is daily from 2026-09-28** (previously weekly). JPX
  posts all issues around 16:00 on the next business day, by 申込日, with yen
  value and ratio to listed shares. Old weekly and new daily series are not
  directly comparable around the switch.
- **信用取引現在高** (market-wide) consolidated into a single weekly file
  (Tuesday ~16:00) from late September 2026.
- **投資部門別売買状況** file format changed (2026-09-29 posting; latest week
  only).
- **大量保有報告 and TOB rules revised 2026-05-01** (TOB threshold 30% incl.
  on-market purchases; joint-holder definitions changed — many mechanical new
  filings appeared around that date).
- **TOPIX second stage:** first periodic replacement effective 2026-10-30;
  non-retained names (移行措置銘柄) are weight-reduced in 8 quarterly steps;
  re-evaluation October 2027. **TOPIX Next-tier** index calculated from the
  same date.
- **Nikkei 225 methodology** revised 2026-10-01 (information & communication
  sector added; same-sector replacement step; 特設注意 → 特別注意).
- **BOJ ETF/J-REIT disposal** decided 2025-09-19 (ETFs ≈¥330bn/year at book
  value); sales reportedly began in 2026. Small vs daily turnover; mainly an
  overhang/sentiment factor; BOJ may avoid selling into sharp falls.
- **日証金 応札ランク (A–F)** for 品貸入札 published since November 2024.
- Cash-equity trading hours extended to 15:30 (late 2024); daily data post
  later.

---

## 2. 空売り

### 空売り比率 (market-wide)
- **Definition:** JPX "空売り集計" reports daily yen value in 実注文 (ordinary
  sells), 空売り(価格規制あり), 空売り(価格規制なし). 空売り比率 = (規制あり +
  規制なし) ÷ total. Covers stocks, ETFs, REITs; includes 信用 shorts. Also by
  33 sectors.
- **Timing:** same day, evening.
- **Reading:** a flow, not a position. 40%+ is now routine (the "40% = bearish
  extreme" rule of thumb is dated). Rising ratio with rising 価格規制あり share
  during a decline = real pressure; very high at lows can precede covering
  rallies.
- **Pitfalls:** much is market-making, arbitrage and intraday hedge selling
  (any sale of unowned shares must be flagged short). **It is market-wide,
  never a stock-specific number.**

### 空売り残高報告 (per stock, 0.2% / 0.5%)
- **Definition:** holders with short positions ≥0.2% of shares issued report
  via their broker; the exchange publishes positions ≥0.5% with the holder's
  name (individuals <5% shown as 個人). Ratio is vs **issued shares**, not
  float. Past 13 months available.
- **Timing:** calculation date + ≈2 business days.
- **Reading:** the reporters' identities and trend matter more than one
  reading. New/increasing reporters = bearish conviction or hedging; large
  disclosed shorts + catalyst = squeeze risk; declining balances = covering.
- **Pitfalls:** misses positions <0.5% (public) and <0.2% (unreported), most
  retail 信用売り, and derivative/swap shorts — it **understates** total
  shorting. Many are hedges (CB arbitrage, merger arbitrage, pairs, index
  hedges). Gross vs net treatment unverified.

### 空売り価格規制
Triggered when a stock falls ≥10% from its base price; until the next day's
close, shorts cannot be placed at or below the latest price (in a falling
market). Limits, not bans, shorting. Indicates a sharp one-day fall.

---

## 3. 信用取引

### 信用残 (信用買い残 / 信用売り残, per stock)
- **Definition:** outstanding margin buys and sells per issue (shares; now
  also yen and % of listed shares). 制度信用: 6-month repayment limit;
  一般信用: terms set by broker (can be indefinite).
- **Timing:** daily since 2026-09-28 (next business day ~16:00). Before that,
  weekly (Friday 申込日, released the following Tuesday).
- **Reading:** rising 買い残 into a falling price = trapped longs, future
  selling (overhang); 買い残 falling after a drop = washed out; high 売り残
  with rising price = squeeze fuel. 制度信用 buy positions roll off within 6
  months — look at when the big build-up happened.
- **Pitfalls:** do not mix with JSF 貸借残 (a subset); balances move with
  price; compare to float and average volume (e.g. 買い残 ÷ 25-day average
  volume = days of volume).

### 信用倍率
- **Definition:** 信用買い残 ÷ 信用売り残 (state whether 制度+一般, or which).
- **Reading:** <1 (売り長) = potential squeeze fuel if price rises; very high
  (e.g. >10×) on a stock that has stalled = overhang.
- **Pitfalls:** noisy for illiquid names; a low ratio isn't bullish alone
  (buyers may be few because the stock is disliked); always look at the
  absolute balances too.

### 信用評価損益率 (market-wide)
- Unrealized P/L of margin buyers as % of position value, published weekly
  by brokers/media (some brokers publish their own daily figure).
- Rule of thumb: about 0% to −20%; near −20% has often been a washout zone,
  near 0% an overheated zone. Heuristic only; regimes shift.

### 日々公表銘柄 / 増担保規制 / 注意喚起
- **日々公表銘柄:** designated when margin positions are extreme vs listed
  shares or margin trading dominates turnover (e.g. short ≥10% of listed
  shares with short/long ≥60%, or long ≥20%; or price far from the 25-day MA
  with high new-margin ratios). Not a sanction — a crowding flag.
- **増担保規制 (委託保証金率引上げ):** stage 1 = 50% (cash 20%), stage 2 = 70%,
  stage 3 = 90%, stage 4 = new margin trades prohibited. Applies to new
  positions; tends to cool speculative rallies and squeezes. Released after
  balances normalize. Brokers may add their own stricter rules.
- **注意喚起:** TSE alert when material information is unclear (financing,
  M&A, revisions, false statements). Can precede a TOB — event risk both
  ways, not necessarily negative.
- **信用取引売買比率:** daily share of new margin buys/sells; feeds the
  regulatory triggers.

---

## 4. 日証金・貸借

### 貸借取引残高 / 貸借倍率 (JSF)
- **Definition:** 融資残 (funds lent for margin buys) and 貸株残 (shares lent
  for margin sells) after brokers' internal matching; 貸借銘柄 only. 貸借倍率
  = 融資残 ÷ 貸株残.
- **Timing:** daily — 速報 same evening (~18:30), 確報 next morning (~11:00).
  Use 確報 for analysis.
- **Reading:** the fastest read on short pressure in 貸借銘柄. 貸株超過 +
  rising 品貸料 = shares hard to borrow (squeeze risk).
- **Pitfalls:** a subset of total margin (excludes internal matching, 一般信用,
  non-貸借 names). Not the same as JPX 信用残.

### 品貸料 (逆日歩)
- **Definition:** fee paid by 制度信用 short sellers (received by buyers)
  when JSF must borrow shares via auction (品貸入札). Per-share fee × days
  (spans holidays/weekends). "*****" (満額) = shortage filled, no fee. 応札ランク
  A (tightest) to F.
- **Timing:** JSF on the auction morning; JPX table ~16:00.
- **Reading:** rising and persistent 品貸料 = crowded short with scarce
  shares → squeeze risk and cost drag on shorts; spikes around 権利付最終日
  (dividend/優待 record dates) are often seasonal (cross trades), not a
  directional signal.

### 貸株注意喚起 / 貸株申込制限 (申込停止)
JSF warns that share procurement may become difficult, then restricts
lending applications; brokers then typically stop new 制度信用 short sales.
Extreme borrow tightness — also common for TOB targets and low-float names.

### 貸借銘柄 vs 信用銘柄
貸借銘柄 can be shorted via 制度信用 (and has visible 貸借倍率/品貸料); other
issues may allow only 一般信用 shorts. Absence from 貸借 does not mean no
shorting. A new 貸借銘柄 selection can attract short selling.

---

## 5. 投資部門別・先物

### 投資部門別売買状況 (stocks, weekly)
- **Definition:** weekly buys/sells by investor type (海外投資家, 個人,
  信託銀行, 投資信託, 事業法人, 生損保, 都銀・地銀等, 証券会社自己 etc.);
  domestic common stocks (ETFs/REITs separate). Includes ToSTNeT (incl.
  buybacks) and 立会外分売.
- **Timing:** 4th business day of the following week (usually Thursday
  afternoon).
- **Reading:** sustained 海外投資家 net buying often drives the index trend;
  事業法人 net buying ≈ buybacks (net buyer for 20+ straight years); 信託銀行
  reflects pensions/rebalancing (often contrarian); 個人 tends to buy dips
  (contrarian).
- **Pitfalls:** cash only — foreign selling via futures shows in the
  derivatives table; one week is not a trend; MOF 対内証券投資 differs in scope.

### 投資部門別取引状況 (futures/options, weekly) and 先物手口
- Weekly futures/options volume by investor type (Thursday). Daily
  participant (broker) volume rankings (~17:45; top 20 by combined buy+sell
  since Nov 2023 — net buy/sell by firm no longer visible); weekly open
  interest by participant.
- **Pitfalls:** broker ≠ end client; much is market-making/arbitrage; volume
  ≠ open interest.

### 裁定取引残高
Index-arbitrage cash positions (裁定買い残 vs 裁定売い残), daily for trades two
business days earlier. Large 裁定買い残 = potential unwind selling near SQ.

### SQ
Nikkei 225 futures/options major SQ on the second Friday of Mar/Jun/Sep/Dec;
options SQ monthly.

---

## 6. 保有・大量保有・自社株買い

### 大量保有報告書 / 変更報告書 / 特例報告
- **Rule:** >5% holders file within 5 business days; 変更報告 on ±1% changes
  or material changes. Institutions may use 特例報告 (fixed reference dates,
  twice monthly) unless they intend >10% or 重要提案行為.
- **Reading:** new 5% holders, activists stating 重要提案行為 purpose,
  strategic buyers = catalysts; core holder/parent/founder reductions = supply.
- **Pitfalls:** ratio is at the obligation date (up to ~a week old at
  release); 純投資 vs 重要提案行為 purpose; 2026-05-01 rule change triggered
  mechanical joint-holder filings; 5% is a disclosure line, not control (TOB
  trigger is 30%).

### 自己株式取得 (buybacks)
- Board resolution on TDnet (枠: shares, amount, period) → monthly
  自己株券買付状況報告書 (by ~the 15th of the next month; shows monthly
  purchases and progress vs 枠) → completion notice. ToSTNeT-3 executions are
  usually a specific seller.
- **Pitfalls:** 枠 is a ceiling; programs pause before results; treasury
  shares can be reissued unless cancelled (消却).

### 大株主・外国人持株比率・株式分布状況調査
- 有報 大株主の状況 (top 10 at FYE; 信託口 are custody accounts, not economic
  owners). JPX 株式分布状況調査 (annual; foreign ownership at record share of
  market value in FY2025).
- High foreign ownership = sensitivity to global risk-off and yen; low
  foreign ownership + reform story = potential new buyers.

### 政策保有株
Disclosed per company in 有報 (株式の保有状況). Unwinding = supply (often
via 売出し or issuer ToSTNeT-3 buyback) and higher effective float.

### 浮動株比率 / 流通株式
Index float (for TOPIX weights) differs from 流通株式 used for listing
standards. Rising float ratio → index weight up (passive buying) and vice
versa.

---

## 7. 指数・機関フロー

- **TOPIX (second stage):** continuation requires annual turnover ≥0.14 and
  cumulative free-float market cap within the top 97% (check final rules for
  addition criteria). Annual review effective late October; 移行措置銘柄
  weight cut in 8 quarterly steps. Check a stock's status (retained / added /
  transition) and estimate flow vs average trading value.
- **Nikkei 225:** reviews effective first business day of April and October;
  liquidity-based; price-weighted with 株価換算係数; high-priced names
  dominate the index.
- **JPX-Nikkei 400** (annual), **MSCI** (quarterly; Feb/May/Aug/Nov),
  **FTSE**.
- **BOJ ETF disposal:** slow pro-rata selling; overhang/sentiment.
- **GPIF:** rebalancing within bands; check the current policy mix before
  citing it.

---

## 8. イベント需給

- **権利付最終日:** two business days before the record date (T+2).
  Dividend/優待 demand builds into it and unwinds after; 品貸料 spikes around
  it (クロス取引).
- **公募増資・売出し (PO):** announcement → pricing about a week later at a
  discount; shorts active into pricing; over-allotment/syndicate cover.
- **立会外分売:** small discount distribution to widen the shareholder base
  (often to meet 貸借/listing criteria); brief selling pressure.
- **MSワラント/CB:** continuous selling as exercised; CB arbitrage shorts
  appear in 空売り残高報告.
- **TOB:** target trades near the offer; 貸株注意喚起/申込停止 common; shorts
  squeezed if a premium bid appears.
- **Index events:** pre-positioning and closing-auction volume on effective
  dates.

---

## 9. 市場センチメント (market-wide)

| Gauge | Definition | Conventional reading | Pitfalls |
|---|---|---|---|
| 日経VI | 30-day implied vol from Nikkei 225 options (Nikkei Inc., real time) | Spike = fear (often near capitulation); low = complacency | Not directional; expiry/hedging effects |
| 騰落レシオ | Usually 25-day advancers ÷ decliners × 100 (vendor-computed) | ≥120 overheated, ≤70 oversold (rule of thumb) | Universe (Prime vs all) matters; stays extreme in trends |
| 日経225オプション Put/Call | Put ÷ call volume or OI (vendor-computed) | Extremes contrarian | Institutional hedging; expiry distortions |
| 空売り比率 | See §2 | Context only | Flow, not position |
| 信用評価損益率 | See §3 | −20% washout / 0% overheated (heuristic) | Weekly lag; regime shifts |
| 売買代金・回転率 | Daily trading value; turnover | Rising value with rising prices = participation | Index/SQ days inflate; compare with 25-day average |

---

## 10. 個別銘柄の標準需給チェック

1. **信用残:** 買い残, 売り残, 信用倍率 (state 申込日 and release date), trend
   over 4–12 weeks, 買い残 vs average daily volume; when the build-up happened
   (制度信用 6-month deadline).
2. **貸借 (if 貸借銘柄):** 貸借倍率, 貸株超過, 品貸料 and 応札ランク history,
   貸株注意喚起/申込制限.
3. **空売り残高報告:** reporters ≥0.5%, total disclosed %, trend, reporter
   types (hedge funds, prop, CB arbitrage).
4. **Regulatory flags:** 日々公表, 増担保規制, 注意喚起.
5. **Holders:** 大株主 (excluding 信託口), recent 大量保有/変更報告, activists,
   parent/cross-holders likely to sell, foreign ownership.
6. **Corporate supply/demand:** buyback progress, recent/possible equity
   issuance, MS warrants/CB, 売出し, 立会外分売.
7. **Index:** TOPIX status (retained/added/transition), Nikkei 225 or other
   index review candidacy, float changes.
8. **Calendar:** earnings, 権利付最終日, SQ, index effective dates, lock-up
   (IPO) expiry.
9. **Liquidity:** average 売買代金, 浮動株比率, price limits.

Squeeze-candidate test (all should be checked; none is sufficient alone):
売り長 or rising 売り残, 逆日歩 persistence and 応札ランク tight, 貸株申込制限,
disclosed short reporters building, small float, a plausible positive
catalyst, and shorts that are directional rather than hedges.

Finding the data (search phrases that usually work):
- 信用残 (daily since 2026-09-28): 「<銘柄名> 信用残 日々」「銘柄別信用取引残高
  JPX」. Many aggregator pages still show the weekly series — check which
  series and 申込日 you are reading.
- 貸借・逆日歩: 「<銘柄名> 日証金」「<コード> 貸借倍率」「<銘柄名> 逆日歩」.
  Only 貸借銘柄 have these.
- 空売り残高報告: 「<銘柄名> 空売り残高」 (JPX publishes; aggregators list by
  reporter and 計算日).
- 規制: 「<銘柄名> 日々公表」「<銘柄名> 増担保」「<銘柄名> 貸株注意喚起」.
