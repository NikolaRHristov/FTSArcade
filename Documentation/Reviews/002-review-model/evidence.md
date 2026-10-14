# Evidence Review - Change 002 (Threefold Review Model)

Reviewer: evidence facet. Scope: the five files of change 002 (plan 002-review-model.md §1) against their sources - the Reference export (Documentation/Reference/we're looking to prepare a grant application for h.md, 2657 lines), the constitution (instructions.md §1-§10 as of the base commit), and the design authority (Plan/002-review-model.md). Method: `git diff` against the base commit for the changed files; direct reads of the export at the line ranges the plan's §6 names; regex greps for prohibited words; programmatic pipe-count checks for every table row.

## Check table

| # | Check | Result | Detail | Evidence location |
|---|---|---|---|---|
| 1a | §11.2 six comprehension questions copied verbatim from export | **FAIL** | §11.2 carries compressed paraphrases, not the export's questions; the plan (§1.1, §6) required verbatim copying. The plan's own blueprint block shows the paraphrase form, so the plan is internally contradictory and the executor followed the blueprint - but against the export, the executed wording is not verbatim. Quotes below. | instructions.md:120-123; plan:24, 41-44, 235; export:789-794 |
| 1b | §11.2 four rubric-criterion names match export | PASS | Words and order identical to the export's Evaluation Rubric (Transformative Ambition, Viability, Evidence of Results, Durability); case normalized to lowercase (export uses ALL CAPS; the plan's §6 itself lists them in title case). Not a wording mismatch. | instructions.md:124-125; export:544, 560, 576, 592 |
| 1c | §11.5 five paragraph-acceptance questions copied verbatim | PASS | Word-for-word match with the export's "Paragraph acceptance" list; only numbering style ("(1)" vs "1.") and initial lowercase differ. | instructions.md:173-176; export:2094-2098 |
| 1d | Other claimed-verbatim clauses | PASS | Evidence-reviewer clause "checks every factual, partnership, budget, legal, and outcome claim against the source case" is verbatim (export:1123); §11.4 pass-test list "beneficiary, action, responsible party, evidence basis, and limitation without inference" is verbatim (export:1125). | instructions.md:129-130, 152-154; export:1123, 1125 |
| 2 | Cross-references §3, §5, §6, §7, §9, §10 exist and say what is claimed | PASS | §5 (evidence grades E1-E5, line 25), §6 (prohibited words, line 47), §7 (eight editing tests, line 56), §3 (delegation model with pre-plan/execute agents plus the new review-agents bullet, lines 14-19), §10 (file map with the new Reviews row, line 104) all exist and match the claims. §11.4's "Editorial-class" names §9.2's Editorial class (defined line 87) by term only, without an explicit "§9.2" pointer - implicit citation, minor note. | instructions.md:14-19, 25, 47, 56, 83-92, 94-104; plan:109 |
| 3 | changes.md row 3 matches the change | PASS | Class Foundational, Plan ref 002, documents listed all actually changed: instructions.md (§3 bullet line 19, §10 row line 104, §11 lines 106-178), Reviews/README.md (created), Plan/000-index.md (row 002). Row matches the plan's blueprint text (§1.3) verbatim. Class justification (constitution amendment = Foundational, same as scaffold row 2) is stated in the plan; note §9.2's Foundational definition is packet-scoped and covers this only by the plan's stated analogy. Minor note: Plan/002-review-model.md itself is not named in Documents updated (precedent row 001 named Plan/001). | changes.md:11; plan:136, 138; 000-index.md:10 |
| 4 | Plan index row 002 correct | PASS | Plan file path exists and title matches plan 002's title; Notes text matches blueprint. Minor note: status "planned" is semantically stale - the change is already executed (changes.md row 002 present, §11 in the constitution), and precedent row 001 shows "executed" under identical circumstances. The plan's V7 prescribes `planned` (orchestrator flips to `committed` at commit), so the executor followed the design; the inconsistency is design-level, recorded here for the orchestrator. | 000-index.md:10; plan:142, 226; changes.md:11 |
| 5 | No prohibited words in the new text (except its own spec list) | PASS | Grep over instructions.md, Reviews/README.md, changes.md, 000-index.md: the only hits are §6's own pre-existing list (lines 49-54) and "transformative ambition" in §11.2 (line 125) - both explicitly allowed exceptions (plan V2). Zero hits in Reviews/README.md, changes.md, 000-index.md. Also grepped "unique" (in §6's list but absent from plan V2's pattern) - zero hits in new text; plan-level pattern gap only, no occurrence. | grep result: instructions.md:49-54, 125 |
| 6 | Tables render (equal pipe counts) | PASS | Every table row in the four files has equal pipe counts and a separator row: changes.md 9 pipes × 5 rows; 000-index.md 6 × 4; Reviews/README.md 7 × 3; instructions.md four tables (4, 5, 5, 3 pipes; 7/5/6/9 rows). | programmatic count: all four files |
| 7 | No silent inference (no claimed effect the design does not support) | PASS | changes.md "Why": encoding the export's "Review before submission" (export:1117-1126 prescribes exactly the three reviews §11 implements) - supported. "Every section becomes a reviewed unit of work" - §11.1 makes sections the unit - supported. Reviews/README.md "first runs at T01-T12 verification and follow-on sweep" - plan §2.1/§2.2 specify them - supported. Minor note: §11.4's "section cut (page-budget rule)" is stronger than the export's Page budget preference (export:1664 prefers moving detail to an appendix); the budget caps exist and a cut is an orchestrator choice under them, so it is a defensible reading, not unsupported. | changes.md:11; export:1117-1126, 1647-1664; plan:152-177 |

