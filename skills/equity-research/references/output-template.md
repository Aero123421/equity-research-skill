# Output templates

Use the user's language and requested length. Answer the question first.
State each material fact once and place its source beside it. These are
optional shapes, not mandatory section or item counts.

Contents:
1. Choose the format
2. Normal answers and follow-ups
3. Reports and coverage statuses
4. Report template
5. Citations, dates and gaps

## 1. Choose the format

- **Normal (default):** conversational, with as much detail as requested.
  A single fact may need only a few sentences; an ordinary analysis may use
  ~300–800 words (日本語 ~800–2,000字). Do not pad to reach a length guide.
- **Report:** use when the user requests a structured/full report or accepts
  an earlier report offer. “詳しく / deeply” alone changes research depth,
  not output format. An explicit “three bullets” or “briefly” takes precedence.

Depth and format are independent. Do not hide material uncertainty to keep
an answer short; remove repetition and irrelevant background instead.
Do not append a standing offer for a longer report to every answer.

## 2. Normal answers and follow-ups

For a fact, give the answer, its definition/date/source and any caveat that
changes the meaning. A broad analysis can add key findings, an easy-to-miss
point or counter-evidence, and the next useful check. Add sections or small
tables only when they make the answer clearer.

For a **follow-up**, lead with what changed since the stated baseline, what
that changes in the conclusion and what remains unconfirmed. Reuse supported
background; refresh changing facts. If the baseline is unavailable, say you
can provide a current snapshot but cannot establish the delta.

For a **source-limited answer**, identify the provided evidence and cut-off.
Do not call it a live or latest check. Avoid repeating this caveat in every
paragraph.

### Example: one factual calculation

All company names, dates and figures below are fictional supplied inputs.
No live source retrieval is implied.

User: 「この表の信用倍率だけ教えて」

Provided table A: A社; 信用買い残120万株・信用売り残60万株;
対象日2026-10-23、公表日2026-10-26.

> 表の信用倍率は **2.0倍** です（120万株 ÷ 60万株）。対象日は10月23日、
> 公表日は10月26日です。これは信用買い残と売り残の比率で、日証金の貸借倍率とは
> 別の指標です。この倍率だけで株価の上げ下げは判断できません。
> 出典：提供資料「表A」。

Do not add an earnings calendar, 14-lens table or unrelated company analysis
to this answer. For an analytical squeeze question, add the relevant
positioning and catalyst evidence instead.

### Example: uncertainty in a price-move answer

When the inputs show rising prices, a low margin ratio and declining short
balances, write:

> 買い戻しが寄与した可能性はありますが、この需給データだけでは上昇への寄与の
> 大きさは特定できません。

Identify the disclosure and market/peer comparison separately. Do not promote
a possible driver to “most of the move” without evidence of that contribution.

## 3. Reports and coverage statuses

Select sections that help answer the request. For a comprehensive company
report, show the 14-lens assessment compactly. For a focused report, state the
scope and show the relevant lenses; do not add unrelated sections for symmetry.

Use the same status meanings in working notes and reports:

| Status | Japanese | Meaning |
|---|---|---|
| Checked | 確認済 | Relevant evidence was assessed; cite what supports the finding |
| Partial | 一部 | Some evidence was assessed, but a material part is unresolved |
| Not found | 未取得 | A reasonable search found no usable evidence; state sources/scope or access limit |
| Not checked | 未確認 | The assessment was not performed; say why, e.g. budget or unavailable tools |
| N/A | 対象外 | The lens is genuinely irrelevant to this question; explain briefly |

A lens judged relevant but left unresearched is **Not checked**, not N/A.
“Not found” does not mean the fact is false, and “Checked” does not mean an
issuer's underlying assertion has independent confirmation.

Include the claims/numbers that support the answer; do not require 5–10
entries. If a crucial fact is disputed, show its status and the effect on the
conclusion. Do not label the whole table “verified” while hiding unverified
entries.

For analytical conclusions, include the best supported counter-case. Related
companies need relation type and evidence when included. Cite actual exposure
and the stage of any project. If there is no supported contradiction, say so
or omit that section.

List **relevant confirmed upcoming events when available** with the source and
date checked. Show estimated windows separately with their basis; do not turn
a historical schedule into an exact confirmed date. If nothing is announced
or checkable, state that plainly. Never add unrelated macro events to meet a
minimum count.

Suggest only useful remaining investigations, with the question, why it
matters and where to verify it. Tags such as verify / disconfirm / compare /
fill_gap / monitor are optional. Do not make up open questions when the user's
request is complete.

## 4. Report template

Adapt this template; remove unneeded sections and empty placeholder rows.

```markdown
# <Company / theme> — <question>
Information cut-off: <YYYY-MM-DD HH:MM timezone, or stated date>.
Scope: <security/market, question and source limits>.
Latest results used, when relevant: <period and release date>.

## Answer
<Direct answer, main supporting evidence and material uncertainty.>

## Key claims and numbers
| Claim / figure | Value / status | Period / as-of | Publication date | Basis / unit | Source and check |
|---|---|---|---|---|---|
| <Only decisive entries> | ... | ... | ... | ... | <Source, attribution, passage checked / recomputed / unresolved> |

## Findings
<Relevant facts, estimates and inferences, with sources next to each claim.>

## Coverage
| Lens | Status | Evidence or limitation |
|---|---|---|
| <Relevant lens; all 14 for a comprehensive report> | <Actual status> | ... |

## Contradictions and counter-evidence
<What challenges the headline, how far it was resolved and what would change the view.>

## Related companies
| Company | Relation | Evidence and stage | Effect on the question |
|---|---|---|---|
| ... | <customer / competitor / supplier / parent / inferred theme link> | ... | ... |

## Conditional scenarios
| Scenario | Stated assumptions | Mechanism / computation | What would confirm or reject it |
|---|---|---|---|
| ... | ... | ... | ... |

## Upcoming events
<Only relevant announced dates with sources. List estimates separately,
or say no relevant date could be confirmed within the stated source scope.>

## Remaining questions
<Only material unresolved questions, the evidence needed and its likely source.>

## Data limitations
<Material lags, unavailable evidence, source conflicts or comparability limits.>

Sources: <Titles, publication dates, URLs or supplied document/page identifiers>.
```

A short event report can be brief. For a broad report, ~1,000–2,000 words
(日本語 ~3,000–6,000字) is often sufficient; a complex deep investigation may
need more. The question and user instruction decide length, not a fixed quota.

## 5. Citations, dates and gaps

Use host-supported citations or direct links for fetched sources. Name
provided documents/tables and pages without inventing public URLs. A source
list supplements claim-level citations; it does not replace them.

Identify market data's session/time and lagged data's as-of and publication
dates. Distinguish company guidance from consensus, consolidated from parent
figures, and GAAP from adjusted metrics. Show inputs for decisive calculations.

Describe a missing claim according to the actual work: “not in the provided
documents,” “not found in the issuer releases checked through <date>,” or
“could not access the original filing.” Do not claim a search, independent
review or current verification that did not occur.
