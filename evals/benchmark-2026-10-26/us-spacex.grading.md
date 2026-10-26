# Grading: us-spacex ("How has SpaceX stock done since its IPO, and what should I watch for with the lockup expirations?")

Grader: blind, text-only. Today is 2026-10-26. Criteria G2–G10, G12, G13 per bench-rubric v0.4.0.

Cross-answer context (used only to judge substance, not as ground truth): four answers (B, C, E, F) place the 28% (~1.3B share) earnings-linked tranche on Oct 22, two trading days after Q3 results. E and F both report an Oct 22 close of $144.75 (-9.1%). A treats the timing of that tranche as unknown and possibly still ahead. D found no price after Oct 20. For a question asked on Oct 26, the main test is whether the answer caught the largest unlock to date, which had just happened.

---

## A

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers business segments, Q2/Q3 results, Q2 LSEG consensus, market cap and a target, capex and cash, ownership (Musk 48.4%), lock-up catalysts, Tesla and space peers, news, price path and risks. |
| G3 Data dating | PASS | Price table has a source column for each row ("Aug 4 \| Close $125.33 \| ... \| MoneyWeek (Aug 5)"), and the undated 52-week low is explicitly left out. |
| G4 Expectations hygiene | PASS | "above the $6.9B LSEG consensus"; "no Q3 consensus"; flags the guidance conflict: "TeslaNorth says the release gave no numeric guidance, while Financial Modeling Prep says ... $33B to $37B". |
| G5 Disconfirmation | PASS | "Strongest case against the conclusion ... the largest release so far was absorbed without a sell-off". |
| G6 Contradictions | PASS | "Strong quarter, flat stock"; "The feared unlock wave did not appear"; "Revenue beat, stock fell". |
| G7 Related companies | PASS | Tesla "Possible combination partner"; Rocket Lab, AST SpaceMobile, EchoStar "Space-sector peers". |
| G8 Catalysts | PASS | Dec 8, 2026 day-180 release; Jun 12, 2027 Musk unlock; Feb–Aug 2027 tranches. |
| G9 Next steps | PASS | Five tagged investigations, including "[disconfirm] Pull daily closes and volume for SPCX from Oct 20 to Oct 26, against Nasdaq and Tesla". |
| G10 Honesty about gaps | PASS | "Not retrieved: Q3 operating cash flow, Q3 consensus, short interest, borrow cost, options data, current float". |
| G12 Market context | FAIL | Moves are discussed but never benchmarked: "no index or peer benchmark was retrieved, so none of the moves above are market-adjusted". |
| G13 Internal consistency | FAIL | "The low point I found was a close of $125.33 on Aug 4", yet its own table has Aug 5 "Opened more than 10% lower", which implies a lower price that the answer ignores. Lock-up arithmetic gives "about 7% at day 180" next to "~800M" in the table; the answer flags this but does not reconcile it. |

**U = 6.** Strengths: very careful sourcing, with conflicts and gaps documented honestly; a solid disconfirmation section; a strong next-steps list. Weaknesses: it misses that the 28% (~1.3B) tranche unlocked on Oct 22, so its headline advice ("Watch the Q3-linked release first") is out of date on the question's central point; it misses the early-August low (~$105–108) and the Oct 22 -9% move; it has no market-adjusted context.

---

