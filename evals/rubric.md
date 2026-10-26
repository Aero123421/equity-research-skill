# Grading rubric (iteration 1)

Score each assertion PASS/FAIL with a one-line evidence quote or reason.

## Generic (all cases)
- G1 Coverage: the answer explicitly shows which research lenses were checked / partial / not found / not relevant (a coverage table or equivalent list covering at least 10 distinct lenses).
- G2 Lens breadth: the answer contains substantive content from at least 8 of these: business, results quality, expectations (guidance/consensus), valuation, capital policy, positioning (short/margin/options), ownership/insiders, catalysts calendar, related companies, macro, sector data, news/sentiment, price action, risks.
- G3 Data dating: lagged positioning data (short interest, margin balances, 13F etc.), if cited, includes an as-of date; key numbers carry a period/date and source.
- G4 Expectations hygiene: company guidance/forecast and analyst consensus are not conflated (if either is mentioned, they are labelled distinctly; if consensus not found, this is said).
- G5 Disconfirmation: the answer explicitly presents the strongest counter-argument to its main conclusion.
- G6 Contradictions: the answer identifies at least one tension/contradiction between different data points and discusses it.
- G7 Related companies: related companies are named with a relation type (competitor, customer, supplier, etc.), not just a list.
- G8 Catalysts: at least two dated upcoming events relevant to the stock/theme are listed.
- G9 Next investigations: 3+ prioritized next steps, at least one explicitly aimed at disproving the thesis.
- G10 Honesty about gaps: missing/unavailable data is stated as missing rather than filled with unsourced numbers.

## Case-specific
### us-earnings-tesla
- T1 Separates the quarter's actuals vs consensus for at least revenue and EPS, with basis (GAAP vs non-GAAP) stated.
- T2 Explains the price reaction with more than one driver (e.g., guidance/margins plus positioning/narrative/macro), and states the size and timing of the move.
- T3 Mentions read-across from or to peers/suppliers (e.g., other EV makers, battery suppliers).

### us-short-smci
- S1 Gives short interest with both % of float (or shares) and days to cover, plus the settlement date.
- S2 Distinguishes short interest from daily short volume or explains data lag.
- S3 Considers non-directional reasons for shorts (e.g., convertible-bond hedging) or borrow cost/utilization (or states unavailable).
- S4 Squeeze verdict is conditional, checking at least 3 squeeze conditions (float short, days to cover, borrow, catalyst, options, etc.).

### jp-deep-dive-lasertec
- L1 Gives 信用買い残/売り残 or 信用倍率 with as-of date.
- L2 Mentions 空売り残高報告 (institutional short positions) or explicitly says checked/not found.
- L3 Distinguishes company forecast (会社予想) vs consensus, and/or computes 進捗率.
- L4 Discusses customers/competitors (e.g., EUV ecosystem, chipmakers, KLA etc.) with relation types.

### theme-dc-power
- P1 Covers both Japanese and US companies across at least 3 value-chain layers.
- P2 Distinguishes verified exposure (with evidence such as segment revenue/orders) from mere association.
- P3 Notes what is priced in (valuation/performance) and at least one risk or potential loser.

## Added in iteration 2 (apply to all iteration-2 runs; also apply to iteration-1 with_skill runs for comparison)
- G11 Targeted disconfirmation: the counter-argument section argues against the answer's own headline conclusion (not a generic bull/bear).
- G12 Market context: when a price move is discussed, the move is compared with the index and/or peers on the same day(s).
- G13 Internal consistency: rankings, coverage statuses and figures are consistent across sections (no row says "see below" pointing nowhere; no figure stated two different ways).

### quick-jp-margin-fujikura
- F1 Gives 信用買い残, 信用売り残 and 信用倍率 with the 申込日 (as-of) and source.
- F2 Notes which series is used (weekly vs daily since 2026-09-28) or the data lag.
- F3 Adds an "also worth knowing" block drawing on at least 2 other lenses (e.g., price move, catalyst, 貸借/逆日歩, 空売り残高).
- F4 Concise: answer body (excluding sources) under ~2,500 Japanese characters.

### us-price-move-nvda
- N1 Quantifies the move with start/end dates and prices.
- N2 Compares with an index and peers over the same window.
- N3 Separates sector/market-wide drivers from company-specific ones.
- N4 Presents a credible alternative explanation as the counter-argument.
