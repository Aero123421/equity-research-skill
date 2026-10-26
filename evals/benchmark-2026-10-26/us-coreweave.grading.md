# Grading: us-coreweave ("What's going on with CoreWeave? Is the bond selloff a warning sign for the stock?")

Grader date: 2026-10-26. Graded from the text only (no web checks). Rubric: bench-rubric.md v0.4.0 (G1 excluded).

Consistency rules I applied across answers:
- G3: a key-figure table with no source attached (neither per-row nor table-level) fails, even if a reference list appears at the bottom.
- G4: passes only if guidance and consensus are kept apart AND the answer either gives a consensus estimate or says it is missing. Analyst price targets alone do not count as consensus.
- G8: needs at least two events with a specific date (or a specific week). "In November" / "mid-November" alone does not count.
- G9: a "what to watch" list of monitoring items does not count as next investigations unless at least one is framed as a test that could disprove the answer's conclusion.
- G12: needs a quantified comparison with an index, sector or peers.

---

## Answer A

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Coverage spans business, results, expectations, valuation (EV ≈ $76B, ~6x revenue), capital policy (ATM 35M shares, $3.7B converts), positioning (SI 59.95M, Sep 30), insiders, catalysts, related cos, macro, sector (Gartner), news, price, risks. |
| G3 Data dating | PASS | "Short interest 59.95M shares (Sep 30 settlement, published Oct 9)"; "On Oct 14, the 9.625% notes due 2032 traded at about 79.5¢ ... (TIKR)". |
| G4 Expectations hygiene | PASS | "Company Q3 and FY guidance found. Q3 consensus EPS of −$1.70 is a single estimate (MarketBeat), so not a reliable consensus." |
| G5 Disconfirmation | PASS | "Strongest case against this conclusion: 'The bond selloff is noise, not a warning'", incl. Nebius falling almost as much, risk-neutral CDS caveat, secured IG debt. |
| G6 Contradictions | PASS | "Revenue doubled but Q2 operating cash flow fell 77% q/q ... Open, and it matters."; CEO "irrational" vs steady selling. |
| G7 Related companies | PASS | Table: Nvidia "Supplier, ~10% holder, buyer of unsold capacity"; Nebius "Competitor"; OpenAI/Meta/Microsoft "Customers". |
| G8 Catalysts | PASS | "Oct 27–28 FOMC ... Confirmed"; "~Nov 9 Q3 results Estimated"; "Nov 10 October CPI". |
| G9 Next steps | PASS | Five items, incl. "[disconfirm] Q2 10-Q liquidity section ... If most is covered, the Bernstein gap is overstated." |
| G10 Honesty about gaps | PASS | "I found no bond prices after Oct 15."; "Borrow cost and options implied move not found." |
| G12 Market context | PASS | Table: CRWV −33.9% vs NBIS −28.2%, ORCL −10.8%, SMH −12.6%, QQQ −6.2% (Oct 9→23). |
| G13 Internal consistency | PASS | Spot checks hold: EV 30+51.6−5.5 ≈ 76; "10% fall in EV cuts equity ~25%" (7.6/30); "1.4–1.5× Nebius" (15.5/10.1, 10.1/7.2); FCF 0.68−6.4 ≈ −5.7. |

U = 9. Best balance of currency and rigor.
- Strengths: (1) The only answer that is current through Oct 23–26 and quantifies the funding need (Bernstein $85B/$76B gap, Morgan Stanley $24–37B), which is the most decision-relevant item. (2) Properly separates the sector/rate component from the company-specific component, using Nebius −28% vs CRWV −34% and index comparisons. This tempers its own headline. (3) Flags the Q2 operating cash flow collapse as an open, decision-relevant contradiction.
- Weaknesses: (1) It relies mostly on secondary sources; filings were not read directly (it says so). (2) The "$24–76B funding gap" merges two analysts' differently defined estimates into one range. (3) The bond prices are 11 days stale relative to the stock prices.

