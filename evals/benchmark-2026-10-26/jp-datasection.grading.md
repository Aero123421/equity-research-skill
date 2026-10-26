# Grading — jp-datasection (データセクション 3905), as of 2026-10-26

User question: 「データセクション（3905）ってなんでこんなに話題なの？今後どうなりそうか調べて。」
I graded each answer from its text only, with no web checks. Where answers disagree on a fact, I note it. I don't treat one answer as ground truth.

Cross-answer factual tensions worth noting (unverified):
- **Contract term**:
  - A, C, D and F say "annual 1.752億ドル, 3 years (+2 extension)".
  - E says the same and states a total of 5.256億ドル.
  - B says "5年累計1,399億円" (citing the company release) and explicitly flags the conflict with the 3-year press reports.
- **Warrant expiry**:
  - A, C and E report that the 第23回新株予約権 exercise period expired on 10/19.
  - E adds that only about 271億円 of the planned 558億円 was raised (a shortfall of about 286億円) and cites the 10/19 TDnet PDF.
  - B misses the expiry and still models up to about 59% dilution from 2,260万 remaining potential shares.
- **Short interest**:
  - Only B finds the reported institutional shorts (Barclays/MS MUFG/GS, about 12% combined).
  - A concludes from margin sell balances alone that short covering does not explain the rally.

---

## A
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers business, FY/Q1 quality, company forecast, PER/PBR, warrants, margin balances, holder filings, catalysts, Sakura, FOMC/USDJPY, Sakura GPU data, news, price/liquidity and risks. |
| G3 Data dating | PASS | "信用残は10/16時点(株探)のみ"; "PER 8.4倍、PBR 2.94倍(株探、10/26、会社予想ベース)". |
| G4 Expectations hygiene | PASS | "会社予想は確認。コンセンサスは未取得(アナリストカバー不明)". |
| G5 Disconfirmation | PASS | Has a section 「この結論に反する最も強い見方」 (自己資本比率76.2%, 10月稼働開始, 3年契約, strong GPU demand). |
| G6 Contradictions | PASS | "「営業利益48億円のQ1」でも株価が大きく下がった"; "予想PER 8倍台なのに買い手が慎重だった". |
| G7 Related companies | PASS | Table lists さくらインターネット (競合), NVIDIA (供給元), the unnamed US customer (顧客) and the terminated hyperscaler (元顧客). |
| G8 Catalysts | PASS | FOMC 10/27–28, Sakura results 10/28, 2Q results 11/16. |
| G9 Next steps | PASS | 5 items, including "[disconfirm] 9/18「大口契約の締結に関するお知らせ」の原文を読む". |
| G10 Honesty about gaps | PASS | "10月26日のS高の理由は、今回の調査では特定できていません"; it marks secondary-source figures and the unread filings. |
| G12 Market context | PASS | "データセクション+26.1%…日経平均−0.80%…グロース250は続伸…さくらインターネット(3778)は+1.79%". |
| G13 Internal consistency | PASS | Figures are consistent. One minor dangling item: the data note discusses an "調整後EBITDA 582億円、経常利益125億円" choice that the body never uses. |

**U = 8**

Strengths:
- Correctly ties the rebound to two things: the 10/23 service-start disclosure, and the expiry of the 1,250円 fixed-price warrant on 10/19, at a time when the stock traded below the exercise price.
- Does a quantitative gap check. The 9/18 contract is worth about 270億円 a year, or about 17% of the 1,622億円 guidance, against the roughly 799億円 contract that was terminated.
- Gives the best market context, with the 10/26 Nikkei, Growth 250 and Sakura moves, plus a dated catalyst list.

Weaknesses:
- Misses the reported institutional short positions (about 12% per B). This weakens its claim "踏み上げ…で説明できる上昇ではありません", which rests on margin data alone.
- The actual amount raised from the warrant exercise is unknown. Several key Q1 numbers (88% one-off, the 740億円 gap) come from blogs.

