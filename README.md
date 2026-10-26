# equity-research

**An Agent Skill for wide-lens Japanese & US stock research — no tunnel vision.**
日本株・米国株を「視野狭窄に陥らず」調べさせるための Agent Skill。 → [日本語](#日本語)

![Agent Skills](https://img.shields.io/badge/Agent%20Skills-SKILL.md-0d9488)
![Markets](https://img.shields.io/badge/markets-JP%20%7C%20US-2563eb)
![License](https://img.shields.io/badge/license-Apache--2.0-64748b)

`equity-research` is a text-only [Agent Skills](https://agentskills.io/specification)
package: a `SKILL.md` plus reference files. It needs no code, no API keys and
no server. Your agent's own web search does the fetching. The skill tells the
agent:
- what to look at;
- how to read it correctly;
- what to dig into next.

The failure mode it targets is **tunnel vision**. A typical AI answer finds
one story (great earnings, a hot theme) and builds the whole answer around it.
It ignores:
- expectations;
- positioning (short interest, 信用残, 逆日歩);
- related companies;
- the evidence against its own conclusion.

---

## Architecture

![Architecture](docs/images/architecture.svg)

The skill loads in three layers, called *progressive disclosure*:

1. **Metadata.** Name and description with JP/EN trigger words. It is always
   in context, so the agent knows when to use the skill.
2. **`SKILL.md`.** Loaded when the skill triggers. It holds the workflow,
   principles, tool-call budgets, the output contract and a hygiene checklist.
3. **`references/`.** The agent reads only the 2–4 files the task needs:
   definitions, publication lags and common misreadings for each data type.

## Workflow

![Workflow](docs/images/workflow.svg)

1. **Frame & budget.** Classify the request into one of 8 types:
   - single-stock deep dive
   - earnings
   - price move
   - event
   - theme
   - comparison
   - macro
   - positioning

   Then set a hard budget of search + fetch calls.
2. **Pin the security & the clock.** Confirm the code/ticker, fiscal year and
   accounting basis, the latest results, and what happened in the last few
   days.
3. **Wide sweep.** Do a minimum check of all 14 lenses. Before marking
   anything "not found", run a freshness sweep. Before naming a cause for a
   price move, compare the stock with the index, its sector and peers.
4. **Go deep.** Order: contradictions, then surprises, then high-impact
   unknowns, then second-order effects on related companies.
5. **Disconfirm.** State the headline conclusion in one sentence. Then search
   for the best evidence that *this* conclusion is wrong.
6. **Synthesize & check.** Build the priced-in view and conditional scenarios.
   Then run a consistency pass: tiers, figures, cross-references and
   comparative claims must all match.
7. **Verify the key numbers.** Keep a ledger of the 5–10 numbers the
   conclusion rests on, each with its source, date and basis. After drafting:
   - re-open the sources, preferring primary documents;
   - re-check the status of time-limited items (warrants, lock-ups, offers);
   - recompute every derived figure.

   Where the agent can start a sub-agent, a fresh agent checks the ledger
   independently.

## The 14 lenses

![14 research lenses](docs/images/coverage-lenses.svg)

All 14 lenses are researched for every question. In Report mode, the answer
includes a coverage table that shows the status of each lens: Checked /
Partial / Not found / N/A. Blind spots stay visible instead of silently
missing.

## What an answer looks like: two output modes

Research depth and output length are separate. The agent always researches
wide, but by default it answers short.

| | **Normal mode (default)** | **Report mode** |
|---|---|---|
| When | Everyday questions | 「詳しく」「レポートで」「全部」, or accepting the offer at the end of a Normal answer |
| Length | ~300–800 words (日本語 ~800–2,000字) | Full structured report |
| Shape | Prose: answer → key facts with dates → easy-to-miss points → what to watch | Answer → verified key numbers → coverage table → contradictions → related companies → strongest counter-case → dated events → next investigations → caveats |

Normal mode example (fictional company):

> A社は10/24の上方修正で株価が2日で約18%上がりました。ただし、修正後の営業利益予想
> (120億円)は、アナリスト予想の平均(約125億円)をまだ下回っています。上昇の大半は、
> 売り方の買い戻しが効いた可能性があります。
>
> **ポイント**
> - 通期営業利益予想を100億円から120億円に上方修正(10/24、決算短信)
> - 2日間で+18%。同じ期間のTOPIXは+0.6%
> - 信用倍率0.7倍の売り長(10/23申込分)
>
> **見落としやすい点**
> - 行使価額修正条項付の新株予約権(発行済株式の約6%)が残っていて、上値を抑えやすいです。
> - 主要顧客B社の設備投資計画が11/5に出ます。
>
> **次に見るところ:** 11/5 B社決算、11/12 A社 第2四半期決算
>
> 詳しいレポート形式でもまとめられます。

## Highlights

- **Correct reading of positioning data, verified against primary sources (as
  of 2026-10).** Examples:
  - 空売り比率 is market-wide; 空売り残高報告 is per stock.
  - JPX 銘柄別信用残 has been published **daily since 2026-09-28**.
  - FINRA short volume ≠ short interest.
  - Borrow cost measures lendable-supply tightness, not short conviction.
  - Form SHO data is not public until 2028.
- **Rule-change ledger.** It lists recent changes that make older knowledge
  wrong:
  - Japanese TOB threshold of 30%, effective 2026-05
  - TOPIX second-stage review
  - Russell reconstitution twice a year
  - abolition of the 四半期報告書
  - SEC proposal for semiannual reporting
- **Expectations hygiene.** 会社予想 / guidance, consensus and actual results
  are always kept separate. Consensus is never invented.
- **Typed related companies.** Each link is labelled competitor, customer,
  supplier, parent or "same theme (unverified)", with its evidence. Media
  "関連銘柄" lists are not treated as proof of exposure.
- **Budgets.**

  | Depth | Search + fetch calls |
  |---|---|
  | Quick | ≤ 30 |
  | Standard | ≤ 80 |
  | Standard-wide (themes) | ≤ 120 |
  | Deep (詳しく) | ≤ 160 |

  Answer length is set by the output mode, not by the depth.
- **Number verification.** The agent keeps a key-number ledger. After
  drafting, it:
  - re-opens the sources;
  - re-checks the status of time-limited items;
  - recomputes derived figures;
  - when sources conflict, uses the primary or majority value, never a lone
    outlier.
- **Safety.** Web content is treated as data, never as instructions. The
  skill gives no buy/sell calls, only conditional scenarios.

## Evaluation

### Held-out benchmark: recent stocks × 3 models (blind)

![Held-out benchmark by model](docs/images/benchmark-models.svg)

The benchmark used four stocks that were in the news and were never used
during development:
- データセクション
- キオクシア
- CoreWeave
- SpaceX

Each prompt was answered by Haiku 5.5, Sonnet 5.5 and Opus 5.5, with and
without the skill, for 24 answers in total. Grading was blind: an Opus grader
saw answers labelled A–F. A separate agent fact-checked 144 numeric or date
claims against sources.

| | Without skill | With skill |
|---|---|---|
| Rubric pass rate | 49% | **95%** |
| Usefulness (1–10) | 4.83 | **7.67** |
| Average rank (of 6) | 4.92 | **2.08** |
| Wrong claims | 6 / 72 | 5 / 72 |

What the results show:
- The skill won all 12 same-model pairs.
- Haiku with the skill (6.25) slightly outscored Opus without it (6.00).
- Factual accuracy did **not** improve. v0.4.1 adds rules aimed at the error
  patterns found: build a dated disclosure timeline first, re-check the status
  of time-limited items, handle conflicting sources, and recompute derived
  numbers.

These results are for v0.4.0. v0.5.0 adds Normal and Report output modes
and the number-verification step, and has not been re-benchmarked yet.

Method, caveats (semi-blind grading, single runs, a shared search quota that
hurt late with-skill runs) and all grading files:
[`evals/benchmark-2026-10-26/`](evals/benchmark-2026-10-26/).

### Development iterations

![Evaluation results](docs/images/eval-results.svg)

Six development prompts were run with and without the skill and graded
against [`evals/rubric.md`](evals/rubric.md). Three rounds of fixes covered:
- counter-arguments aimed at the conclusion itself;
- a market-comparison gate;
- dated next events;
- consistency checks;
- budgets.

See [`evals/README.md`](evals/README.md).

## Install

Copy `skills/equity-research/` into your agent's skills directory:

| Agent | Location |
|---|---|
| Claude Code | `~/.claude/skills/equity-research/` or `<project>/.claude/skills/equity-research/` |
| Claude.ai / Claude API | upload the folder (zip) as a custom skill |
| OpenAI Codex | `~/.agents/skills/` or `<repo>/.agents/skills/` |
| Gemini CLI | `~/.gemini/skills/` or `.agents/skills/` |
| Cursor | `.agents/skills/` or `.cursor/skills/` |
| GitHub Copilot CLI | `.github/skills/` or `~/.copilot/skills/` |

```bash
git clone https://github.com/Aero123421/equity-research-skill.git
cp -r equity-research-skill/skills/equity-research ~/.claude/skills/
```

The agent needs **web search and page fetch** tools. Paths can change; check
your agent's documentation.

## Usage

Just ask:

- 「レーザーテック（6920）って今どうなの？詳しく調べて」
- 「データセンター向け電力設備で、本当に恩恵を受けている銘柄は？」
- 「フジクラの信用残ってどうなってる？」
- 「キオクシアについて詳しくレポートでまとめて」 (Report mode)
- "How did Tesla's latest quarter look, and why did the stock react that way?"
- "Is SMCI a short-squeeze candidate?"

## Repository layout

```
skills/equity-research/
├── SKILL.md                      workflow, principles, budgets, output contract, checklist
└── references/
    ├── coverage-map.md           minimum check per lens, mandatory lenses by request type, contradiction patterns
    ├── output-template.md        report templates
    ├── disclosures-earnings.md   JP/US filings, earnings checklist, accounting differences, red flags
    ├── supply-demand-jp.md       空売り・信用残・貸借/逆日歩・投資部門別・大量保有・TOPIX/日経
    ├── supply-demand-us.md       short interest, borrow, 13F/13D/Form 4, options, flows, index events
    ├── events-catalysts.md       TOB/M&A/index/FDA/offerings…, rule-change ledger, news & sentiment
    ├── macro-sector.md           macro & cross-asset indicators, KPIs for 22 sectors
    ├── valuation.md              valuation, peer comparison, price action & liquidity
    └── related-companies.md      value-chain mapping, relation types, evidence standards
evals/                            test prompts, rubric, results
docs/images/                      diagrams
```

## Maintenance

Market rules and data publication practices change. The references carry a
dated change log, last reviewed **2026-10-26**. When something changes, please
open a PR and bump `metadata.last_reviewed` in `SKILL.md`.

## Disclaimer

This skill is for research and education only. It is **not investment
advice**. Verify important figures against primary sources. Data you retrieve
is subject to its source's terms.

## License

[Apache-2.0](LICENSE)

---

## 日本語

`equity-research` は、AIエージェントに日本株・米国株の調査を**視野狭窄に陥らず**
行わせるための Agent Skill です。中身はテキストだけで、コード・APIキー・サーバーは
不要です。エージェント自身のWeb検索を使い、このSkillが次の3点を指示します。
- 何を見るか
- どう正しく読むか
- 次に何を掘るか

### 何が変わるか

- **結論の前に14の観点を確認します。**
  業績、期待値、バリュエーション、需給、株主、イベント、関連企業、マクロ、業界、
  ニュース、株価、リスクなどです。回答には観点ごとの確認状況を示す
  カバレッジ表が付きます。
- **需給データを正しく読みます。**
  - 空売り比率は市場全体の数字、空売り残高報告は個別銘柄の数字です。
  - 信用残は2026年9月28日から日次公表です。
  - 日証金の貸借倍率と逆日歩も確認します。
  - 米国の Short Interest と Short Volume は別物として扱います。
- **株価変動の原因を言う前に、指数・セクター・同業と比べます。**
- **自分の結論への最も強い反論を必ず示します。**
- **関連企業は関係の種類と根拠で示します。**
  関係の種類は顧客、競合、仕入先、「同テーマ・未検証」などです。
  ニュースの「関連銘柄」リストは、恩恵の根拠として扱いません。
- **普段は短く答えます(普通モード)。**
  調査は14観点を広く行ったうえで、回答は会話の長さにまとめます。
  「詳しく」「レポートで」と頼まれたときだけ、フルのレポート形式で出します。
- **重要な数字は検証してから使います。**
  結論を支える数字は、出典・時点・基準(連結か単体か等)を記録して管理します。回答を書いた後に、
  - 出典を開き直して値を確認します。
  - 期限のある情報(ワラント・ロックアップ等)は、今の状態を再確認します。
  - 自分で計算した数値は検算します。
- **次の調査と、日付付きの今後のイベントを提案します。**
  次の調査には verify / disconfirm / compare / fill_gap / monitor のタグが付きます。
- **調査量に上限があります。**

  | 深さ | 検索・取得の回数 |
  |---|---|
  | Quick | 30回まで |
  | Standard | 80回まで |
  | テーマ調査 | 120回まで |
  | 詳しく | 160回まで |

### 評価

#### 話題の銘柄でのベンチマーク

対象は開発に使っていない4銘柄です。
- データセクション
- キオクシア
- CoreWeave
- SpaceX

Haiku・Sonnet・Opus（いずれも5.5）のそれぞれで、Skillあり・なしを比較しました。
どれがSkillありかを伏せて採点し、回答中の主要な数字の事実確認も行いました。

| 指標 | Skillなし | Skillあり |
|---|---|---|
| 採点基準の合格率 | 49% | **95%** |
| 有用度（10点満点） | 4.83 | **7.67** |
| 誤った記述の数 | 6/72 | 5/72 |

- 同じモデル同士で比べると、12組すべてでSkillありが上回りました。
- Skillありの Haiku は、Skillなしの Opus をわずかに上回りました。
- 一方、数字の正確さはほとんど変わりませんでした。そのため v0.4.1 で、次の対策を追加しています。
  - 最初に、日付付きの開示タイムラインを作る
  - 期限のある情報（ワラントなど）が今も有効か、再確認する
  - 情報源どうしの数字が食い違うときの扱いを決める
  - 自分で計算した数値は、検算する

詳細は `evals/benchmark-2026-10-26/` を参照してください。

#### 開発中の改善

| ラウンド | 結果 |
|---|---|
| 初回 | Skillあり **93%** / なし 48% |
| 改善3回目（最も難しい3ケース） | **96%** |

### インストール

`skills/equity-research/` を、使っているエージェントの skills ディレクトリに
コピーしてください。場所は上の表を参照してください。

### 注意

調査・学習用です。投資助言ではありません。重要な数値は一次情報で確認してください。
