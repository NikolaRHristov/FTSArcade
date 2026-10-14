# 002 - Review Model: Threefold Review of Every Section (Constitution §11)

> **For Hermes:** Execute this plan with subagent-driven development (one execute agent for the whole change). The orchestrator reviews and commits once per version. This change amends the constitution only; it does NOT run any review and does NOT change any packet document. Review runs happen in later plans (Section 2.2).

**Goal:** Amend the repo constitution with §11 - a threefold review model in which every document section is reviewed by three separate agents (comprehension, rubric, evidence), iteratively through the standard pre-plan → execute cycle until all three pass, with tracked artifacts - so the grant packet becomes review-proof before submission.

**Scope - in:** the 5 files in Section 1 only.
**Scope - out:** running any review (the first runs happen at T01-T12 verification and the follow-on sweep, Section 2); any change to packet documents under `Documentation/Reference|Research|Prospectus|Refinement` or any README file; changing the task text of plan 001 (T01-T12 apply §11 at execution, per Section 2.1); email or promotional drafting (protocol R1); git commits (orchestrator-only, rule R2).

---

## 1. Target file tree (this change)

| # | Path | Purpose |
|---|---|---|
| F1 | `Documentation/Logs/instructions.md` | Constitution amendment: new §11 (threefold review model); one line added to §3 (delegation model); one row added to the §10 file map. Modified. |
| F2 | `Documentation/Reviews/README.md` | Master review index: the convention for the tracked review-artifacts directory, created empty of runs. New. |
| F3 | `Documentation/Logs/changes.md` | One revision-record row for this change. Modified. |
| F4 | `Documentation/Plan/000-index.md` | Row 002 added. Modified. |
| F5 | `Documentation/Plan/002-review-model.md` | This plan (written by the pre-plan agent). New. |

### 1.1 F1 - new §11 in `Documentation/Logs/instructions.md`

Insert after §10 (end of file). Headers verbatim; each subsection 3-8 lines, imperative, enforceable - same register as the existing numbered sections. Copy the wording of the six comprehension questions, the rubric-criterion names, and the five paragraph-acceptance questions verbatim from the Reference export (Section 6 gives the source lines).

```
## 11. Review model - threefold review of every section

### 11.1 Granularity - sections are the unit of work
- Split every document into review sections: each existing ## heading is one
  section; where a page budget applies, each budgeted page starts a new section.
- Review every paragraph inside a section individually, in reading order; never
  skip, sample, or merge paragraphs.
- A section is reviewed, revised, and re-reviewed on its own; never batch two
  sections into one review.
- Slugify every section heading (lowercase, hyphens) for artifact naming (§11.3).

### 11.2 The three reviewer roles
- One section's review consists of THREE separate review agents, run
  independently: comprehension, rubric, evidence.
- Comprehension reviewer: an unfamiliar reader restates the section without
  looking back and answers the six questions: who benefits, what problem, what
  the team delivers, why outcomes should follow, why the amount is justified,
  what remains after funding.
- Rubric reviewer: scores the section 1-5 on the four rubric criteria
  (transformative ambition, viability, evidence of results, durability),
  justifies each score, and names the strongest claim, the most important
  unsupported assumption, the main execution risk, and what would raise each
  score.
- Evidence reviewer: checks every factual, partnership, budget, legal, and
  outcome claim against the source case; verifies evidence grades (§5), figures
  against the data dictionary, no silent inference, no prohibited words (§6),
  and the editing tests (§7).
- Each reviewer runs the named steps of its facet in order and writes one
  artifact per round (§11.3); reviewers never edit the section - findings and
  verdicts only.

### 11.3 Review artifacts
- Every round writes to Documentation/Reviews/<NNN>-<slug>/<section-slug>/:
  comprehension.md, rubric.md, evidence.md - one file per facet per section;
  rounds append, never rewrite.
- Each facet file records: reviewer, date, round, findings table
  (paragraph | finding | rule violated | severity), and verdict PASS or FAIL.
- Each run's index Documentation/Reviews/<NNN>-<slug>/index.md holds one row per
  section: section | comprehension | rubric | evidence | rounds | status |
  pass date.
- The master index Documentation/Reviews/README.md holds one row per review run;
  add the row when the run starts.
- Superseded findings stay in the files (audit trail); delete nothing after a
  round.

### 11.4 Pass rules and iteration
- Comprehension passes when the reviewer answers all six questions without
  looking back and each answer names the beneficiary, action, responsible
  party, evidence basis, and limitation without inference.
- Rubric passes when all four criteria carry a score with justification and
  every named blocker ("what would raise the score") is answered in the section
  or recorded as [INFORMATION NEEDED: <owner>; why; decision blocked].
- Evidence passes when every material claim has an evidence grade and source,
  no E5 claim remains, figures match the data dictionary, and no prohibited
  word (§6) or failed editing test (§7) remains.
- A section passes only when all three facets pass in the SAME round; a single
  FAIL sends the section back to revision.
- Revision runs through the standard cycle (§3): a pre-plan agent designs the
  revision (Editorial-class fixes may use an addendum to the producing plan),
  an execute agent implements it, then all three facets re-review.
- Rounds are capped at three per section per facet; after round three with any
  facet failing, status becomes blocked and the orchestrator chooses: a new
  plan, a section cut (page-budget rule), or a recorded [INFORMATION NEEDED].
- The orchestrator records pass and blocked statuses in the run index; it never
  overrides a reviewer's FAIL without a new round.

### 11.5 Paragraph acceptance - five questions per paragraph
- Review every paragraph with five yes-or-no questions: (1) does the first
  sentence state its claim, (2) can the claim be traced, (3) is its certainty
  correctly labeled, (4) does it add exactly one new idea, (5) would deleting
  it remove useful information rather than tone.
- Retain the paragraph only if all five answers are yes; any no is a finding
  naming the failed question.
```