## B

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS (thin) | Covers business segments, Q3 results, liquidity and capex, analyst views (Morgan Stanley, Morningstar), Musk ownership, lock-up calendar, price path, volume and risks. No related companies, macro or positioning. |
| G3 Data dating | FAIL | Prices are dated, but individual figures carry no source ("Average daily volume is roughly 100M shares" has neither date nor source). All sources sit in a list at the end. |
| G4 Expectations hygiene | FAIL | Says "no numeric guidance in the release" but never gives Q3 consensus or says it is missing. It calls the report "strong" with no expectations baseline. |
| G5 Disconfirmation | FAIL | No counter-argument to its own conclusion ("The lockup overhang is unusually large"). |
| G6 Contradictions | PASS | "Morningstar cited 455.8M shares for August 20. That figure matches the unmet price-bonus tranche, not the August 20 release". |
| G7 Related companies | FAIL | Names no related companies (Tesla, peers, suppliers). |
| G8 Catalysts | PASS | Dec 8, 2026; Mar 18, 2027; May 17, 2027; Jun 12, 2027. |
| G9 Next steps | FAIL | The "What to watch" items are monitoring cues, not investigations, and none is aimed at disproving the conclusion. |
| G10 Honesty about gaps | PASS | "I could not verify the October 22 close directly"; "I could not confirm trading outcome". |
| G12 Market context | FAIL | Moves such as the "Up more than 12% intraday" are never compared with an index or peers. |
| G13 Internal consistency | FAIL | "The float is about 280M shares, and the schedule roughly triples it over time" conflicts with its own "roughly 12.85 billion shares eligible by mid-2027", which is far more than triple. It also says it "could not confirm" the Oct 22 outcome, then asserts "The October 21 rally faded into the October 22 unlock". |

**U = 5.** Strengths: a full, clearly typed lock-up calendar through mid-2027 (earnings-triggered, fixed-date, price bonus); sensible "eligible does not mean sold" and volume cues. Weaknesses: little analytical depth (no market context, no counter-case, no related companies); figures are not sourced individually; the float arithmetic is internally inconsistent.

---

## C

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers all 14 lenses in substance, including earnings quality, dilution, short interest, index inclusion, FOMC and related parties. |
| G3 Data dating | PASS | Dated and sourced figures ("S&P 500 closed 7,431.46 that day", "(Stocktwits, Jun 12)", "Q3 13F due about Nov 16"); undated short interest is flagged: "early August (undated)". |
| G4 Expectations hygiene | PASS | "diluted EPS $0.35 (consensus $0.15, from one aggregator)"; "No company guidance"; Q4 capex is labelled "reportedly signalled ... (secondary)". |
| G5 Disconfirmation | PASS | "The best evidence against that is that none of the large price moves was clearly lock-up-driven." |
| G6 Contradictions | PASS | "Record quarter, flat week"; "Net income above operating income"; "Unlock supply has not behaved like supply." |
| G7 Related companies | PASS | Tesla "Affiliate, possible merger partner"; Rocket Lab "Competitor"; Valor "3.4% holder and AI hardware lessor (related party)". |
| G8 Catalysts | PASS | Oct 27–28 FOMC; Dec 8 unlock; Dec 8–9 FOMC; ~Jun 12, 2027 Musk unlock. |
| G9 Next steps | PASS | Five tagged items, including "[disconfirm] Price reaction on Oct 22–23 relative to the Nasdaq and Tesla". |
| G10 Honesty about gaps | PASS | "I could not find the Oct 22 and 23 closes or the index moves for those days, so whether the unlock caused this is a hypothesis." |
| G12 Market context | PASS | "Oct 21 ... +7.8% to +11%, versus S&P +0.6% and Nasdaq +1.1%"; "S&P 500 +4.4% (Jun 12 to Oct 21)"; "The S&P 500 fell only about 2% over the same stretch". |
| G13 Internal consistency | PASS | The derived closes chain correctly (~$108 → +6.1% → $114.92 → +15.8% → ~$133). Cumulative float figures (4.5B, then 5.3B after Dec 8) reconcile. One minor rounding issue: "roughly 7-fold" where the stated numbers imply about 8x. |

**U = 8.** Strengths: the best fundamental read of any answer (net income above operating income from related-party other income and a tax benefit, roughly -$35B free cash flow, Cursor dilution); clear market-relative context; a well-reasoned counter-case and scenarios. Weaknesses: it could not get the Oct 22 close, so the most important unlock's reaction is left as a hypothesis; the 2027 extended tranches are not broken out; the answer is dense.

---

