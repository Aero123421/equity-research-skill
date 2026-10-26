# Macro, cross-asset and sector data

Contents:
- Part A: How to use macro in equity research
- Part B: Macro and cross-asset indicators (Japan / US / Asia)
- Part C: Sector KPIs and industry statistics (22 sectors)
- Part D: Cross-cutting data rules

This file teaches mechanisms, typical timing and misreadings. **Levels and
the current policy regime go stale fast. Always look up the current policy
rate, the latest prints and the official release calendar before using
them.** Release timings below are typical patterns; confirm exact dates on the
publisher's calendar.

---

## Part A. How to use macro in equity research

1. Identify the 1–3 macro variables that actually move this company's profit
   or valuation (rates, FX, a commodity, a policy, a demand indicator).
2. Find the company's **disclosed sensitivity** (e.g. operating profit impact
   per ¥1 move, 想定為替レート, rate sensitivity per +25bp, commodity
   sensitivity tables) and hedging policy. Prefer this to generic rules.
3. Compare the company's assumption with the current market level and with
   consensus forecasts of that variable.
4. Map second-order effects: every macro move has winners and losers. List
   both (e.g. weak yen: exporters and inbound tourism up; importers,
   utilities, airlines, food with imported inputs down).
5. Check the upcoming macro calendar within the user's horizon (central bank
   meetings, CPI, jobs, GDP, Tankan) as catalysts.

---

## Part B. Macro and cross-asset indicators

### B1. Monetary policy

| Item | Typical timing | Sensitive sectors | Misreading to avoid |
|---|---|---|---|
| **日銀 金融政策決定会合** | 8 meetings/year, 2 days each; 展望レポート at the Jan/Apr/Jul/Oct meetings; 主な意見 ≈1 week later; minutes after the next meeting | Banks/insurers (higher rates, steeper curve: positive), real estate/REITs/utilities/long-duration growth (negative), exporters via yen | Reading only the decision. Vote split, dissents, the press conference and the 展望レポート risk balance carry the signal. A hold with hawkish language can move yen and JGBs. |
| **FOMC** | 8 meetings/year; SEP and dot plot only at Mar/Jun/Sep/Dec meetings; minutes ≈3 weeks later | Same logic; regional banks (curve, CRE), homebuilders, REITs, small caps | Dots are not commitments. Compare with the market-implied path (futures/OIS), not the prior dots. |
| **Trade / tariff policy** | Ad hoc | Autos, machinery, steel, semis, pharma, retailers with imported goods | Quoting a headline tariff rate without legal basis, exemptions, who absorbs the cost, or legal challenges. Look up the current regime. |
| **Fiscal / political events** | Budget cycles, elections, US shutdowns | Defense, construction, healthcare, super-long JGBs | Shutdowns delay and can permanently damage data series. |

### B2. Rates, curve, real yields, FX

| Item | Frequency | Sectors | Misreading to avoid |
|---|---|---|---|
| **JGB 2y/10y/30y** | Daily | Banks and life insurers benefit from higher yields over time; bond mark-to-market losses hit capital; REITs/real estate down | "Higher yields good for banks" without checking 有価証券評価損益 and capital treatment. Weak super-long auctions (tail, bid-to-cover) are a term-premium/fiscal signal, not necessarily a BOJ signal. |
| **UST 2y/10y, 2s10s** | Daily | Banks (steepening +), long-duration growth (−), utilities/REITs (−) | An inverted curve leads recessions by quarters and un-inverts before downturns. Bear-steepening from term premium ≠ from growth. |
| **Real yields / breakevens** | Daily | Gold and long-duration growth move inversely to real yields | Breakevens include liquidity and oil effects, not just inflation expectations. Japan's linker market is thin; use swaps and Tankan inflation expectations. |
| **USDJPY** | Daily; MOF intervention data monthly/quarterly | Exporters (+ on weak yen), inbound/duty-free (+); importers, airlines, utilities, food (−) | Uniform benefit assumed. Check per-¥1 sensitivity, hedge ratio, translation vs transaction effects, and the company's assumed rate. Tankan assumed rates tend to be conservative. |
| **DXY** | Daily | EM, commodities | Euro-heavy; a poor yen proxy. Use USDJPY and the US–Japan 2y spread. |

