# 003 - Review Revision: Verbatim Comprehension Questions, Run-Trigger Rule, and §9.2 Citation (Constitution §11)

> **For Hermes:** Execute this plan with subagent-driven development (one execute agent for the whole change). The orchestrator reviews and commits once per version. This change revises §11 of the constitution (F1) plus the two log/index rows; it does NOT run any review itself. Per the new §11.6 rule this change adds, a threefold review run is triggered for this change's own output - the orchestrator runs it after execution, before committing, with artifacts at `Documentation/Reviews/003-review-revision/`.

**Goal:** Revise constitution §11 so it carries the Reference export's six comprehension questions verbatim (§11.2), states when a review run starts and who starts it (new §11.6), and cites §9.2 for Editorial-class revisions (§11.4) - resolving review 002's FAIL (evidence check 1a) and the rubric's trigger and citation follow-ups.

**Scope - in:** the 4 files in Section 1 only.
**Scope - out:** the severity-vocabulary and facet-template items (deferred, Section 3); running any review (orchestrator step, Section 4 V7); any change to packet documents under `Documentation/Reference|Research|Prospectus|Refinement`, any README, or plan 002; git commits (orchestrator-only, §9.1).

---

## 1. Target file tree (this change)

| # | Path | Purpose |
|---|---|---|
| F1 | `Documentation/Logs/instructions.md` | Constitution revision: §11.2 comprehension bullet reworded to the export's verbatim questions; new §11.6 run-trigger subsection; §11.4 revision bullet gains the §9.2 citation. Modified. |
| F2 | `Documentation/Logs/changes.md` | One revision-record row for this change. Modified. |
| F3 | `Documentation/Plan/000-index.md` | Row 003 added. Modified. |
| F4 | `Documentation/Plan/003-review-revision.md` | This plan (written by the pre-plan agent). New. |

### 1.1 F1 - `Documentation/Logs/instructions.md` (three edits, nothing else)

**Edit A - §11.2 comprehension bullet.** Replace the current bullet (lines 120-123, quoted here as executed):

```
- Comprehension reviewer: an unfamiliar reader restates the section without
  looking back and answers the six questions: who benefits, what problem, what
  the team delivers, why outcomes should follow, why the amount is justified,
  what remains after funding.
```

with:

```
- Comprehension reviewer: an unfamiliar reader restates the section without
  looking back and answers the six questions:
  1. Who in San Francisco benefits?
  2. What problem does the project address?
  3. What does the team actually deliver?
  4. Why should that produce the claimed outcomes?
  5. Why is the requested amount justified?
  6. What remains after funding ends?
```

