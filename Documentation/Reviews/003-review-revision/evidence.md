# Evidence Review (Re-review) - Change 003 (Review Revision)

Reviewer: evidence facet (re-review). Date: 2026-10-14. Round: 1 (change 003 revision review, re-review of change 002's failed check 1a).

Scope: change 003 per `Documentation/Logs/changes.md` row 003 - verbatim §11.2 comprehension questions, new §11.6 run-trigger, §11.4 cites §9.2 - against the Reference export (`Documentation/Reference/we're looking to prepare a grant application for h.md`), the constitution (`Documentation/Logs/instructions.md`), and the design authority (`Documentation/Plan/003-review-revision.md`, `001-repo-scaffold.md`, `002-review-model.md`).

Method: direct reads of instructions.md §11 and the export lines 789-794; programmatic line-by-line byte comparison of the six questions; regex scan for §6 prohibited words across instructions.md, changes.md, 000-index.md; programmatic pipe-count check on every table row of instructions.md; existence check for the plan references named in §11.6 (plan 001 T01-T12; plan 002 §2.1, §2.2).

## Check table

| # | Check | Result | Detail | Location |
|---|---|---|---|---|
| 1 | §11.2 six comprehension questions character-for-character identical to export lines 789-794 | **PASS** | All six question strings are byte-identical to the export's lines 789-794. The only delta is two leading spaces per line in instructions.md (markdown list indentation under the "- Comprehension reviewer:" bullet); zero characters of the quoted question text differ. No words dropped or reworded (the change 002 check-1a failure mode). Quotes below. | instructions.md:122-127; export:789-794 |
| 2 | §11.6 run-trigger exists, is imperative, names the orchestrator as initiator | **PASS** | §11.6 "Run trigger - when a review starts" exists. Imperative: "A review run starts for every change that modifies a document, before the version is committed". Initiator named: "The orchestrator starts the run - assigns the three reviewers (§11.2) and adds the run's row to the master index (§11.3)". Trigger conditions are concrete (per plan 001 T01-T12; per plan 002 §2.1; follow-on sweep per plan 002 §2.2), not vague. | instructions.md:184-192 |
| 3 | §9.2 citation appears in the §11.4 bullet | **PASS** | §11.4 revision bullet carries an explicit pointer: "(Editorial-class fixes (§9.2) may use an addendum to the producing plan)". §9.2 defines Editorial with the meaning the bullet relies on. (Change 002's evidence noted the citation was implicit by term only; 003 makes it explicit.) | instructions.md:167-169; §9.2 at 83-92 |
| 4 | changes.md row 003 matches the change (Clarifying, plan ref 003) | **PASS** | Row 003: Date 2026-10-14, class Clarifying, Plan ref 003, Documents updated (Logs/instructions.md §11.2 block, new §11.6, §11.4 citation; Plan/000-index.md). Every listed document/row was verified present and matching; "Why" states the fix of review 002's FAIL (evidence check 1a) plus the trigger/citation follow-ups. | changes.md:12 |
| 5 | 000-index.md row 003 present | **PASS** | Row 003 exists with the correct plan file path (`Documentation/Plan/003-review-revision.md`), title ("Review revision: verbatim comprehension questions, run-trigger rule, §9.2 citation (constitution §11)"), and status "planned" (orchestrator flips to "committed" at commit - design-level convention, not a defect). | 000-index.md:11 |
| 6 | No prohibited words outside the §6 list | **PASS** | Full-file regex scan of instructions.md, changes.md, and 000-index.md for the §6 blacklist (revolutionary, world-class, unique, cutting-edge; empower/unlock/transform; scalable; sustainable; "partners include"; "data shows"): zero hits outside §6's own list (instructions.md lines 49-54). The §11.6 and §11.2 additions are clean. | grep result: 0 hits in all three files |
| 7 | Tables render (equal pipe counts) | **PASS** | Programmatic pipe-count check over instructions.md: 4 tables, 0 rows with mismatched pipe counts, every table has a separator row. changes.md (1 table, 8 rows) and 000-index.md (1 table, 3 rows) also uniform. | programmatic count: all files |
| 8 | No silent inference in the new text | **PASS** | §11.2 questions are verbatim quotes (no claims); §11.6's factual references are grounded: plan 001 contains tasks T01-T12 (verified T01..T12 present) and plan 002 contains §2.1 ("How §11 binds T01-T12 (plan 001, Section 2)") and §2.2 ("The existing packet sweep - follow-on, not interleaved"); §11.4's §9.2 pointer matches the §9.2 class table. Nothing claimed that the design does not support. | instructions.md:184-192; plan 001; plan 002:152, 171 |

## Verbatim quotes (check 1 - both sides)

Export, "Test comprehension before scoring" (lines 789-794):

> 1. Who in San Francisco benefits?
> 2. What problem does the project address?
> 3. What does the team actually deliver?
> 4. Why should that produce the claimed outcomes?
> 5. Why is the requested amount justified?
> 6. What remains after funding ends?

instructions.md §11.2 (lines 122-127), as executed:

>   1. Who in San Francisco benefits?
>   2. What problem does the project address?
>   3. What does the team actually deliver?
>   4. Why should that produce the claimed outcomes?
>   5. Why is the requested amount justified?
>   6. What remains after funding ends?

Difference: per line, two leading spaces only (list nesting); question text byte-identical. No word-level differences of the kind that failed check 1a in change 002 (e.g., question 1 retains "in San Francisco"; question 4 retains "Why should that produce the claimed outcomes?" with its causal framing).

## Verdict

**PASS** - all eight checks pass. Change 003 resolves change 002's single FAIL (check 1a): the six comprehension questions are now the export's verbatim wording, with only markdown indentation differing. No defect to rank.

Highest-priority note (non-blocking): the §11.2 question block is indented two spaces relative to the export's lines 789-794; if byte-exact parity of the block (including indentation) is later demanded, the indent can be dropped without changing any wording.