## Answer B

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Business/backlog, results, expectations (consensus EPS −$1.28, targets), ownership (Nvidia 10%), catalyst (Q3), peers, macro (CPI), sector (hyperscaler $228B bond issuance), news, price, risks. Thin, but ≥8. |
| G3 Data dating | FAIL | The fundamentals table gives periods but no sources. "The consensus target is about $140 across roughly 40 analysts" has no date or source. |
| G4 Expectations hygiene | PASS | "Q3 guidance: Interest expense of $860-940M ..." (company) vs "the consensus EPS estimate is about -$1.28" (analysts). |
| G5 Disconfirmation | PASS | "The bull case": $104B backlog, Nvidia backing, "Cantor says 'the market is getting it wrong.'" |
| G6 Contradictions | PASS | "The gap between price and consensus target has more than doubled since Sept 30, which tells you more about how stale the targets are than about upside." |
| G7 Related companies | FAIL | Only Nvidia gets a relation ("owns about 10%"). Oracle, Dell and Nebius are listed as same-day movers, and customers are unnamed ("a small number of AI customers"). |
| G8 Catalysts | FAIL | Only one dated event: "Q3 earnings (about Nov 16, unconfirmed)". "A confirmed Fed hike" has no date. |
| G9 Next steps | FAIL | "Watch these things" are monitoring items (Q3, bonds/CDS, new financing, rates). None is set up as an investigation that could disprove the conclusion. |
| G10 Honesty about gaps | PASS | "Data as of roughly Oct 19, 2026. I found no reliable coverage after that ... figures come from secondary sources ... I couldn't verify." |
| G12 Market context | PASS | "Oracle fell about 9%, Dell about 11% and Nebius about 10% on the same day" vs CRWV −15.5%. |
| G13 Internal consistency | PASS | No contradictory figures found. The GAAP operating loss vs adjusted income is labeled explicitly. |

U = 5.
- Strengths: (1) Clear, correct core mechanism: fixed coupons, the marginal cost of new debt, and equity as the residual. (2) Honest about how stale and how secondary its data is.
- Weaknesses: (1) Stale by a week. It misses the Oct 22 leg to ~$55, Bernstein/Morgan Stanley on funding size and the Musk post. (2) No funding-gap quantification, positioning or valuation. (3) Weak catalyst and next-step structure.

## Answer C

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS (marginal) | Results, expectations (guidance, targets), business/backlog, peers, macro (CPI/Fed), news/sentiment (CEO, analysts), price, risks, ownership (Nvidia stake), catalyst (Q3). No valuation, positioning or capital policy. |
| G3 Data dating | PASS | "Total debt, June 30, 2026 ..."; "Sources for the table: TIKR, ROIC, Investinglive"; "on October 14"; "on October 15". |
| G4 Expectations hygiene | FAIL | Gives company guidance and analyst targets but never mentions consensus estimates or that they are missing. |
| G5 Disconfirmation | PASS | "Why it may be overdone": backlog, sector-wide move, bullish analysts. |
| G6 Contradictions | PASS | "Sources disagree on the October 16 move (about -6.9% per ROIC, about -12% per TIKR)"; targets "do not reflect the credit market's view." |
| G7 Related companies | PASS (marginal) | "Nvidia, which owns a stake and is a major customer"; "Concern ... spread to peers: Nebius, Applied Digital and Iren". (Calling Nvidia a "major customer" is questionable.) |
| G8 Catalysts | FAIL | "Q3 results, due in November" is the only catalyst. No dated events. |
| G9 Next steps | FAIL | "What to watch" is a single list of things to monitor, with no investigations and no disconfirmation test. |
| G10 Honesty about gaps | PASS | "the most recent reporting I could find runs through about October 16, 2026. I found nothing from the last ten days". |
| G12 Market context | FAIL | Peers are said to have "fell" with no magnitudes, and there is no index comparison, so the relative move cannot be judged. |
| G13 Internal consistency | PASS | No figure is stated two ways. Note the analytically meaningless "interest ($640M) was more than ten times the operating loss ($49M)". |

U = 4.
- Strengths: (1) Concise, correct framing of backlog vs cash conversion. (2) A good data-definitions note on debt with vs without leases.
- Weaknesses: (1) The most stale answer (data to Oct 16). It misses the further ~10% decline and all the funding-gap analysis. (2) No valuation, positioning, catalysts or investigation plan. (3) A confused "ten times the operating loss" ratio and a questionable "Nvidia ... major customer" label.