Two small edits to the same file:

- **§3 (Delegation model)** - add one bullet after the orchestrator bullet:
  `- review agents: three independent reviewers per section (comprehension, rubric, evidence - see §11); they report findings and verdicts only, never revise content.`
- **§10 (File map)** - add one row to the table:
  `| Documentation/Reviews/ | Threefold review artifacts: comprehension.md, rubric.md, evidence.md per section; run + master indexes (§11) |`

Cross-references (integration points): §11.2 cites §5, §6, §7; §11.4 cites §3 and §9.2 (revision plans carry a change class); §11.5 copies the export's paragraph-acceptance wording; §10 row cites §11; §3 line cites §11.

### 1.2 F2 - `Documentation/Reviews/README.md` (master review index; new)

```
# Reviews - Threefold Review Artifacts

Purpose: every review run of every document section lives here, one run per
producing plan. Convention (constitution §11):
- Run directory: Documentation/Reviews/<NNN>-<slug>/ where <NNN>-<slug> is the
  plan whose execution the review verifies.
- Per section: <section-slug>/comprehension.md, <section-slug>/rubric.md,
  <section-slug>/evidence.md (prefix the document slug when a run reviews
  sections from more than one document).
- Run index: <NNN>-<slug>/index.md - one row per section.
- Statuses: pending -> in review -> in revision -> passed | blocked.

## Index
| Run | Plan ref | Document(s) | Sections | Status | Pass date |
|---|---|---|---|---|---|
(no runs yet - first runs occur at T01-T12 verification and the follow-on sweep)
```

### 1.3 F3 - `Documentation/Logs/changes.md` row

Append one row (same columns as the existing table). Date = the execution date (orchestrator commit date), not the plan date.

| 2026-10-14 | Foundational | Constitution §11: threefold review model (comprehension, rubric, evidence reviewers; tracked artifacts; iterative pass rules) | encode the export's "Review before submission" as a permanent operating rule so every section becomes a reviewed unit of work | - | Adopt threefold section review for all documents | Logs/instructions.md (§3 line, §10 row, new §11), Reviews/README.md, Plan/000-index.md | 002 |

Class = Foundational because it amends the constitution's operating rules - the same class as the scaffold that created them (plan 001, changes.md row 2).

### 1.4 F4 - `Documentation/Plan/000-index.md` row 002

| 002 | `Documentation/Plan/002-review-model.md` | Review model: threefold review of every section (constitution §11) | planned | Flipped to "committed" by the orchestrator in this version's single commit |