## D

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers Q3 results, expectations, valuation (101x revenue, analyst targets), positioning (short interest), insiders (Shotwell), catalysts, price path, volatility, float and risks. |
| G3 Data dating | FAIL | Sources are not tied to figures, and positioning data is undated: "Short interest fell from over 36% to about 16% of tradable shares". |
| G4 Expectations hygiene | PASS | "Revenue was $14.58B ... against about $12.7B to $13B expected"; analyst targets are dated "in August and September". Guidance and consensus are not conflated. |
| G5 Disconfirmation | FAIL | No strongest counter-argument is presented. |
| G6 Contradictions | PASS | "In August the stock rose through the first big unlock, helped by a short squeeze"; "The Motley Fool article's price box and text were inconsistent." |
| G7 Related companies | FAIL | None named. |
| G8 Catalysts | PASS | Oct 26 tranche; Dec 8; about June 2027 Musk tranche. |
| G9 Next steps | FAIL | The watch list has no structured investigations and none aimed at disproving a conclusion. |
| G10 Honesty about gaps | PASS | "I could not find a price for any session after Oct 20, so I don't know how the stock reacted". |
| G12 Market context | FAIL | Moves (-17% Jun 23, -14% Aug 5, +15.8% Aug 7) are never compared with an index or peers. |
| G13 Internal consistency | FAIL | It puts the low in "Mid-July ... The 52-week low of about $104.83 came during the post-IPO sell-off", but its own Aug 7 row ("The week closed at $133.11, up about 26%") implies the low came in early August. |

**U = 4.** Strengths: candid about missing post-Oct 20 data; flags the Oct 22 tranche as the key thing to check; useful notes on short interest and float. Weaknesses: no data after Oct 20, so it cannot answer "how has it done" for the most important week; it misdates the low; it has no counter-case, no market context and no related companies.

---

## E

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS (thin) | Covers business segments, Q2/Q3 results, analyst targets, Musk ownership and Class B, insider filings, lock-up catalysts, Tesla merger, leveraged ETFs and price path. No macro or positioning. |
| G3 Data dating | FAIL | Figures carry dates but no per-figure source; sources appear only in a list at the end. |
| G4 Expectations hygiene | FAIL | "Rallied on a Q3 beat" gives no consensus figure and does not say consensus is missing. |
| G5 Disconfirmation | FAIL | No counter-case to its bottom line ("the Q4 earnings unlock is the date to plan around"). |
| G6 Contradictions | PASS | "Aug. 6 went well, with a strong report and a +6% day. Oct. 22 went badly: a strong report, then a −9% day". |
| G7 Related companies | PASS (thin) | Tesla, possible merger partner ("Both boards have special committees"). |
| G8 Catalysts | PASS | Dec 8; Mar 18, 2027; May 17, 2027; Jun 12, 2027; Tesla's December annual meeting. |
| G9 Next steps | FAIL | Watch items only; nothing is aimed at disproving the conclusion. |
| G10 Honesty about gaps | FAIL | Few gaps are stated. It attributes the Oct 22 drop to "holders took profits" with no evidence or market check, and it sizes the Q4 tranche at "roughly 1.5B shares" with no source. |
| G12 Market context | FAIL | The Oct 22 -9% is reported with no index comparison (other answers note the Nasdaq fell 2.6% that day). |
| G13 Internal consistency | FAIL | The short version says "The heaviest part of the lockup schedule is now behind it", but section 3 calls the Q4 tranche "the big one ... larger than any release so far". Its extended group "about 7.8B shares" includes Musk, yet it says "Musk's own lockup ends" on June 12, while sizing the Q4 tranche at 20% of that group. |

**U = 5.** Strengths: has the actual Oct 21 and Oct 22 closes and the day-by-day reaction to each unlock; covers the Tesla merger as a factor that could change the lockup picture; readable, with a clear bottom line. Weaknesses: its central recommendation rests on a Q4 tranche size (~1.5B) that appears to fold in Musk's separately locked shares and conflicts with its own description; the summary contradicts the body; the Oct 22 drop is attributed without market context.

---

## F