## Verbatim-mismatch quotes (check 1a)

Export, "Test comprehension before scoring" (Documentation/Reference/we're looking to prepare a grant application for h.md, lines 789-794):

> 1. Who in San Francisco benefits?
> 2. What problem does the project address?
> 3. What does the team actually deliver?
> 4. Why should that produce the claimed outcomes?
> 5. Why is the requested amount justified?
> 6. What remains after funding ends?

instructions.md §11.2 (lines 120-123), as executed:

> an unfamiliar reader restates the section without looking back and answers the six questions: who benefits, what problem, what the team delivers, why outcomes should follow, why the amount is justified, what remains after funding

| # | Export (verbatim) | §11.2 (executed) | Difference |
|---|---|---|---|
| 1 | Who in San Francisco benefits? | who benefits | "in San Francisco" dropped |
| 2 | What problem does the project address? | what problem | "does the project address" dropped |
| 3 | What does the team actually deliver? | what the team delivers | "actually" dropped; verb form changed |
| 4 | Why should that produce the claimed outcomes? | why outcomes should follow | reworded; causal framing weakened |
| 5 | Why is the requested amount justified? | why the amount is justified | "requested" dropped |
| 6 | What remains after funding ends? | what remains after funding | "ends" dropped |

The design authority required verbatim copying (plan §1.1: "Copy the wording of the six comprehension questions, the rubric-criterion names, and the five paragraph-acceptance questions verbatim from the Reference export"; plan §6: "Copy wording verbatim into §11.2") but its own blueprint block (plan lines 41-44) shows the compressed form, which the executor reproduced exactly. Either reading, the constitution's §11.2 does not contain the export's six questions verbatim.

## Verdict

**FAIL** - check 1a fails; the wording of the six comprehension questions in instructions.md §11.2 is not copied verbatim from the Reference export despite the design authority's explicit requirement. All other checks pass.

Single highest-priority defect: **§11.2's six comprehension questions are compressed paraphrases of the export's questions, not the required verbatim copy** - most materially, question 1 drops "in San Francisco" (the scope anchor of the export's own criteria) and question 4 replaces "Why should that produce the claimed outcomes?" with "why outcomes should follow", losing the causal framing the comprehension facet exists to test. Root cause is in the design authority: plan §1.1's verbatim instruction contradicts plan §1.1's own blueprint block (lines 41-44), which shows the paraphrase; the executor followed the blueprint. Resolution: revise the blueprint and §11.2 to the export's exact question wording (or, if compression is intended, strike the verbatim requirement from §1.1/§6 so the record stops claiming it).