### 1.5 F5 - this plan

Self-referential; no action.

---

## 2. Integration with the roadmap and the existing packet

### 2.1 How §11 binds T01-T12 (plan 001, Section 2)

Rule: at execution of every task T01-T12, the task's verification gains a threefold review per §11 of every section the task created or modified; the task's changes.md row is appended only after all three facets pass (or blocked status is recorded with the orchestrator's decision). The amended change cycle for every later change: pre-plan (designs the change AND names the sections to review) → execute (implements) → threefold review (three agents per section) → orchestrator consolidation (records verdicts in the run index; one commit per version) → changes.md row (appended once all facets pass).

| Task | Output file(s) | Sections reviewed at verification |
|---|---|---|
| T01 | `03-registers.md`, `00-prospectus.md`, root `README.md` | the decision-register entry section; the readiness and banner sections the decision changes |
| T02-T04 | `03-registers.md`, `01-source-case.md`, `00-prospectus.md` | the DR sections and the source-case/prospectus sections the decision bites |
| T05 | `06-participant-pathway.md` | every section of the new file |
| T06 | `07-platform-boundary.md` | every section of the new file |
| T07 | `02-claim-ledger.md` | the claim-ledger table section(s) |
| T08 | `08-first-year-operating-plan.md` | every section of the new file |
| T09 | `09-unit-cost-model.md` | every section of the new file |
| T10 | `10-narrative.md` | every section of the new file |
| T11 | `02-refinement-checklist.md` | the updated checklist section(s) |
| T12 | `Prospectus/README.md`, root `README.md`, `Plan/000-index.md` | the relabel/status section(s) |

Each task's producing plan names its run directory `Documentation/Reviews/<NNN>-<slug>/` when it is written; if a task plan omits it, the run directory takes the task's own plan number and slug.

### 2.2 The existing packet sweep - follow-on, not interleaved

The pre-existing files (Prospectus 00-05, Refinement 00-02, Research facts-pack/sources, the README files) get their section-by-section threefold review in a **follow-on sweep** - a dedicated plan (003-review-sweep) run after the build tasks complete and before the final audit sequence (eligibility → logic → evidence → operations → financial → traceability → compression → sign-off, per the export). Recommendation and justification:

- Sections a task touches are reviewed at that task's verification while the change is fresh; sweeping them again is double-handling. Interleaving would review old text that a task is about to rewrite.
- The sweep's findings route through the same revision cycle without racing in-flight build tasks (the export's cadence rule: one foundational decision per cycle).
- A dedicated sweep gives the final audit sequence stable, fully reviewed inputs. The sweep plan is written after this plan is approved (delegation rule R2); plan 002 does not design its file list.

### 2.3 The review pipeline (named steps - "split your steps")

| # | Step | Who | Output |
|---|---|---|---|
| 1 | Split | Orchestrator maps the document to sections (§11.1) | Section list |
| 2 | Assign | Orchestrator delegates three review agents per section | Assignments |
| 3 | Review | Each agent runs the named steps of its facet, writes its artifact | `comprehension.md` / `rubric.md` / `evidence.md`, round N |
| 4 | Consolidate | Orchestrator records verdicts in the run index | `index.md` rows |
| 5 | Revise | Findings route through pre-plan → execute (§11.4) | Revised section |
| 6 | Re-review | All three facets re-review the revised section | New round artifacts |
| 7 | Pass record | All three pass in one round → orchestrator marks the section passed | `index.md` status + pass date |

---

## 3. Review-artifacts directory design (recap for the executor)

| Item | Convention |
|---|---|
| Run directory | `Documentation/Reviews/<NNN>-<slug>/` - the plan whose execution the review verifies |
| Per-section files | `Documentation/Reviews/<NNN>-<slug>/<section-slug>/comprehension.md`, `rubric.md`, `evidence.md` (one file per facet per section; rounds append) |
| Section slug | The reviewed section heading, slugified; prefix the document slug when a run spans several documents |
| Run index | `Documentation/Reviews/<NNN>-<slug>/index.md` - one row per section: section | comprehension | rubric | evidence | rounds | status | pass date |
| Master index | `Documentation/Reviews/README.md` - one row per run: Run | Plan ref | Document(s) | Sections | Status | Pass date |
| Status lifecycle | pending → in review → in revision → passed \| blocked |

