# Evaluation

Use the [current rubric](rubric.md) for v0.7 and later work. It checks accuracy,
request fit and applicable output requirements with PASS / FAIL / N/A.
A short, correct answer must not fail merely because it omits a coverage table
or a fixed number of events. Conversely, format cannot rescue a fabricated fact.

## Files and scope

| File | Purpose |
|---|---|
| [behavioral-cases.json](behavioral-cases.json) | Eight fictional, offline cases with worker inputs separated from grader assertions |
| [behavioral-results-2026-10-31.md](behavioral-results-2026-10-31.md) | Actual v0.7.0 behavioral run: 8/8 cases, 34/34 case-specific assertions; limits stated |
| [behavioral-run-2026-10-31.json](behavioral-run-2026-10-31.json) | Exact answers, per-assertion grades and evaluated skill hashes |
| [cases.json](cases.json) | Ten live research prompts; verify their premises and retrieve current evidence |
| [rubric.md](rubric.md) | Current common, scope/mode and request-specific checks |
| [legacy-rubric-v0.4.md](legacy-rubric-v0.4.md) | Unchanged former active rubric, retained to interpret historical development scores |
| [benchmark-2026-10-26/](benchmark-2026-10-26/) | Unchanged historical v0.4.0 benchmark, including its own rubric and caveats |

The new behavioral cases are regression fixtures, not a new accuracy benchmark.
Their presence does not mean that a model has passed them. Record actual runs
separately with the evaluated revision and do not reuse the historical scores
as evidence for the current version.

## Offline behavioral checks

These cases require no market-data account, network, script or persistent state.
The companies and documents are fictional; they test evidence handling and
response behavior rather than claims about real securities.

1. Select a case from `behavioral-cases.json` and give a **fresh worker only its
   `input` object**, plus the skill folder. Do not pass the fixture file itself,
   its `assertions`, this rubric, another run's output or the proposed fix.
2. Ask naturally: "Use equity-research at <skill folder> for the following
   request and supplied documents." Preserve the input's context, time,
   conversation (if present), user prompt and source extracts. Honor its
   document-only setting; the worker may read the skill's references.
3. Save the exact worker response and any tool trace. Record skill commit or
   snapshot, model/effort, date and case name. A single conversation covering
   all cases is not equivalent to independent fresh sessions.
4. Give a separate grader the input, answer, current rubric and that case's
   assertions. Grade each applicable item with evidence, list critical
   failures and distinguish unobserved process checks from passed checks.
5. Report which cases were actually run and any remaining failures. If a skill
   change follows a failure, rerun that case in a fresh context; preserve the
   earlier result rather than silently replacing it.

The eight cases cover a one-number answer, a cash-receipt follow-up, copied
sources versus a corrected primary source, historical publication cutoffs,
offline reporting with unknown events, operational milestones/photo evidence,
scenario arithmetic, and instructions embedded in source text.

## Live research checks

For each selected prompt in `cases.json`, start a fresh session with the
required web tools. The old benchmark prompts are now known development
material, not held-out tests. The IPO/lock-up prompt deliberately requires
checking its premise before calculating consequences.

- **With the skill:** provide the skill and the exact prompt.
- **Without the skill:** use the same prompt, information cutoff, model,
  tool access and available budget in an independent session.
- Save answers, cited sources and tool traces. Record quota/access failures;
  a source unavailable to one run can affect the comparison.
- Grade against the current rubric, blind to configuration where practical.
  Do not award points for a report when the user requested brevity. Request
  an explicit report only when testing Report mode, and record that variant.
- Check material facts independently against sources. Report accuracy and
  usefulness separately, with run counts and limitations.

Depth ceilings remain Quick 30, Standard 80, Standard-wide 120 and Deep 160
search queries/page fetches, shared with delegated work. They are maxima,
not target counts. Observe counts from traces, not the number of tool wrappers.

## Historical results — not remeasured for v0.7

The following results were already recorded in this repository. Their original
rubrics, prompts, budgets and output behavior differ from the current version.
The original development answers are not included, so these scores are not
reproduced by the current fixtures. Preserve them as historical evidence,
with the limitations below.

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