### B3. Inflation

| Item | Timing pattern | Sectors | Misreading to avoid |
|---|---|---|---|
| **Japan CPI** (総務省): core (ex fresh food), core-core (ex fresh food & energy). **Tokyo 23-ward CPI** is the early read around month end. | Monthly | Retail, food, utilities; banks via BOJ path | Policy noise: energy subsidies, fee waivers, tax changes shift the y/y. Strip them before inferring BOJ implications. |
| **企業物価 (CGPI), SPPI** (BOJ) | Monthly | Materials, food, retailers (margin pass-through) | Input price ≠ margin. Check 価格転嫁 and Tankan 販売/仕入価格DI. |
| **US CPI** (BLS) | Mid-month | Retail, staples, REITs (shelter), banks | **US October 2025 CPI was never collected** due to the shutdown; BLS will not publish October 2026 12-month changes for affected indexes. Check base effects around Oct–Nov 2025 data. |
| **PCE / core PCE** (BEA) | ≈4 weeks after month | Fed reaction function | CPI core ≠ PCE core (weights; healthcare and financial services). |
| **PPI, import prices** | Monthly | Industrials, materials | PPI final demand has a large margin/trade-services component. |

### B4. Labor and wages

| Item | Timing pattern | Sectors | Misreading to avoid |
|---|---|---|---|
| **毎月勤労統計** (厚労省): 現金給与総額, 所定内給与, 実質賃金, 共通事業所ベース | 速報 ≈5 weeks after month; 確報 ≈1 month later | Retail, restaurants, consumer finance; BOJ | 現金給与総額 includes bonuses (Jun/Jul, Dec swings). January sample rotation causes breaks; compare 共通事業所. |
| **春闘** (連合 tallies Mar → final early Jul) | Annual | Services, staffing, banks via BOJ | Mixing 定期昇給 with ベア; sample skewed to large unionized firms; flows into wages gradually. |
| **有効求人倍率, 完全失業率**; Tankan 雇用人員判断DI | Monthly/quarterly | Staffing, restaurants, logistics | Ratio can fall from fewer postings or shrinking labor supply. |
| **US payrolls & unemployment** (BLS, first Friday) | Monthly | Cyclicals, staffing, banks | Large revisions; low survey response rates; annual benchmark revision. Breakeven payroll growth depends on immigration. |
| **JOLTS, jobless claims, ECI, AHE** | Monthly/weekly/quarterly | Staffing, consumer | Openings ≠ hiring (use hires/quits); claims noisy around holidays; ECI is the cleanest wage-cost gauge. |

### B5. Growth, activity, surveys

