# Comprehension Review - instructions.md §11 (threefold review model)

| Field | Value |
|---|---|
| Reviewer | comprehension reviewer |
| Date | 2026-10-14 |
| Round | 1 |
| Section | `Documentation/Logs/instructions.md` §11 (Review model), reviewed with its integration points (§3 review-agents bullet, §5/§6/§7 citations, §9.2 change-class cite, §10 file-map row, `Documentation/Reviews/README.md`, changes.md row 002, Plan/000-index row 002) |
| Method | Section read once, then restated and answered from memory without looking back |

## 1. Restatement (from memory)

Section 11 makes every document section a reviewed unit of work: each `##` heading is one section (with page-budget boundaries added where a page budget applies), and every paragraph in it is checked individually, in reading order, never batched across sections. Three independent agents review each section - comprehension (restates it from memory and answers six questions: who benefits, what problem, what the team delivers, why outcomes follow, why the amount is justified, what remains after funding), rubric (scores 1-5 on the four criteria, justifies each score, names the strongest claim, the most important unsupported assumption, the main execution risk, and what would raise each score), and evidence (verifies factual, partnership, budget, legal, and outcome claims against the source case, evidence grades §5, the data dictionary, the prohibited-words list §6, and the editing tests §7). Each round writes append-only artifacts under `Documentation/Reviews/<NNN>-<slug>/<section-slug>/`; a section passes only when all three facets pass in the same round, and any FAIL sends it back through the standard pre-plan → execute → re-review cycle, capped at three rounds per facet before the orchestrator chooses a new plan, a section cut, or a recorded `[INFORMATION NEEDED]`. Reviewers never edit the section - findings and verdicts only; the orchestrator records pass/blocked statuses in the run index and never overrides a FAIL without a new round.

## 2. The six comprehension questions

| # | Question | Answer (one line) |
|---|---|---|
| 1 | Who benefits? | The orchestrator, later reviewers, and ultimately the grant evaluators - anyone who must trust a section is clear, scored, and verified; concretely every later change and the final audit sequence consume these artifacts. |
| 2 | What problem does it address? | "Review before submission" was previously one-shot and unstructured, so unclear, unsupported, or unscored sections could reach submission with no tracked check, no iteration, and no audit trail. |
| 3 | What do the team/agents actually do? | Pre-plan agents design changes and name sections to review; execute agents implement; the three review agents run their named facet steps in order and write append-only artifacts with a findings table and a PASS/FAIL verdict; the orchestrator consolidates verdicts in the run index, routes FAILs back through revision, and commits once per version. |
| 4 | Why should it produce the intended effect? | Three independent facets each apply explicit, named checks with separate pass rules, so a section cannot pass without demonstrated comprehension, justified scores, and verified evidence - and the round cap forces a blocked section to a recorded orchestrator decision instead of silent acceptance. |
| 5 | Why this design? | Three facets triangulate reader, scorer, and verifier perspectives (mirroring the export's review-before-submission sequence); independent agents stop authors from passing their own work; append-only rounds give an audit trail; routing revision through §3 keeps the existing pre-plan/execute delegation discipline intact. |
| 6 | What remains after a review pass? | The section is marked passed in the run index with a pass date, all findings stay on file as the audit trail, the section text itself is unchanged by reviewers, and any later revision re-triggers all three facets. |

## 3. Paragraph-acceptance check (per subsection)

| Subsection | Claim first? | Traceable? | Certainty labeled? | One new idea? | Deletion loses info, not tone? | Questions failed |
|---|---|---|---|---|---|---|
| 11.1 Granularity | yes (heading states "sections are the unit of work"; first bullet states the split rule) | yes - concrete, enforceable rules | yes - normative rules, no unlabeled empirical claim | yes - one theme: what a review unit is | yes - every bullet is an operative rule | 0 |
| 11.2 The three reviewer roles | yes ("one section's review consists of THREE separate review agents") | yes - each role's named steps, cites §5/§6/§7 | yes - role definitions are normative; no hedge or bare claim | yes - one theme: the three roles plus the never-edit constraint | yes - dropping any role loses a whole facet | 0 |
| 11.3 Review artifacts | yes ("every round writes to …") | yes - exact paths, file contents, index schemas | yes - imperative conventions, nothing asserted as fact | yes - one theme: tracked, append-only artifacts | yes - the paths/formats are load-bearing for later runs | 0 |
| 11.4 Pass rules and iteration | yes ("comprehension passes when …") | yes - pass conditions tie to facets, §3, §9.2 | yes - `[INFORMATION NEEDED]` convention labels unknowns; rules are normative | yes - one mechanism (pass conditions + failure handling); dense but single-themed | yes - round cap, same-round rule, and no-override rule each carry distinct info | 0 |
| 11.5 Paragraph acceptance | yes ("review every paragraph with five yes-or-no questions") | yes - the five questions are concrete and checkable | yes - binary yes/no determination, no uncertain claim | yes - one checklist, one retention rule | yes - the two sentences define the whole check | 0 |

Note (non-blocking): 11.4 packs five distinct rules (three facet pass conditions, same-round requirement, revision cycle, round cap, orchestrator authority); it is the densest subsection but holds a single coherent mechanism, so "one new idea" still holds.

## 4. Verdict

**PASS** - the restatement is faithful to §11 and its integration points (§3 bullet, §10 row, README index, changes.md row 002, plan-index row 002); all six comprehension questions are answered; no subsection fails more than one acceptance question (all fail zero). No blocking defect. Minor observation only: 11.4's density makes it the likeliest future comprehension-failure point and could be split, but this does not fail acceptance today.