## Answer D

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | All 14 lenses addressed, with valuation (EV ~$60B, 4.7x), capital policy, insiders ($472M sold), macro, sector and risks. |
| G3 Data dating | PASS | "Closes: Oct 9 $82.08 ... Oct 23 $54.24 (StockAnalysis, cross-checked: MarketBeat)"; "Balance sheet at 2026-06-30 ... (IR release)". |
| G4 Expectations hygiene | PASS | "Company guidance found; consensus vs actuals not found; analyst targets only". |
| G5 Disconfirmation | PASS | "The warning may be overdone ... Or it may be understated", with a settling test: "a new financing at spreads at or inside August's +550 over SOFR". |
| G6 Contradictions | PASS | "Falling average cost of debt vs wider new loans. Both are true: older, cheaper debt rolls into more expensive marginal debt." |
| G7 Related companies | PASS | Table: Nvidia "Supplier, ~10% holder"; Oracle "Same-theme ... not a direct competitor"; Nebius "Direct neocloud peer"; Microsoft/Meta/OpenAI "Customers". |
| G8 Catalysts | PASS | "Oct 27-28 FOMC confirmed"; "Dec 8-9 FOMC"; "about Nov 10 Q3 estimated"; "By end-2026 ... DSCR covenant ≥1.35x". |
| G9 Next steps | PASS | "[disconfirm] Are the bonds mispriced? Read Q2 10-Q debt note and the 8-Ks filed Oct 14 and Oct 22", plus 4 more. |
| G10 Honesty about gaps | PASS | "Aggregators show roughly 17-18% of float short but give no settlement date, so I excluded the figure"; "The cause of Oct 22's -10.1% was not found." |
| G12 Market context | PASS | "CRWV -25.2% ... vs S&P 500 -1.95%, Nasdaq -4.48%"; Oct 16 "SOX -3.8% ... vs CRWV -11.9%"; peer moves on Oct 14. |
| G13 Internal consistency | FAIL | The Answer says the drop was "roughly 6x the S&P 500's weekly decline during the first leg", but its own data (−25.2% vs S&P −1.95%) gives ~13x. About 6x is the Nasdaq ratio (−4.48%). |

U = 8.
- Strengths: (1) The key analytical insight that marginal loan spreads widened deal by deal (+225 → +450 → +550) even as the average cost fell, plus a concrete test (the next deal vs +550). (2) Uses the company release over conflicting secondary data (capex $6.4B vs $9.4B), with careful own-calculation labels (H2 external need ~$17–20B). (3) Current price data through Oct 23, plus a dated covenant catalyst.
- Weaknesses: (1) The "6x the S&P" misstatement. (2) It attributes "most of the move" to company-specific factors without comparing Nebius over the full period, which other evidence suggests fell almost as much. (3) It misses the Bernstein/Morgan Stanley funding-gap notes and the Oct 25 Musk post, though it admits the search budget ran out.

## Answer E

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Market move, bonds/CDS, balance sheet, backlog/customers, positioning, macro, related cos, catalysts, scenarios, risks, news. |
| G3 Data dating | PASS | "Short interest was 59.95M shares at the Sep 30 settlement ... (Equibles)"; "Balance sheet (10-Q, 6/30/2026)"; numbered source list with dates. |
| G4 Expectations hygiene | PASS | "TIKR Q3 guidance unverified; no consensus table"; "Q3 interest guidance of $860–940M appears in TIKR, which labels it an estimate." |
| G5 Disconfirmation | PASS | "The best counter: much of the Oct 14 break was a rates shock ... What would confirm the counter: a Fed hold, the 2031 yield back below about 13% ..." |
| G6 Contradictions | PASS | "Stock and bonds moved together ... Same-day co-movement does not show that bonds lead." Five tensions are listed. |
| G7 Related companies | PASS | Table with relations: Oracle "AI-infrastructure peer ... (not verified as a CRWV customer)"; Nvidia "Shareholder ... GPU supplier"; hyperscalers "Competing AI-debt issuers". |
| G8 Catalysts | PASS | "Oct 26 FINRA short-interest publication"; "Oct 28, 2:00 PM ET FOMC decision"; "Nov 10 FINRA". |
| G9 Next steps | PASS | "[disconfirm] Read the Oct 15 short-interest settlement ..." plus verify/compare/fill_gap/monitor items. |
| G10 Honesty about gaps | PASS | "the search tool stopped after 11 searches ... news from Oct 20–26 is missing"; "I cannot translate either into a probability without a recovery assumption, so I do not." |
| G12 Market context | PASS | "CRWV fell 15%, against Nasdaq Composite -1.88%, the Philadelphia semiconductor index -4.3%, Oracle -8.8%, Nebius -10%". |
| G13 Internal consistency | PASS | Spot checks hold: 35.1/21.4 = +64%; 59.95/551.5 = 10.9%; 640/2,575 ≈ 25%; equity ~40% of $86.6B. Its CDS and 10-year conflicts are disclosed, not hidden. |