| Item | Timing pattern | Sectors | Misreading to avoid |
|---|---|---|---|
| **日銀短観**: 業況判断DI, 先行き, 想定為替レート, 設備投資計画, 雇用人員判断DI, 価格DI, 企業の物価見通し | Quarterly (Mar/Jun/Sep/Dec surveys; released early Apr/Jul/Oct, mid-Dec). A survey redesign is planned from 2027 — check for series breaks. | Large manufacturers (cyclicals), non-manufacturers (domestic demand), capex plays | DI measures breadth, not magnitude. 設備投資計画 starts low in March and is typically revised up — compare with the same survey month in prior years. 先行き is habitually cautious. |
| **機械受注** (内閣府): 船舶・電力を除く民需 | Monthly, ≈6 weeks lag; quarterly 見通し | Machinery, FA, electrical equipment | ±5–10% monthly swings are normal; use 3-month averages. Orders ≠ production. |
| **鉱工業生産** (経産省): 速報, 確報, 予測指数 | 速報 at end of following month | Autos, machinery, steel, chemicals | 予測指数 is chronically optimistic; use the METI-adjusted (補正) estimate. |
| **Japan GDP**: 1次速報, 2次速報 (after 法人企業統計) | ≈6–7 weeks and ≈10 weeks after quarter | Broad | Annualized q/q is volatile; revisions can be large. |
| **景気ウォッチャー, 家計調査, 商業動態統計, 景気動向指数** | Monthly | Retail, services | 家計調査 is noisy; prefer 商業動態統計 and company monthly data. |
| **Japan trade (貿易統計)**: 上中旬 flash, full month; BOJ 実質輸出入 | Monthly | Exporters, trading houses, energy importers | Yen value mixes price, FX and volume; check volume indices and destination/commodity detail. |
| **ISM manufacturing / services**; S&P Global PMIs; regional Fed surveys | ISM mfg 1st business day, services 3rd business day | Industrials, materials, semis | 50 is a breadth line, not a recession line; look at new orders minus inventories, prices paid. |
| **US GDP** (BEA advance/2nd/3rd) | Quarterly | Broad | Use final sales to private domestic purchasers; inventories and net exports distort. |
| **US retail sales** (Census) | ≈mid-month | Retail, restaurants, autos | Nominal; use the control group and deflate. |
| **US housing** (starts, permits, new/existing sales, Case-Shiller, mortgage rates) | Monthly/weekly | Homebuilders, building products, banks | Existing sales are closings (lagged); mortgage lock-in suppresses turnover. |
| **Consumer sentiment** (Michigan, Conference Board, 消費者態度指数) | Monthly | Discretionary | Tracks price perception and politics more than actual spending. |

### B6. Credit and financial conditions