## B
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers business, results, forecast, valuation (own PER calculation, diluted), capital policy, short-sale reports and margin balances, the FIRST PLUS/アースエレメンツ holding table, catalysts, related companies, FX/FOMC, news, price action and risks. |
| G3 Data dating | PASS | "Barclays 6.45%（10/21）…モルガン・スタンレーMUFG 3.36%（10/22）"; "信用残（10/16時点）". |
| G4 Expectations hygiene | PASS | "会社予想は確認。コンセンサスは見つからず（アナリストのカバーはほぼない模様）". |
| G5 Disconfirmation | PASS | Has a section 「この結論への最も強い反論」 (the 10/26 briefing, directional shorts causing a squeeze, warrant exercise ending). |
| G6 Contradictions | PASS | "大型案件が解約されたのに通期予想は据え置き"; "好材料が続いているのに株価は下がり続けた"; it also flags the 5-year vs 3-year contract conflict. |
| G7 Related companies | PASS | Lists the US customer (顧客), NVIDIA (供給元・仲介), ASRock Rack (調達先) and さくら (同業). |
| G8 Catalysts | PASS | FOMC 10/27–28, the remaining deposit (late October), 2Q 11/16 and FOMC 12/8–9. |
| G9 Next steps | PASS | 5 items, including "[disconfirm（反証）] 10/26の説明会の中身を確認する". |
| G10 Honesty about gaps | PASS | "10/26の上昇理由は特定できていません"; it notes that Q1 figures are secondary and that the 11/16 date is not confirmed by the company. |
| G12 Market context | PASS | "10/23の東証グロースは値下がり優勢（上昇167・下落387）、さくらは−1.73%". |
| G13 Internal consistency | PASS | The arithmetic checks out: 1,930円 × 38.42M = 741億; full dilution gives 1,178億. The term conflict is disclosed rather than hidden. |

**U = 8**

Strengths:
- Has the richest positioning and ownership evidence. The FIRST PLUS exercise-and-sell table and the rise in reported shorts from about 6% to about 12% convincingly explain why good news failed to stop the decline.
- Uses primary sources for the contract (9/18 release, the 10/23 service start, the 10/26 briefing) and confirms the 0.9855億ドル deposit receipt.
- Does a clear gap analysis: about 140億円 of revenue this fiscal year from the new contract, versus the 798.64億円 lost.

Weaknesses:
- Misses the 10/19 warrant expiry. As a result, its "最大約59%の希薄化余地" and "行使売りが一巡" framing may be stale. This is material to its forward view.
- Has no 10/26 index comparison; it only covers 10/23.

## C
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS (marginal) | Covers business, results quality (88% one-off), plan, capital/dilution, catalysts, news, price action and risks. Valuation (みんかぶ target only) and ownership ("開示一覧には…並んでいます") are thin. |
| G3 Data dating | PASS | Its timeline rows carry dates and links, e.g. "5月8日…([カブタン]…、[同社IR]…)". |
| G4 Expectations hygiene | FAIL | Never addresses consensus. A みんかぶ target of 819円 is cited without distinguishing it from analyst consensus. |
| G5 Disconfirmation | FAIL | Has only generic 強気/弱気 lists and no counter-argument to its own conclusion. |
| G6 Contradictions | PASS | "計画は据え置いたものの、計画の土台だった契約が解除されています". |
| G7 Related companies | FAIL | Compal and ASRock Rack appear only incidentally as purchase sources. There is no related-company analysis or peer. |
| G8 Catalysts | FAIL | Gives only "2026年11月の中間決算", with no exact date and no second dated event. |
| G9 Next steps | FAIL | Its 確認ポイント are monitoring items, and none aims to disprove the view. |
| G10 Honesty about gaps | PASS | "10月23日と26日の上昇の背景…は、見出しレベルの情報までしか確認できていません". |
| G12 Market context | FAIL | Discusses the 10/23 and 10/26 limit-ups with no index or peer comparison. |
| G13 Internal consistency | PASS | Its "約75%下落" uses the 8/27 low and does not recognize the 10/23 low of 1,100円. The timeline order is slightly off (5/29 listed after 6/3–4), but there is no direct contradiction. |

**U = 4**

