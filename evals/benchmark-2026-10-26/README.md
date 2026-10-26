# Held-out benchmark (2026-10-26, skill v0.4.0)

This benchmark tests the skill on four stocks that were in the news, none of
which were used during development. It uses three models, with and without
the skill. All grading was blind: each grader saw six answers per case
labelled A–F, without knowing which model or setup produced each.

## Setup

| | |
|---|---|
| Cases | データセクション (3905): why it is hot and what next · キオクシア: "is it OK to buy now?" · CoreWeave: is the bond selloff a warning? · SpaceX: performance since IPO and lock-up expirations |
| Models | Haiku 5.5, Sonnet 5.5, Opus 5.5, each at its default effort. Sonnet 5 and explicit effort settings were not available in the test environment. |
| Configs | `with`: skill installed, v0.4.0. `without`: same prompt, no skill. Both had web search and fetch. |
| Runs | 4 cases × 3 models × 2 configs = 24 answers, one run each |
| Grading | Opus, blind. Rubric items G2–G10, G12, G13 ([rubric.md](rubric.md)). The coverage-table item G1 was excluded because it rewards the skill's own format. Each answer also got a usefulness score (1–10) and a rank within its case. |
| Fact-check | Sonnet with WebFetch. For each answer, the 6 most decision-relevant numeric or date claims were checked against cited or primary sources, giving 144 checks in total. |

## Results

| Config | Rubric pass | Usefulness (1–10) | Avg rank (1 = best of 6) | Facts correct* | Wrong claims |
|---|---|---|---|---|---|
| Haiku, without | 45% | 4.00 | 5.75 | 88% | 3 |
| **Haiku, with** | **89%** | **6.25** | **3.25** | 88% | 3 |
| Sonnet, without | 57% | 4.50 | 5.25 | 90% | 2 |
| **Sonnet, with** | **98%** | **8.00** | **1.75** | 100% | 0 |
| Opus, without | 45% | 6.00 | 3.75 | 96% | 1 |
| **Opus, with** | **100%** | **8.75** | **1.25** | 92% | 2 |
| All without | 49% | 4.83 | 4.92 | — | 6 / 72 |
| All with | 95% | 7.67 | 2.08 | — | 5 / 72 |

\* correct ÷ (correct + incorrect); unverifiable claims are excluded.

### Findings

- **The skill improved every model on every case.** With the skill, usefulness
  beat the same model without it in 12 of 12 model × case pairs.
- **Haiku with the skill (6.25) scored slightly above Opus without it (6.00).**
- **The skill improved research quality but not factual accuracy.** Wrong
  claims were 5 of 72 with the skill and 6 of 72 without. The errors fell into
  three groups:
  - a single outlier secondary source used for a key figure (SpaceX float);
  - a figure the agent derived itself without support (SpaceX tranche size);
  - a stale fact (warrants still described as live after they had expired),
    plus small date and arithmetic slips.

  v0.4.1 adds rules for each group: build a dated disclosure timeline first,
  re-check the status of time-limited items, use the primary or majority
  figure when sources conflict, and show and recompute every derived number.
- **The weakest result was Haiku with the skill on データセクション** (rank 4
  of 6). The answer had excellent hygiene but missed the core recent
  disclosures. This motivated the "timeline first" rule.

## Caveats

- **Semi-blind grading.** The skill's output structure is recognisable, so
  the grader could guess which answers used it. G1 was dropped for this
  reason, and the grader was told not to reward format or length.
- **One run per configuration.** Variance is not measured.
- **Search quota.** The test environment shares a web-search quota across
  agents, and it ran out during the run. Several with-skill runs had searches
  refused partway through and relied on page fetches instead (see
  [tool-calls.tsv](tool-calls.tsv)). This biases against the skill.
- **Shallow fact-check.** Six claims per answer were checked, not the whole
  answer.
- **Point-in-time data.** All market data is as of 2026-10-26 and will go
  stale. The answers themselves are not published here.

## Files

- `<case>.grading.md`: per-answer rubric grades, strengths, weaknesses and
  the ranking.
- `<case>.factcheck.md`: per-claim verdicts with sources.
- `<case>.mapping.json`: the blind label for each config.
- `tool-calls.tsv`: search and fetch counts per run as reported, with notes
  where searches were refused.