| Item | Frequency | Sectors | Misreading to avoid |
|---|---|---|---|
| **IG / HY credit spreads (OAS)** | Daily | Banks, REITs, leveraged companies, energy | Tight spreads ≠ safety; check defaults, CCC vs BB dispersion and private credit. Free historical series may be shortened (e.g. FRED's ICE series limited to recent years). |
| **Financial conditions** (NFCI, VIX, MOVE), Fed SLOOS, BOJ loan surveys and 貸出・預金動向 | Weekly/quarterly/monthly | Banks, cyclicals | Look at changes, not levels. SLOOS measures lending standards (supply), not demand. |

### B7. Commodities, power and shipping

| Item | Frequency | Sectors (+/−) | Misreading to avoid |
|---|---|---|---|
| **Crude (WTI/Brent)**, EIA weekly inventories, rig count, OPEC+ decisions | Daily/weekly | Upstream (INPEX, trading houses) +; airlines, chemicals, utilities, Japan trade balance − | Spot ≠ realized (lags, hedges); geopolitical premium can decay; check curve shape. |
| **Natural gas / LNG / power** (Henry Hub, JKM/TTF, JEPX); **燃料費調整制度** | Daily/weekly/monthly | Utilities, gas, trading houses, chemicals | Japan fuel-cost adjustment uses a lagged multi-month average of fuel prices, creating timing gains/losses (期ずれ). LNG contracts are often oil-linked with lags. |
| **Copper, gold, iron ore, coking coal** | Daily | Copper: cable/wire, smelters, trading houses; gold: inverse to real yields; iron ore/coal: steel, trading houses | Exchange-specific distortions (tariffs, stockpiling). Price changes of different commodities can offset for diversified companies. |
| **Shipping** (container indices like SCFI/WCI, Baltic Dry, tanker rates) | Weekly/daily | Container lines (Japanese majors via their JV), dry bulk, importers | Spot indices cover a minority of volume; contract rates reset annually; route diversions drive rates. |

### B8. Asia early reads (lead indicators for JP/US tech and industrials)

| Item | Timing pattern | Read-across | Misreading to avoid |
|---|---|---|---|
| **Korea exports** (full month on the 1st; 1–10 and 1–20 day partials) | 3×/month | Semis (memory), SPE, components, autos | Working-day differences (holidays) swing y/y; memory price spikes inflate value. |
| **Taiwan export orders** (≈20th), Taiwan exports | Monthly | AI servers, semis, EMS | Orders include goods made abroad by Taiwanese firms; orders ≠ shipments. |
| **TSMC monthly revenue** (≈10th) | Monthly | Foundry, SPE, materials, AI supply chain | NT$ vs USD guidance; lumpy — compare quarterly totals to guidance. |
| **China**: official NBS PMI, private PMI (RatingDog, formerly Caixin), trade, credit (TSF), activity data | Monthly | Machinery, FA, machine tools, chemicals, cosmetics, luxury, inbound travel | Official PMI skews to large SOEs, private PMI to SMEs; credit impulse (change) matters more than level. Politics affect consumption of Japanese goods and travel. |

---

## Part C. Sector KPIs and industry statistics

For each sector: key KPIs, typical data sources and the most common mistake.
Company IR decks and earnings releases are the main source for company KPIs.

### Semiconductors & equipment
- **Industry:** global semiconductor sales (SIA/WSTS, 3-month moving average,
  ≈5-week lag); WSTS forecasts; SEMI global equipment billings (quarterly);
  SEAJ Japan-made equipment sales (3-month average, ≈3-week lag, 速報 then
  確定); DRAM/NAND contract and spot prices; TSMC monthly revenue; Korea/
  Taiwan exports; hyperscaler capex (from 10-Qs/earnings calls).
- **Company:** orders/backlog (受注残), book-to-bill, China share of sales,
  service revenue share, gross margin, inventory days, lead times.
- **Mistakes:** treating a 3-month average as a monthly print; mixing SEMI
  (global) with SEAJ (Japan-made); extrapolating price-driven memory revenue
  into unit demand; missing double ordering and inventory build near peaks;
  equating hyperscaler capex with chip demand (buildings, power, land are
  included); confusing orders, shipments and revenue recognition.

### Machinery (machine tools, construction equipment, FA)
- **Data:** 工作機械受注 (日本工作機械工業会, 速報 then 確報; 内需/外需),
  機械受注, 建設機械 shipments, robot orders (日本ロボット工業会), Komatsu
  KOMTRAX hours, Caterpillar dealer sales, China PMI.
- **Mistakes:** not separating price/mix/FX; treating large one-off orders as
  trend; orders vs sales timing; 速報 vs 確報 revisions; base effects.

### Autos
- **Data:** Japan new car sales (registered + kei, published on the 1st),
  OEM monthly global production/sales, US SAAR, incentives per vehicle, days'
  supply, average transaction price, hybrid/EV mix; tariffs; per-¥1 FX
  sensitivity; warranty costs.
- **Mistakes:** raw monthly units instead of SAAR; sell-in vs retail;
  volume growth read as margin growth while incentives and tariff absorption
  rise; ignoring mix; relying on domestic data for an export-driven profit
  pool.

### Retail & restaurants
- **Data:** company monthly 既存店売上 = 客数 × 客単価 (released early next
  month); 商業動態統計; department store, chain store, convenience store and
  restaurant association statistics; duty-free sales; US Census retail
  sales, comps (traffic vs ticket).
- **Mistakes:** price-driven comps hiding falling traffic; calendar/weather/
  promotion base effects; new-store growth mistaken for like-for-like;
  nominal vs real; lag between menu price increases and cost inflation.

### Software / SaaS
- **KPIs:** ARR, NRR/NDR, GRR, churn (解約率), RPO and cRPO, billings, Rule of
  40, SBC % of revenue, CAC payback, seat vs consumption pricing, AI
  monetization metrics.
- **Mistakes:** Rule of 40 with FCF that ignores SBC; RPO inflated by
  multi-year deals; differing NRR definitions; ARR ≠ revenue; ignoring seat
  compression from AI.

### Internet & advertising
- **KPIs:** paid clicks/CPC, impressions/price per ad, MAU/DAU, ARPU, take
  rate, GMV, traffic acquisition cost; Japan ad market statistics (電通
  「日本の広告費」 annual).
- **Mistakes:** mixing volume and price; ignoring FX and seasonal/political
  cycles; one platform's data extrapolated to the market; GMV vs revenue.

### Banks
- **Japan KPIs:** NIM, 預貸金利ざや, loan/deposit balances (日銀
  貸出・預金動向), 与信関係費用, capital ratios (international vs domestic
  standards treat unrealized securities gains/losses differently),
  その他有価証券評価損益, 政策保有株式 sales, deposit outflows, disclosed rate
  sensitivity.
- **US KPIs:** NII and NIM, deposit beta, loan growth (H.8), net charge-offs,
  ACL ratio, CRE exposure, CET1 and stress capital buffer, HTM/AFS
  unrealized losses, uninsured deposits, efficiency ratio.
- **Mistakes:** NIM expansion read as NII growth (volume matters); deposit-
  beta lag; one-off cross-holding sale gains as run-rate; low credit cost
  without checking reserve coverage; ignoring AOCI/capital regime.

### Insurance
- **Non-life:** combined ratio (loss + expense ratio), catastrophe losses,
  reserve development, rate increases, reinsurance renewals, 政策保有株
  reduction.
- **Life:** 新契約価値 (VNB), embedded value, economic solvency ratio (ESR;
  check the current regime status), 基礎利益, lapse rates, rate sensitivity,
  unrealized losses on bonds.
- **Mistakes:** P/E instead of EV/ESR for life insurers; low combined ratio
  from reserve releases or a benign catastrophe year; one-off gains from
  stock sales as earnings power.

### REITs
- **US:** FFO, AFFO (definitions vary), same-store NOI, occupancy, leasing
  spreads, implied cap rate, NAV premium/discount, debt maturities.
- **J-REIT:** 分配金 (DPU), 稼働率, 賃料改定, NAV倍率, 含み益, appraisal cap
  rate, NOI yield, LTV, DPU smoothing via gains on sale and reserves, spread
  to 10y JGB.
- **Mistakes:** applying US FFO logic to J-REIT DPU; assuming appraisal cap
  rates move with rates (they lag); ignoring dilution from equity issuance.

### Real estate (office, residential, developers)
- **Data:** Tokyo office vacancy and rents (monthly brokerage statistics;
  asking vs contracted), new supply schedules, new condominium data (price,
  契約率 with 70% benchmark), land prices (公示 in March, 基準地価 in
  September); US office occupancy, CMBS delinquencies, vacancy.
- **Mistakes:** asking rents as realized; ignoring incentives; ignoring
  submarkets; one-off sale gains counted as recurring profit.

### Utilities
- **Japan:** fuel-cost adjustment timing effects (期ずれ), nuclear restart
  status per plant, JEPX prices, capacity market, transmission charges, data
  center demand.
- **US:** rate base growth, allowed vs earned ROE, rate cases, capex plans,
  data-center load growth and interconnection queues, capacity auction
  prices, wildfire liability.
- **Mistakes:** timing gains read as earnings power; assuming nuclear
  restart savings flow to profit; allowed ROE ≠ earned ROE.

### Energy
- **KPIs:** crack spreads, refinery utilization, rig count, completions,
  production, inventories, OPEC+ spare capacity, LNG spreads, breakeven
  prices (e.g. Dallas Fed Energy Survey); Japan refiners' 在庫評価損益;
  upstream per-$1 sensitivity.
- **Mistakes:** rig count ≠ production; spot vs realized price after hedges;
  leaving inventory valuation effects in refiners' operating profit; ignoring
  cost inflation and windfall taxes.

### Materials & chemicals
- **KPIs:** product–feedstock spreads (ethylene–naphtha, etc.), utilization
  (domestic ethylene plants), crude steel production, iron ore/coking coal vs
  steel price, semiconductor materials utilization.
- **Mistakes:** product price up read as margin up; inventory valuation lag;
  treating structural Chinese overcapacity as cyclical; ignoring utilization
  breakeven.

### Pharma & biotech
- **KPIs:** pipeline by phase and indication, probability of success, PDUFA
  dates, advisory committees, trial readouts and medical congresses, loss-of-
  exclusivity dates, biosimilars, drug concentration; US drug pricing policy
  (Medicare negotiation schedule, tariffs — look up current status); Japan
  薬価改定 (annual) and 診療報酬改定 (biennial).
- **Mistakes:** peak sales without probability, pricing and LOE; surrogate
  endpoint wins treated as de-risked; PDUFA date treated as approval;
  milestone income as recurring.

### Trading houses (総合商社)
- **KPIs:** resource vs non-resource profit, disclosed commodity and FX
  sensitivities, equity-method income, shareholder returns, investment and
  asset recycling, net DER, guidance assumptions.
- **Mistakes:** spot commodity prices used for earnings (realized prices lag
  and are hedged); one-off gains/impairments as run-rate; equity-method lag.

### Shipping
- **KPIs:** container rates, dry bulk index, tanker rates, fleet growth and
  orderbook-to-fleet, diversions, ship prices; Japanese majors' equity income
  from their container JV; payout policy.
- **Mistakes:** spot index ≠ realized freight; disruption spikes treated as
  structural; ignoring newbuild deliveries.

### Airlines, rail, travel
- **Data:** 訪日外客数 (JNTO, ≈3rd week of next month, preliminary),
  outbound travelers, hotel occupancy/ADR/RevPAR, duty-free sales, airline
  traffic (RPK/ASK, load factor, yield, RASM/CASM), fuel and hedges, TSA
  throughput, rail passenger volumes.
- **Mistakes:** arrivals ≠ spending (market mix); high load factor with
  falling yield; one-off events in the base; fuel/FX; geopolitical
  disruptions of specific routes.

### Telecom
- **KPIs:** ARPU (definitions differ), churn, net adds/MNP, subscriber
  statistics (総務省 quarterly), capex/FCF, regulatory price pressure; US
  postpaid phone net adds, broadband and fixed wireless.
- **Mistakes:** ARPU growth from mix/non-telecom revenue; promotional lock-
  ins; comparing ARPU across carriers with different definitions.

### Gaming & entertainment
- **KPIs:** title sales, MAU/ARPPU, net bookings vs revenue, installed base
  and attach rate, digital ratio, capitalized development cost, IP licensing.
- **Mistakes:** sell-in vs sell-through; hit-driven quarters extrapolated;
  ignoring capitalized cost amortization; single-title concentration.

### Construction
- **Japan:** 建設工事受注動態統計, contractors' 受注高, 手持ち工事高,
  完成工事総利益率, labor and material costs, overtime regulation since
  2024, demand from redevelopment, semis and data centers, public works.
- **US:** architecture billings, Dodge Momentum Index, construction spending,
  backlog indicators, data-center construction.
- **Mistakes:** orders read as revenue; ignoring low-margin legacy backlog;
  lumpy mega-projects; cost overruns hidden in margins.

### Staffing / HR
- **KPIs:** job-offers ratio, new job postings, dispatched-worker hourly
  wages, headcount, bill rates, gross margin, placement fees, minimum wage
  revisions (October in Japan); US temp-help employment, JOLTS, job postings.
- **Mistakes:** falling ratios read as weak demand when supply shrinks;
  price renegotiation lag vs wage cost.

### Healthcare services
- **Japan:** 診療報酬 (biennial) and 介護報酬 (triennial) revisions, bed
  occupancy, prescriptions and dispensing fees, wage-related allocations.
- **US:** managed care medical loss ratio, cost trend, Medicare Advantage
  rate notices and Star ratings, risk adjustment, hospital admissions, payer
  mix.
- **Mistakes:** revision headline read as provider revenue growth; MLR
  improvement from repricing that hides membership loss.

---

## Part D. Cross-cutting data rules

1. Note whether a figure is seasonally adjusted, annualized, nominal or real,
   preliminary or final, a moving average or a single month, and its base
   period.
2. Date the data by its reference period, not just the release date. Asian
   lead indicators (TSMC, Korea, Taiwan) often lead Japanese/US equipment and
   component results by 1–3 months.
3. Policy and methodology changes (subsidies, waivers, tax, shutdown gaps,
   survey redesigns, index renamings) cause breaks; check before comparing.
4. Seek at least two independent confirmations for an industry call (e.g.
   Korea exports + TSMC + SEAJ for semis; Tankan + 機械受注 + 工作機械受注 for
   capex).
5. Do not rely on a single secondary headline; reopen the primary table for
   definitions and revisions when the number matters.