Strengths:
- Gives a clear narrative of the AI-datacenter pivot, with GPU purchase details (Compal B300 at 3.25億ドル, ASRock B200).
- Flags the cancelled contract, the one-off Q1 revenue and the funding burden of 510億 against 330億 in total assets.

Weaknesses:
- Gives no reason for the 10/26 move and is unsure of the date.
- Lacks positioning, consensus, peer context and dated catalysts.
- Its contract framing ("総額1.752億ドル") differs from every other answer, and it does not reconcile the difference.

## D
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS (marginal) | Covers business (domestic/overseas split), results, forecast, PER "6倍台", warrants/share count, earnings catalyst, price, risks and third-party analysis. |
| G3 Data dating | FAIL | Sources appear only as a generic list ("数値の出典は…決算短信…株式情報サイト…第三者による分析記事"). Key numbers do not carry their own source. |
| G4 Expectations hygiene | FAIL | Makes no mention of consensus. |
| G5 Disconfirmation | FAIL | Has only bull, neutral and bear scenarios. |
| G6 Contradictions | PASS | Q1 operating profit of 48億 sits against the 88% one-off fee, and its PER "表面的には割安に見えます". |
| G7 Related companies | FAIL | Names none with a relation type. OpenAI is mentioned only to say that no tie is confirmed. |
| G8 Catalysts | FAIL | Gives "2026年11月の中間決算" with no date, and no other dated event. |
| G9 Next steps | FAIL | Lists 注目すべき材料 to watch, with none aimed at disproving the view. |
| G10 Honesty about gaps | PASS | "この日の上昇理由は、今回の調査では確認できていません"; the 799億円 figure is "会社の開示資料で直接確認できていません". |
| G12 Market context | FAIL | Discusses the 10/23 +24.4% move with no comparison. |
| G13 Internal consistency | PASS | Has no direct contradictions. However, "自己資本比率76.2%…財務体力はあります" sits next to "GPU取得額…総資産…を上回って" without reconciliation. |

**U = 3**

Strengths:
- Gives a compact overview of the business, including legacy segment geography and the TAIZA/TOKENaaS strategy.
- Correctly flags the one-off Q1 revenue and the dilution from share count growth.

Weaknesses:
- Is anchored to the 10/23 close and entirely misses the 10/26 second limit-up, even though 10/26 is "today".
- Dates the large order to 9/24 (the price reaction) rather than its announcement. Most numbers are not tied to a specific source.
- Has no positioning, related companies, dated catalysts or disconfirmation.

## E
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers business, results quality, forecast, valuation (market cap, PER 5.5倍), capital policy (warrant shortfall), ownership (アースエレメンツ, 杉原氏, FIRST PLUS), catalyst, news (東洋経済), price/volume and risks. |
| G3 Data dating | PASS | Its timeline is dated with links per block; "予想PER5.5倍（1,530円時点）". |
| G4 Expectations hygiene | FAIL | Never mentions consensus or its absence. |
| G5 Disconfirmation | FAIL | Its thesis is "修正リスクはかなり高い". It mentions the company's "業績予想に織り込み済み" claim but immediately dismisses it, and has no section on the strongest counter-case. |
| G6 Contradictions | PASS | "8月の解約で…約799億円分の売上がなくなりました。それでも会社は予想を据え置いています". |
| G7 Related companies | FAIL | Names no related companies with a relation type. Only shareholders appear. |
| G8 Catalysts | FAIL | Its only dated upcoming event is 11/16 2Q results. |
| G9 Next steps | FAIL | Its "調べきれなかった点" lists 2 items, and none is a disconfirming investigation. |
| G10 Honesty about gaps | PASS | "26日の資料は今回読めませんでした"; "9月案件の残額（3,285万ドル）が入金されたかどうかは確認できませんでした". |
| G12 Market context | FAIL | Discusses the limit-ups with no index or peer comparison. |
| G13 Internal consistency | PASS | Its stated PER of 5.5倍 at 1,530円 does not square with its own figures (about 588億 market cap and 87億 net income, about 6.8倍), but no figure is stated two ways. Its FY3/26 経常利益 of 42億 differs from D and F (36.3億). |

