# Output template

Write in the user's language (Japanese question → Japanese answer; keep
tickers and form names as they are). State each fact once and refer back to
it. Keep coverage rows to one line. Respect the length guide for the depth
level set in SKILL.md.

## Standard / Deep report

```markdown
# <Company (code/ticker, market)> — <question in a few words>
As of <YYYY-MM-DD>. Latest results used: <period, release date>.

## Answer
<2–5 sentences that directly answer the question, with the main reason and
the main caveat.>

## Key findings
- <Fact with number, period, basis, as-of date> (source)
- ...

## Coverage
| Lens | Status | Note (one line) |
|---|---|---|
| Business | Checked | ... |
| Results & quality | Checked | ... |
| Expectations | Partial | Company guidance found; consensus not found |
| Valuation | Checked | ... |
| Capital policy | Checked | ... |
| Positioning | Checked | 信用倍率 x.x (MM/DD申込分, MM/DD公表) ... |
| Ownership & insiders | Partial | ... |
| Catalysts | Checked | Next earnings MM/DD ... |
| Related companies | Checked | ... |
| Macro | Checked | ... |
| Sector data | Partial | ... |
| News & sentiment | Checked | ... |
| Price & liquidity | Checked | Move vs index/peers on MM/DD ... |
| Risks | Checked | ... |
Status: Checked / Partial / Not found / N/A (日本語: 確認済 / 一部 / 未取得 /
対象外). Give a reason for anything other than Checked.

## Contradictions & surprises
- <A vs B> → <what explains it / still open>

## Related companies
| Company | Relation | Evidence | Latest read-across |
|---|---|---|---|
| ... | customer (≈X% of sales) | 有報 主要な顧客 FY2025 | capex guidance cut → negative |

## Strongest case against this conclusion
<The best evidence or scenario in which the headline answer is wrong, and
what would confirm it.>

**Main supporting points:** ...

## What seems priced in / scenarios
| Scenario | Key assumptions | What must be true | Indicative impact |
|---|---|---|---|

## Next dated events
| Date | Event | Status |
|---|---|---|
| MM/DD | <company earnings / AGM / lock-up …> | confirmed (IR) / estimated |
| MM/DD | <peer or customer results> | confirmed (source) |
| MM/DD | <FOMC / 日銀 / CPI …> | confirmed |

## Next investigations
1. [disconfirm] <question> — why it matters — what to search/read
2. [fill_gap] ...
3. [monitor] <event/date> ...

## Data caveats
- <lags, secondary data, definitional differences, source conflicts, gaps>

Sources: <titles, dates, URLs>
```

## Quick answer

```markdown
<Direct answer with the number(s), period, as-of date and source.>

**Also worth knowing:** <2–4 bullets from other lenses that change how to read
the answer — e.g. positioning, upcoming event, peer read-across.>

**Could be wrong if:** <one line: the strongest counter to the answer>

**Coverage:** checked <lenses>; not checked / not found <lenses and why>.

**Next:** [verify] ... / [disconfirm] ...
```

## Example (Quick, illustrative — company and figures are fictional)

User: 「A社の空売りって多い？」

```markdown
A社の空売り残高報告では、機関投資家3社が合計で発行済株式の約2.1%を
売り建てています(10/22計算分、10/24公表)。前月の約1.2%から増えています。

**合わせて見るべきこと:**
- 信用倍率は0.8倍(10/23申込分、10/26公表)で売り長です。日証金では逆日歩が
  5日連続で発生しており、借りにくい状態です。
- 9月に転換社債を発行しているため、空売りの一部はCBアービトラージの
  ヘッジである可能性があります(推定)。
- 決算発表は11/7。空売りの増加と決算前のタイミングが重なっています。

**この見方が外れるケース:** 報告者の中心がCBアービトラージなら、方向性の
売りは見た目より少なく、決算で踏み上げが起きても続きにくいです。

**カバレッジ:** 需給・イベント・ニュースは確認済。業績とバリュエーションは
簡易確認のみ。コンセンサスは未取得。

**次に調べること:** [verify] CBの発行条件と残高 / [disconfirm] 空売り報告者の
戦略(ヘッジファンドか証券会社のヘッジか)
```