Facet-file template (each round appends one block): `# <Facet> review - <document> <section>` → `## Round <N> (<date>, reviewer <agent>)` → `### Findings` (table: `# | Paragraph/sentence | Finding | Rule violated | Severity (blocker|minor)`) → `### Verdict` (`PASS`/`FAIL`) → `### Facet answers` (comprehension: the six answers; rubric: table `Criterion | Score 1-5 | Justification | What would raise it`; evidence: table `Claim | Grade | Source | Status`).

## 4. Granularity rule (recap for the executor)

- Sections: each existing `##` heading in a document is one review section; where the export's page-budget table applies, each budgeted page is a section boundary even mid-heading.
- Paragraphs: every paragraph is reviewed individually against the five acceptance questions (§11.5); a failing paragraph is a finding naming the failed question, never a silent rewrite.
- Unit of work: a section is reviewed, revised, and re-reviewed on its own; two sections are never batched in one review.

---

## 5. Verification - how the executor proves the change is correct

Run in order; every check must pass before handoff.

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | §11 present with headers verbatim | `grep -nE '^## 11\.|^### 11\.[1-5]' Documentation/Logs/instructions.md` | 6 lines, each matching the blueprint's exact header strings (Section 1.1) |
| V2 | No prohibited words outside the allowed list | `grep -niE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Logs/instructions.md Documentation/Reviews/README.md` | 0 hits, except: the rubric-criterion name "transformative ambition" in §11.2 (the official criterion name; note "transformative" contains "transform") and §6's own list block, which is pre-existing |
| V3 | Tables render | For every markdown table in the changed files: header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each |
| V4 | Only the named files changed | `git status --porcelain` before and after; diff the file lists | Exactly F1-F5 touched: instructions.md modified (§11 added, §3 line, §10 row), Reviews/README.md added, changes.md modified (one row), 000-index.md modified (row 002), 002-review-model.md added; no packet file modified; no deletions |
| V5 | Reviews convention documented | `test -f Documentation/Reviews/README.md` and inspect it | File exists; contains the run-directory, per-section-file, and status-lifecycle lines and the Index table header from Section 1.2 |
| V6 | Cross-references present | Inspect instructions.md §11 and §10 | §11.2 cites §5, §6, §7; §11.4 cites §3 and §9.2; §10 table has the Documentation/Reviews row citing §11; §3 has the review-agents bullet |
| V7 | changes.md + plan-index rows present | Inspect both files | changes.md has exactly one new row with class Foundational and Plan ref 002; 000-index.md has row 002 with status `planned` (orchestrator flips to `committed` in the single commit) |
| V8 | One commit per version | Orchestrator, after handoff: `git add` F1-F5; `git commit -m "docs(grant): add threefold review model to the constitution"` | Exactly one commit; tree clean afterwards |

---

## 6. Executor inputs (not derivable from this plan - read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| Six comprehension questions + pass test | Reference export, "Test comprehension before scoring" (lines 785-798) and "Review before submission" (lines 1117-1126) | Copy wording verbatim into §11.2 |
| Four rubric-criterion names | Reference export, Evaluation Rubric (lines 544-610): Transformative Ambition, Viability, Evidence of Results, Durability | §11.2 names them |
| Paragraph-acceptance five questions | Reference export, "Paragraph acceptance" (lines 2090-2100) | Copy verbatim into §11.5 |
| Page-budget table | Reference export, "Page budget" (lines 1647-1664) | §11.1 references it; no need to copy the table itself |
| Data dictionary | `Documentation/Prospectus/03-registers.md` §2 (rule: every figure must appear there with one definition); cross-check rule also in `02-refinement-checklist.md` row 13 | §11.2/§11.4 evidence-facet checks point at it |
| Changes.md row date | Execution date (orchestrator commit date) | Seed rows use commit dates |
| Commit message | Section 5, V8 | Orchestrator's single commit |

No review is run by this change; the first runs occur when T01-T12 execute (Section 2.1) and in the follow-on sweep plan (Section 2.2).