# Output templates

Write in the user's language (Japanese question → Japanese answer; keep
tickers and form names as they are). State each fact once and refer back to
it.

Two modes (see SKILL.md → Output):
- **Normal mode (default):** conversational, short. The research is just as
  wide; only the presentation is compact.
- **Report mode:** full structured report, used when the user asks for a
  report / 詳しく / 全部, or accepts the offer at the end of a Normal answer.

## Mode rules

There are two output modes. Research depth (Step 1) and output mode are
independent: a Deep investigation can still be answered in Normal mode.

### Normal mode (default) — rules

Use for ordinary questions. Write a conversational answer, mostly prose with
light structure, in the user's language:

- **Length:** about 300–800 words (日本語 ~800–2,000字), excluding sources.
  Quick questions can be shorter.
- **Answer first**, in 2–4 sentences.
- **The key facts** behind it (3–6 items), each with its date/period and a
  short source.
- **What is easy to miss** — 1–3 points from the wider sweep that change how
  to read the answer (positioning, expectations vs consensus, a time-limited
  event, a related company, the strongest counter-argument). This is where
  the breadth of the research shows; do not drop it.
- **What to watch / check next** — 1–2 items, including the next confirmed
  dated event if there is one.
- A one-line note on important gaps or data limits, if any.
- End with a one-line offer of the full report (e.g. 「詳しいレポート形式でも
  まとめられます」). If the user accepts, produce Report mode from the research
  already done instead of starting over.

Do not show the coverage table, tag lists or scenario tables in Normal mode;
the research steps still happen, only the presentation is shorter.

### Report mode — rules

Use when the user asks for a report, 詳しく/徹底的に/全部/レポート, a full
write-up, or accepts the offer above. Use the Report template below:

1. **Answer first** — direct answer to the question.
2. **Key numbers** — the verified ledger from Step 7 (value, as-of,
   basis, source, verification status).
3. **Key findings** — decision-relevant facts with date and source. State
   each fact once; later sections refer back instead of repeating it.
4. **Coverage table** — every lens, one line each, with a text status:
   Checked / Partial / Not found / N/A (in Japanese: 確認済 / 一部 /
   未取得 / 対象外). Give a reason for Partial, Not found and N/A. Mark
   lenses unrelated to the question N/A rather than padding them.
5. **Contradictions & surprises** and how far they were resolved.
6. **Related companies** — relation type (competitor, customer, supplier,
   parent, substitute, same-theme-unverified) and the evidence.
7. **Strongest case against the conclusion** (from Step 5), plus the main
   supporting points.
8. **Next dated events** — at least two dates confirmed by sources fetched in
   this run, each marked confirmed (with source) or estimated. Dates from
   memory count as estimated.
9. **Next investigations** — 3–5 prioritized items tagged `verify` /
   `disconfirm` / `compare` / `fill_gap` / `monitor`, each with why it matters
   and exactly what to search or read. Include at least one `disconfirm`.
10. **Data caveats** — lags, secondary data, definitional differences,
    conflicts between sources, missing data.
11. **Sources** with titles and dates.

Report length guide (excluding sources): Standard ~1,000–2,000 words
(日本語 ~3,000–6,000字); themes ~1,500–2,500 words (~4,000–8,000字); Deep up
to ~4,000 words (~12,000字).

### Both modes — rules

Match the user's language (Japanese question → Japanese answer). For
positioning questions, the most useful extras are the neighbouring
positioning data first (信用残 → 貸借倍率/逆日歩 and 空売り残高報告; short
interest → borrow cost, days to cover and options), then the next catalyst.

---

## Normal mode

Mostly prose, light structure. About 300–800 words (日本語 ~800–2,000字),
excluding sources.

```markdown
<Answer in 2–4 sentences: the conclusion, the main reason, the main caveat.>

**ポイント / Key facts**
- <fact with number + period/as-of date> (<short source>)
- <fact> (<source>)
- <fact> (<source>)

**見落としやすい点 / Easy to miss**
<1–3 short points from the wide sweep that change how to read the answer:
positioning, expectations vs consensus, a time-limited event, a related
company, or the strongest counter-argument.>

**次に見るところ / What to watch**
<1–2 items, including the next confirmed dated event if there is one.>

<Optional one line on important data gaps or limits.>

<One-line offer: 「詳しいレポート形式でもまとめられます」 / "Want the full
report?">

Sources: <short list, titles + dates>
```

Do not include the coverage table, tag lists or scenario tables here.

### Example (Normal, illustrative — company and figures are fictional)

User: 「A社の株、最近どう？」

```markdown
A社は10/24の上方修正で株価が2日で約18%上がりましたが、修正後の営業利益予想
(120億円)はアナリスト予想の平均(約125億円)をまだ下回っていて、「予想ほど
良くはない」という見方も残っています。上昇の大半は好材料というより売り方の
買い戻しが効いた可能性があります。

**ポイント**
- 通期営業利益予想を100億円→120億円に上方修正(10/24、決算短信)
- 株価は10/23終値2,450円→10/25終値2,890円(+18%)。同じ2日間のTOPIXは+0.6%
- 信用倍率は0.7倍で売り長(10/23申込分)。上昇局面で売り残が約3割減少

**見落としやすい点**
- 9月に発行した新株予約権(行使価額修正条項付)の行使が進むと、株価の上値を
  抑える売りが出やすくなります。残りの行使可能株数は発行済株式の約6%。
- 主要顧客B社が来週の決算で設備投資計画を出す予定で、A社の受注見通しに直結
  します。

**次に見るところ**
- 11/5 B社決算(設備投資計画)、11/12 A社 第2四半期決算

詳しいレポート形式(需給・関連企業・反論・シナリオ込み)でもまとめられます。

Sources: A社 決算短信・業績予想修正(10/24)、JPX 銘柄別信用残(10/26公表)、…
```

---

## Report mode

```markdown
# <Company (code/ticker, market)> — <question in a few words>
As of <YYYY-MM-DD>. Latest results used: <period, release date>.

## Answer
<2–5 sentences that directly answer the question, with the main reason and
the main caveat.>

## Key numbers (verified)
| Number | Value | As-of / period | Basis | Source | Status |
|---|---|---|---|---|---|
| ... | ... | ... | 連結 / GAAP … | <primary / media / aggregator> | 2 sources agree / primary checked / unverified |

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

Length guide (excluding sources): Standard ~1,000–2,000 words (日本語
~3,000–6,000字); themes ~1,500–2,500 words (~4,000–8,000字); Deep up to
~4,000 words (~12,000字). Keep coverage rows to one line.