Rules: the lead-in ("an unfamiliar reader restates the section without looking back and answers the six questions:") stays byte-identical; the "six questions" count label stays, matching the six list items and §11.4's "all six questions". Copy the six question strings character-for-character from the Reference export, "Test comprehension before scoring" (lines 789-794) - do NOT copy them from this plan's quote (this plan's quote is reference; the export file is the source of truth). The numbered items are indented two spaces under the bullet, matching the file's continuation-line convention, so they render as a nested list. Nothing else in §11.2 changes.

**Edit B - new §11.6, appended after §11.5 (end of §11, end of file).** Add exactly:

```
### 11.6 Run trigger - when a review starts
- A review run starts for every change that modifies a document, before the
  version is committed: at each task's verification per plan 001 T01-T12 and
  at every later plan's execution (binding per plan 002 §2.1; the follow-on
  packet sweep runs per plan 002 §2.2).
- The orchestrator starts the run - assigns the three reviewers (§11.2) and
  adds the run's row to the master index (§11.3) - and the change's changes.md
  row is appended only after all three facets pass or a blocked status is
  recorded (§11.4).
```

**Edit C - §11.4 revision bullet (§9.2 citation).** In the revision bullet (current line 164), insert `(§9.2)` after "Editorial-class fixes":

```
- Revision runs through the standard cycle (§3): a pre-plan agent designs the
  revision (Editorial-class fixes (§9.2) may use an addendum to the producing
  plan), an execute agent implements it, then all three facets re-review.
```

This restores the citation plan 002's integration summary (§1.1, line 109) already claimed ("§11.4 cites §3 and §9.2"). Nothing else in §11.4 changes.

### 1.2 F2 - `Documentation/Logs/changes.md` row

Append one row (same columns as the existing table). Date = the execution date (orchestrator commit date), not the plan date.

| 2026-10-14 | Clarifying | Constitution §11: §11.2 comprehension questions copied verbatim from the Reference export; new §11.6 run-trigger rule; §11.4 cites §9.2 | fix review 002's FAIL (evidence check 1a) and the rubric's trigger/citation follow-ups: the constitution must quote the export's comprehension questions verbatim and state when review runs start | - | Adopt the corrected §11 (verbatim questions; run trigger; §9.2 citation) | Logs/instructions.md (§11.2 block, new §11.6, §11.4 citation), Plan/000-index.md | 003 |

Class = Clarifying per §9.2 ("adds missing information") - the same class the rubric's consistency note suggested for the 002 row.

### 1.3 F3 - `Documentation/Plan/000-index.md` row 003

| 003 | `Documentation/Plan/003-review-revision.md` | Review revision: verbatim comprehension questions, run-trigger rule, §9.2 citation (constitution §11) | planned | Flipped to "committed" by the orchestrator in this version's single commit |

### 1.4 F4 - this plan

Self-referential; no action.

---

## 2. Design decisions

- **Run-trigger placement: new §11.6, not a line in §11.1.** §11's subsections are single-topic, each header naming its subject (Granularity, roles, artifacts, pass rules, paragraph acceptance). The trigger is a lifecycle rule - when a run starts and who starts it - not a granularity rule, so placing it under 11.1's "Granularity - sections are the unit of work" header would bury it under the wrong topic and overload that subsection. It gates the pass/iteration rules (§11.4) and the master-index row (§11.3), so it reads naturally at the end of the section; appending as 11.6 renumbers nothing and breaks no existing cross-reference. It also answers the rubric's Completeness follow-up verbatim ("who initiates a run and when"): 11.6 states both - when (every document-modifying change, before the version commits; plan 002 §2.1/§2.2 binding folded in) and who (the orchestrator, with the §11.2/§11.3/§11.4 hooks).
- **Verbatim block form: numbered sub-list, not inline prose.** The export itself presents the questions as a numbered list (lines 789-794); reproducing that block keeps the six strings character-for-character in source order and makes the verbatim requirement machine-checkable (the block diffs directly against the export's lines). Splicing the questions into a prose line would invite re-paraphrase - the exact defect 003 fixes.
- **Scope guard.** Exactly three text edits in F1 (Edit A block, Edit B addition, Edit C line) plus the two index rows. The §11.2 lead-in, §11.4's other bullets, §11.3, §11.5, and all other sections are untouched. The severity/template items are deliberately NOT touched (Section 3).
- **Self-consistency.** 003 modifies a document, so per its own new §11.6 a review run is triggered for it; the orchestrator runs that review after execution (V7), exercising the rule on its first change.

---

## 3. Deferred follow-ups (recorded here; NOT part of this change)

| # | Item | Source | Why deferred |
|---|---|---|---|
| 1 | Severity vocabulary for the §11.3 findings table (allowed values "blocker\|minor" defined only in plan 002 §3's template) | Rubric, Enforceability (a) | Separate Clarifying change; 003 does not touch §11.3 |
| 2 | Facet-file template (comprehension/rubric/evidence artifact schema) lives only in plan 002 §3 | Rubric observation | Decision whether the constitution should own the template is a separate change |
| 3 | Comprehension pass test "without looking back" is self-attested, not mechanically checkable | Rubric, Enforceability (c) | Needs a checkable proxy; separate change |
| 4 | Plan-index status semantics: row 002 shows "planned" though executed (evidence check 4's minor note) | Evidence, check 4 | Design-level; reconcile statuses in a later change |
| 5 | Sweep numbering: plan 002 §2.2 names the follow-on packet sweep "003-review-sweep", now taken by this change - the sweep plan becomes `004-review-sweep` when written | Plan 002 §2.2 | Orchestrator note for the sweep-plan author; plan 002 is committed history, not edited |
| 6 | Changes.md row 002 class Foundational vs §9.2's Clarifying arguably fitting better | Rubric, Consistency (b) | Recorded; no action in 003 |
| 7 | Run-compliance path observation: review 002's artifacts sit one level up from §11.3's literal `<section-slug>/` path | Rubric, run-compliance note | Orchestrator decides whether §11.3's path rule is literal; record in the run index |

---

## 4. Verification - how the executor proves the change is correct

Run in order; every check must pass before handoff.

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | Six comprehension questions verbatim, word-for-word vs the export | For each of the six strings, `grep -Fc "<question>" Documentation/Logs/instructions.md` (six runs, e.g. `grep -Fc "Who in San Francisco benefits?" ...`); then compare the §11.2 numbered block against `sed -n '789,794p' "Documentation/Reference/we're looking to prepare a grant application for h.md"` | Each of the six strings has ≥ 1 hit in instructions.md; the §11.2 block matches Section 1.1 Edit A exactly; each §11.2 list item equals the export line with the same number, character-for-character (San Francisco anchor and "?" included); the lead-in still reads "answers the six questions:" with exactly six items | 
| V2 | Run-trigger rule present | `grep -nE '^### 11\\.6' Documentation/Logs/instructions.md`; `grep -Fc "A review run starts for every change that modifies a document" Documentation/Logs/instructions.md`; `grep -Fc "The orchestrator starts the run" Documentation/Logs/instructions.md` | One line `### 11.6 Run trigger - when a review starts`; both 11.6 bullets present, matching Edit B; 11.6 is the last subsection of §11 (end of file) |
| V3 | §9.2 citation present | `grep -n '§9\\.2' Documentation/Logs/instructions.md` | A hit `(§9.2)` inside the §11.4 revision bullet (`Editorial-class fixes (§9.2)`); §9.2's Editorial-class row exists (line 87); no other new §9.2 hit |
| V4 | No other section changed | `git status --porcelain`; `git diff Documentation/Logs/instructions.md` | File list shows exactly F1-F4 touched by this change (beyond the pre-existing change-002 files and review artifacts, which remain untouched); the instructions.md diff contains exactly three hunks - the §11.2 block (Edit A), the appended §11.6 (Edit B), and the §11.4 line (Edit C); no packet file, README, or deletion |
| V5 | Tables render | Programmatic pipe-count check on `Documentation/Logs/changes.md` and `Documentation/Plan/000-index.md` (every row equals the header's pipe count; separator row present); re-check the unchanged instructions.md tables | changes.md 8 pipes per row (new row included); 000-index.md 4 pipes per row (row 003 included); no malformed row |
| V6 | No prohibited words in the new text | `grep -niE 'revolutionary|world-class|unique|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Logs/instructions.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits except the two pre-existing exceptions: "transformative ambition" in §11.2 (official criterion name; "transform" is a substring) and §6's own list block (§6 lines 49-54) |
| V7 | Orchestrator, after handoff | Run the threefold review of the revised §11 per §11.6 (artifacts at `Documentation/Reviews/003-review-revision/`); then one commit: `git add` F1-F4; `git commit -m "docs(grant): revise review model - verbatim comprehension questions, run trigger, §9.2 citation"` | All three facets pass on the revised §11; exactly one commit; tree clean afterwards |

---

## 5. Executor inputs (not derivable from this plan - read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| Six comprehension questions | Reference export, "Test comprehension before scoring" (lines 789-794): `1. Who in San Francisco benefits?` `2. What problem does the project address?` `3. What does the team actually deliver?` `4. Why should that produce the claimed outcomes?` `5. Why is the requested amount justified?` `6. What remains after funding ends?` | Copy character-for-character into §11.2 (Edit A); the export file is the source of truth, this plan's quote is reference |
| Current §11.2 bullet and §11.4 revision bullet | `Documentation/Logs/instructions.md` lines 120-123 and 163-165 (both quoted in Section 1.1) | Edit A replaces the first; Edit C inserts `(§9.2)` into the second |
| §9.2 change-class model | `Documentation/Logs/instructions.md` §9.2 (Editorial row, line 87) | Citation target for Edit C; class justification for the changes.md row |
| Prohibited-words pattern | `Documentation/Logs/instructions.md` §6 (lines 49-54) | V6's pattern; "unique" is in §6's list, include it |
| Changes.md row date | Execution date (orchestrator commit date) | Precedent: seed rows and row 002 use commit dates |
| Plan-index row conventions | `Documentation/Plan/000-index.md` rows 001-002 | Row 003 mirrors them; status `planned` (orchestrator flips to `committed` at commit) |
| Export question lines | `Documentation/Reference/we're looking to prepare a grant application for h.md` | V1 compares §11.2 against lines 789-794 |

No review is run by this change itself; its own threefold review is the orchestrator's V7 step.