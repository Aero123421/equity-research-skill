# Evaluation

Test cases are in `cases.json` and assertions in `rubric.md`. Each case was
run with a mid-size model (Claude Sonnet) acting as the assistant with web
search, with and without the skill. A separate stronger model graded every
answer against the rubric, using the text only.

## How to run

For each case, start a fresh agent session with web search enabled.

- **With the skill:** install the skill, ask the prompt, and save the answer.
- **Without the skill (baseline):** ask the same prompt with no skill
  installed.

Then grade every answer against `rubric.md`. Each assertion is PASS or FAIL,
with a short quote as evidence.

## Results (2026-10-26)

### Iteration 1 (v0.1): 4 cases, generic G1–G10 and case-specific assertions

| | with skill | without skill |
|---|---|---|
| Rubric pass rate | **50/54 (93%)** | 26/54 (48%) |

Without the skill, answers mostly lacked these things:

- a coverage map
- a disconfirming argument
- dated catalysts
- related companies with relation types
- next steps

### Iteration 2 (v0.2): 6 cases, G1–G13

Three assertions were added: G11 targeted disconfirmation, G12 market
comparison, and G13 internal consistency.

- **Overall:** 89/100.
- **Four repeated cases:** 82% → 88%. The counter-argument was now aimed at the
  headline conclusion in 4 of 4 cases (0 of 4 before).
- **Length:** answers were 28% shorter.
- **Budget:** runs stayed inside the tool-call budget. Iteration 1 had runs
  using 100+ calls.

### Iteration 3 (v0.3): the 3 weakest cases

- **Score:** 47/49 (96%), up from 43/49 (88%).
- **Price moves:** now checked against the index and peers before a cause is
  named.
- **Dated next events:** restored.
- **Undated positioning data:** gone.

### Known remaining weaknesses

These were addressed in v0.3.1 instructions but not re-measured:

- comparative claims not recomputed against the answer's own numbers
- top-tier theme names without their qualifying exposure figure
- calendar dates taken from memory

Market data in the test answers came from live web search on 2026-10-26. The
answers themselves are not included, because they go stale quickly.

### v0.4.0 note

Tool-call budgets were doubled after these runs: Quick 30, Standard 80,
Standard-wide 120 and Deep 160. The aim is to leave more room for the
freshness sweep, market comparison and dated-event checks. The answer-length
guides are unchanged. The scores above were measured with the earlier
budgets.

## Held-out benchmark (2026-10-26)

This benchmark uses four recent stocks that were never used during
development. Each prompt was answered by three models (Haiku, Sonnet and Opus
5.5), with and without the skill. An Opus grader scored the answers blind, and
a separate agent fact-checked their figures.

| | Without | With |
|---|---|---|
| Rubric pass rate | 49% | 95% |
| Usefulness (1–10) | 4.83 | 7.67 |
| Wrong claims | 6/72 | 5/72 |

Full method, caveats and grading files are in
[`benchmark-2026-10-26/`](benchmark-2026-10-26/).