U = 7.
- Strengths: (1) The best use of primary filing data: customer concentration (72% from three customers, 32%/32% of receivables), RPO timing (41% within 24 months) and the H1 cash gap of $10.5B vs $14.0B net financing. (2) An excellent hygiene section that reconciles conflicting CDS, yield, hike-odds and Treasury figures, and refuses unsupported probability conversions. (3) It challenges the popular "bonds lead stock" claim with its own evidence.
- Weaknesses: (1) Market data stops Oct 19, so the price anchor (~$63) is ~15% above the latest close. It misses the Oct 22 drop, Bernstein's funding-gap note and the Musk post. (2) No valuation multiples and no funding-need estimate for H2.

## Answer F

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Business, results, expectations (guidance, targets), valuation (mkt cap < debt), capital policy (ATM, converts), ownership (Nvidia 10%), catalysts, related cos, macro, news, price, risks. |
| G3 Data dating | FAIL | The table has no sources for "External funding still needed in 2026 ~$20–25B (estimate)", "Debt due by end-2027 ~$10.6B" or "Top 3 customers = 72%". "A Meta-backed tranche priced at 5.9% in July" is also unsourced. |
| G4 Expectations hygiene | FAIL | Company "Q3 guide" and a "mean target, about $140" appear, but there is no consensus estimate and no statement that one is missing. |
| G5 Disconfirmation | PASS | "The other side: if Q3 shows adjusted operating income growing toward covering interest ... the gap between bonds and backlog could close fast." |
| G6 Contradictions | PASS | "On Oct 19 the bonds stabilized and the stock bounced, but it then broke to new lows"; a Goldman upgrade vs the bond ranking. |
| G7 Related companies | PASS | "OpenAI is a major CoreWeave customer"; Microsoft payments repay SPV loans; Nvidia "owns about 10% and has agreed to buy unsold capacity". |
| G8 Catalysts | PASS | "Oct 28 Fed decision, plus Microsoft, Meta and Alphabet earnings this week"; "Q3 earnings (mid-November)". |
| G9 Next steps | FAIL | "What to watch" is a monitoring list. The bond "all clear" level is a useful signal, but nothing is framed as an investigation to disprove the thesis. |
| G10 Honesty about gaps | PASS | "my search budget ran out, so I couldn't confirm the Oct 23 close or anything after it. The latest price I found was Oct 22." |
| G12 Market context | PASS | "Oracle, Nebius and Dell also fell 9–11% that day" vs CRWV −15.5%. |
| G13 Internal consistency | FAIL | "At about 30% of its 52-week high" conflicts with its own $56 price and ~$142 high (~39%). Elsewhere it says "well over 50% below". |

U = 6.
- Strengths: (1) Fairly current (Oct 22), and it adds the Oct 8 OpenAI-revenue trigger and the $2.6B "cash trap" loan. (2) Good structural points: SPV/contract-backed debt vs unsecured notes, the ATM program as the dilution path, and a concrete bond "all clear" threshold (85–90¢, CDS < 1,000bp).
- Weaknesses: (1) Several key numbers are unsourced or unexplained estimates (the $20–25B funding need, $10.6B maturities by 2027, the 5.9% Meta tranche). (2) An arithmetic slip on the distance from the 52-week high. (3) It asserts "the stock has been following the bonds" using same-day co-movement, which does not establish a lead.

---

## Ranking

1. **A**: current, comprehensive, quantifies the funding gap, separates the sector move from the company-specific one, and has no consistency errors.
2. **D**: strong analysis (marginal spread widening, a clear test) and current prices. One misstated ratio.
3. **E**: the most rigorous sourcing and primary filing data, but a week stale on prices and news.
4. **F**: current and insightful on structure, but weak on sourcing and has a numeric slip.
5. **B**: a correct core mechanism, but stale and thin.
6. **C**: the most stale and thinnest, with a confused ratio.

```json
{"A": {"pass": 11, "applicable": 11, "U": 9}, "B": {"pass": 7, "applicable": 11, "U": 5}, "C": {"pass": 7, "applicable": 11, "U": 4}, "D": {"pass": 10, "applicable": 11, "U": 8}, "E": {"pass": 11, "applicable": 11, "U": 7}, "F": {"pass": 6, "applicable": 11, "U": 6}, "rank": ["A","D","E","F","B","C"]}
```