| Criterion | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers all lenses, including capital policy ($40B debt, equity issuance language), positioning, macro, sector data and S&P eligibility. |
| G3 Data dating | PASS | "short interest at 219.3M shares, about 34% of float, as of Jul 29 (Bloomberg Law, Jul 31)"; prices "from StockAnalysis daily history; index moves are from AP index tables". |
| G4 Expectations hygiene | PASS | "against a consensus of about $12.7–13.0B (sources differ)"; "Management guided ... Q1 2027 revenue to $33–37B ... TIKR puts the Street's prior expectation at about $22.2B"; "EPS and capex consensus not found". |
| G5 Disconfirmation | PASS | "The Oct 22 drop may have been mostly a market move ... In the other direction, the real overhang may not be the lockup at all but issuance". |
| G6 Contradictions | PASS | "Big beat, then −9.1% the next day"; "Profitable on paper, but heavy cash burn"; "Q1 2027 revenue guide of $33–37B against Q3 revenue of $14.6B". |
| G7 Related companies | PASS | Tesla "Same controlling shareholder; possible merger"; Nvidia "GPU supplier"; CoreWeave "Peers in AI compute"; Cursor "Acquired company". |
| G8 Catalysts | PASS | Oct 27–28 FOMC; Dec 8; mid-Dec index reconstitutions; Q4 results plus tranche; Jun 12, 2027. |
| G9 Next steps | PASS | Five tagged items, including "[disconfirm] Was Oct 22 about the unlock or the market? ... Pull Oct 22 closes for TSLA, NVDA, CoreWeave". |
| G10 Honesty about gaps | PASS | "I did not find operating cash flow"; "A headline claiming a fall to 11% could not be read or dated, so I left it out." |
| G12 Market context | PASS | Earnings-week table: "Oct 22 \| $144.75 \| −9.1% \| 194M \| Nasdaq −2.6%, S&P 500 −1.2%"; "excess drop of roughly 6.5 points". |
| G13 Internal consistency | PASS | Percentages reconcile ($147.49 is +9% vs IPO, -8% vs the first-day close, -35% vs the peak, +41% vs the low). The Dec 8 size conflict (342M vs 797.6M) is surfaced and reasoned through (342M + 455.8M ≈ 797.8M) rather than stated two ways silently. |

**U = 9.** Strengths: the only answer that both has the Oct 22 unlock reaction and adjusts it for the market (-9.1% vs Nasdaq -2.6%); sizes each tranche against average volume (1.3B ≈ 14 days); reframes the overhang toward issuance (capex, $40B debt, a possible stock-funded Tesla deal) with a strong counter-case. Weaknesses: it relies mostly on secondary sources for results and lockup terms; it presents the Q1 2027 revenue guide as fact although another source reportedly says there was no numeric guidance (it does flag this for verification); Musk's stake appears as "~42% by value" in one place and as ~6.4B of 13.58B shares (~47%) elsewhere, which is not reconciled.

---

## Ranking

1. **F**: complete and well sourced; the only answer with a market-adjusted read of the Oct 22 unlock.
2. **C**: equally rigorous, with the best earnings-quality analysis; it lacks the Oct 22 close.
3. **A**: honest and well structured, but it missed that the 28% tranche had already unlocked on Oct 22, so its main watch item is out of date.
4. **E**: has the key Oct 22 data, but its bottom line rests on an internally inconsistent tranche sizing and gives no market context.
5. **B**: good lock-up calendar, thin analysis, inconsistent float arithmetic.
6. **D**: no data after Oct 20, a misdated low and no analytical scaffolding.

```json
{"A": {"pass": 9, "applicable": 11, "U": 6}, "B": {"pass": 4, "applicable": 11, "U": 5}, "C": {"pass": 11, "applicable": 11, "U": 8}, "D": {"pass": 5, "applicable": 11, "U": 4}, "E": {"pass": 4, "applicable": 11, "U": 5}, "F": {"pass": 11, "applicable": 11, "U": 9}, "rank": ["F", "C", "A", "E", "B", "D"]}
```