**U = 7**

Strengths:
- Is the only answer to report the warrant result: only about 271億 of the planned 558億円 was raised, a shortfall of about 286億, and impact is "精査中". This is a critical forward-looking fact for funding and dilution.
- Gives the fullest history behind why the stock is controversial. It covers the 2025 order announcements, the November 2025 downward revision and the 東洋経済 skepticism, which together explain the credibility discount.
- Gives clear, practical takeaways, such as avoiding a large bet before 11/16.

Weaknesses:
- Is weak on research hygiene: no consensus statement, no peer or market comparison, no related companies and no disconfirming next steps.
- Has a valuation and number slippage (PER 5.5倍 versus its own figures).

## F
| Item | Grade | Evidence |
|---|---|---|
| G2 Lens breadth | PASS | Covers business, FY results, forecast, valuation (PER range, みんかぶ), capital policy/funding, related companies, news, price action and risks. |
| G3 Data dating | PASS | Its price table has a date and source per row, e.g. "10/23 … ミンカブ（単一ソース）". |
| G4 Expectations hygiene | PASS | "アナリスト予想は「対象外」で、コンセンサスは未取得です". |
| G5 Disconfirmation | PASS | Has a section 「最も強い反論（この見方が外れるケース）」 with supporting points. |
| G6 Contradictions | PASS | "利益は黒字だが、現金が出ていく"; "営業利益と経常利益に約123億円の差"; "評価が割れている". |
| G7 Related companies | PASS | NVIDIA (GPUの供給元), Compal (サーバーの購入先), the US customer (顧客). |
| G8 Catalysts | FAIL | Gives only "2026-11-14頃…推定", and states "確認済みの将来日程は取得できませんでした". |
| G9 Next steps | PASS | 5 items, including "[disconfirm] 9/18の大口受注の相手先、契約期間と解約条件…". |
| G10 Honesty about gaps | PASS | Gives an extensive coverage table of unretrieved lenses and says "10/26の値は未確認". |
| G12 Market context | FAIL | Discusses the 10/23 move but says "同日の日経平均や同業との比較も取れていない". |
| G13 Internal consistency | PASS | Its PER range of 6.6–8.5 matches its EPS range of 179.31–231.45 at 1,530円, and the market cap and share count agree. |

**U = 5**

Strengths:
- Has excellent hygiene: it separates company forecast from consensus, labels single-source and secondary data, and spots the gap between operating and ordinary profit.
- Is honest about scope and shows a well-structured disconfirmation section.

Weaknesses:
- Misses the core facts behind the story: the Q1 one-off revenue, the cancellation of the roughly 799億 contract, the 10/23 service-start disclosure, the 10/26 second limit-up and the 10/19 warrant expiry. Its answer to "why is it hot" and "what next" is therefore materially incomplete.
- Has no positioning or ownership data and no confirmed catalyst date (it estimates 11/14, whereas others report 11/16).

---

## Ranking
1. **A**: complete research hygiene, the correct rebound mechanism (warrant expiry plus service start) and full market context. Its main gap is the short-interest data.
2. **B**: the deepest positioning and ownership evidence and primary-source contract details. Its forward dilution framing is undermined by the missed warrant expiry.
3. **E**: the most decision-relevant unique fact (the warrant funding shortfall) and the best history of the credibility problem, but weak hygiene.
4. **F**: the cleanest methodology, but it misses most of the material developments since May.
5. **C**: a reasonable narrative of the pivot, but thin and with no counter-case.
6. **D**: stale (ignores 10/26), with a misdated order and generic sourcing.

```json
{"A": {"pass": 11, "applicable": 11, "U": 8}, "B": {"pass": 11, "applicable": 11, "U": 8}, "C": {"pass": 5, "applicable": 11, "U": 4}, "D": {"pass": 4, "applicable": 11, "U": 3}, "E": {"pass": 5, "applicable": 11, "U": 7}, "F": {"pass": 9, "applicable": 11, "U": 5}, "rank": ["A","B","E","F","C","D"]}
```
