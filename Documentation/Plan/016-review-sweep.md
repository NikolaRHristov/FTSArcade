# Plan 016 - Per-Section Threefold Review Sweep of the Pre-Review Packet Files

## Goal

Run the constitution §11 threefold review (comprehension / rubric / evidence reviewers)
over the five packet files that were built by the original fan-out BEFORE the review
model existed and were never threefold-reviewed:

- `Documentation/Prospectus/00-prospectus.md`
- `Documentation/Prospectus/01-source-case.md`
- `Documentation/Prospectus/03-registers.md`
- `Documentation/Prospectus/04-delivery-and-budget.md`
- `Documentation/Prospectus/05-durability-risks-rights.md`

This plan designs the sweep only (run binding: constitution §11.6, "the follow-on
packet sweep runs per plan 002 §2.2"). It modifies no packet document. The reviews
themselves and any revision fixes are separate subsequent changes.

**Excluded from this sweep:** `02-claim-ledger.md` and `06-`/`10-narrative.md`
(built and reviewed under the review model, runs 010-013); `README.md`,
`Prospectus/README.md`, `Refinement/` (runs 004/005/014/015 covered their review
sub-scopes). A unit is a file or one `##` section of a file, per §11.1, with the
mandated relaxation that a short file (≤ ~100 lines) is one whole-file unit.

## 1. Unit table (18 units)

| File | Unit (section) | Unit slug | Review batch |
|---|---|---|---|
| 00-prospectus.md | §1 Decision summary | 00-prospectus-1-decision-summary | 2 |
| 00-prospectus.md | §2 Need | 00-prospectus-2-need | 3 |
| 00-prospectus.md | §3 Solution | 00-prospectus-3-solution | 3 |
| 00-prospectus.md | §4 Change mechanism | 00-prospectus-4-change-mechanism | 3 |
| 00-prospectus.md | §5 San Francisco execution | 00-prospectus-5-san-francisco-execution | 4 |
| 00-prospectus.md | §6 Evidence | 00-prospectus-6-evidence | 4 |
| 00-prospectus.md | §7 Measurement | 00-prospectus-7-measurement | 4 |
| 00-prospectus.md | §8 Financial plan | 00-prospectus-8-financial-plan | 5 |
| 00-prospectus.md | §9 Durability | 00-prospectus-9-durability | 5 |
| 00-prospectus.md | §10 Governance and risk | 00-prospectus-10-governance-and-risk | 5 |
| 00-prospectus.md | §11 Blocking unknowns | 00-prospectus-11-blocking-unknowns | 6 |
| 01-source-case.md | Whole file (2 short §) | 01-source-case | 2 |
| 03-registers.md | §1 Decision register | 03-registers-1-decision-register | 1 |
| 03-registers.md | §2 Data dictionary | 03-registers-2-data-dictionary | 1 |
| 03-registers.md | §3 Evidence register | 03-registers-3-evidence-register | 1 |
| 03-registers.md | §4 Contradiction audit checklist | 03-registers-4-contradiction-audit-checklist | 2 |
| 04-delivery-and-budget.md | Whole file (short) | 04-delivery-and-budget | 6 |
| 05-durability-risks-rights.md | Whole file (short) | 05-durability-risks-rights | 6 |

**Total: 18 units** (00=11 sections, 01=1, 03=4, 04=1, 05=1). All slugs unique.

## 2. Sequencing and batching

Order follows dependency: registers/source-case first (their decisions, dictionary,
and evidence propagate into every other file), then the prospectus master (read
order §1→§11), then delivery/budget and durability/risks/rights (they frame, carry
zero figures, and reference 03/00).

| Batch | Units | Reviewer agents (3 per unit, parallel) | Why this order |
|---|---|---|---|
| 1 | 03-registers-1, -2, -3 | 9 | Propagation root: decision register, data dictionary, evidence register |
| 2 | 03-registers-4, 01-source-case, 00-prospectus-1 | 9 | Close registers + source facts, then decision summary (depends on them) |
| 3 | 00-prospectus-2, -3, -4 | 9 | Need → Solution → Change mechanism (read order) |
| 4 | 00-prospectus-5, -6, -7 | 9 | Execution → Evidence → Measurement |
| 5 | 00-prospectus-8, -9, -10 | 9 | Financial plan → Durability → Governance and risk |
| 6 | 00-prospectus-11, 04-delivery-and-budget, 05-durability-risks-rights | 9 | Blocking unknowns, then the two framing workbooks last |

6 batches × 3 units = 18 units; 54 reviewer runs; 6 consolidation passes.
Batches run strictly sequentially (dependency + consolidation between batches).
Within a batch: 3 reviewer agents per unit run in parallel; the 3 units of a batch
run in parallel where agent capacity allows, otherwise unit-by-unit inside the batch.

## 3. Review-run procedure

### 3.1 Run identity and artifact paths (one run for the whole sweep)

- Run directory: `Documentation/Reviews/016-review-sweep/` (convention §11.3:
  `<NNN>-<slug>` = the plan whose execution the review verifies).
- Per unit: `Documentation/Reviews/016-review-sweep/<doc-slug>[-<unit-slug>]/`
  with `comprehension.md`, `rubric.md`, `evidence.md` - one file per facet;
  the document-slug prefix applies because this run reviews sections from more
  than one document (Reviews/README convention). Whole-file units use the bare
  document slug, e.g. `016-review-sweep/01-source-case/`.
- Rounds append in the SAME files (round header + round's findings appended);
  never rewrite, never delete; superseded findings stay (audit trail, §11.3).
- Run index: `Documentation/Reviews/016-review-sweep/index.md` - one row per
  unit: unit \| comprehension \| rubric \| evidence \| rounds \| status \| pass date.
  Statuses: pending → in review → in revision → passed \| blocked (Reviews/README).
- Master index: the orchestrator adds the run's row to
  `Documentation/Reviews/README.md` when the run starts (§11.6).

### 3.2 Executor flow per batch

1. **Start**: orchestrator creates the run directory + `index.md` (all 18 rows,
   status pending), adds the master-index row.
2. **Spawn reviewers**: per unit, 3 reviewer agents run independently and in
   parallel - comprehension, rubric, evidence (§11.2). Each agent brief carries:
   role facet and its ordered steps; unit target (file, section, line range,
   paragraph list); artifact path; round number; the §11.3 facet-file format
   (reviewer, date, round, findings table: paragraph \| finding \| rule violated \|
   severity, verdict PASS/FAIL); that unit's pass rules (§11.4); the no-edit rule.
3. **Review discipline**: every paragraph of the unit is reviewed in reading
   order - never skip, sample, or merge (§11.1); the five acceptance questions of
   §11.5 are applied per paragraph; reviewers never edit the section.
4. **Consolidate (orchestrator, after the batch)**: read all 9 facet files; update
   the run index rows for the batch's units. A unit passes only when all three
   facets PASS in the SAME round; any single FAIL sends the unit to revision.
   The orchestrator never overrides a reviewer's FAIL without a new round (§11.4).
5. **Revision flow for FAIL units** (§11.4, standard cycle §3): a pre-plan agent
   designs the fix as a NEW plan file (Editorial-class fixes may use an addendum
   to plan 016, §9.2); an execute agent implements it; then all three facets
   re-review the SAME unit - re-review is scoped to the failed unit, round N+1
   appended to the same facet files.
6. **Round cap**: three rounds per section per facet. After round 3 with any facet
   failing, status becomes **blocked** and the orchestrator chooses: a new plan,
   a section cut (page-budget rule), or a recorded `[INFORMATION NEEDED]` (§11.4).
7. **Dependency re-review**: a revision to a source unit (03-registers, 01) may
   force scoped re-review of downstream units that cited it; the revision plan
   names those units - never re-review silently.
8. **Close**: every unit passed or blocked; run index finalized (pass/blocked
   dates), master-index row updated. A change's changes.md row is appended only
   after all its facets pass or a blocked status is recorded (§11.6).

The sweep **finds and records** defects in the run artifacts; fixes are never
silent edits - they go through revision changes with their own changes.md rows.

## 4. Expected findings categories

The five files predate the review model, so the sweep is expected to surface
pre-review-era content that lacks current marker discipline:

| # | Category | Marker of the defect (per §5-§7, §11.5) |
|---|---|---|
| F1 | Ungraded claims | Material claim with no E1-E5 grade, or grade higher than the evidence supports (grades move down, never up) |
| F2 | Bare links / missing source status | URL without retrieval date/status, without a data-dictionary or evidence-register entry |
| F3 | Prohibited words & uncertainty language | §6 words/phrases; claims stated as fact where evidence is below E3 (verbatim phrases §5 missing) |
| F4 | Marker discipline gaps | `[INFORMATION NEEDED]` not in verbatim format (owner; why; decision blocked); partner names without status (confirmed / in discussion / proposed) |
| F5 | Unmarked figures / budget-test failures | Numbers or promised outputs without data-dictionary backing or a named cost line / zero-cost explanation (§7 budget test) |
| F6 | Paragraph-acceptance failures (§11.5) | First sentence does not state the claim, claim not traceable, certainty mislabeled, more than one idea, deletion removes tone not information |
| F7 | Editing-test violations (§7) | Ownerless actions, causal verbs without evidence grades, durability/beneficiary gaps (deletion/substitution/owner/evidence tests) |
| F8 | Cross-file consistency | Decision states (DR-01/06/07/11, etc.) in 00 vs 03; claim counts and conflict refs (C1-C6); status fields synced by change 015 vs older content |

Honest expectation: several units carry pre-review-era prose and will FAIL at
least one facet in round 1 - that is the sweep's purpose. A nonzero FAIL count in
the run index is a success signal, not a regression. Sections partially reviewed
under runs 004-007/015 (sub-scope changes only) are reviewed in full here,
including their unreviewed paragraphs.

## 5. changes.md row (appended at execution)

| Date | Change class | What changed | Why | Evidence/budget affected | Decision | Documents updated | Plan ref |
|---|---|---|---|---|---|---|---|
| 2026-10-15 | Clarifying | Design the follow-on per-section threefold review sweep of the five pre-review packet files (00-prospectus, 01-source-case, 03-registers, 04-delivery-and-budget, 05-durability-risks-rights): 18 review units (00=11 sections, 03=4, 01/04/05 whole-file units), 6 batches of 3 units in dependency order (registers/source-case → prospectus → delivery/budget → durability/risks/rights), single review run `Documentation/Reviews/016-review-sweep/` with per-unit artifact dirs and run index; executor flow: 3 reviewers per unit in parallel, orchestrator consolidates per batch, FAIL units re-review scoped through the standard pre-plan→execute revision cycle (§11.4; max 3 rounds per facet, then blocked) | The five files predate the review model (constitution §11) and were never threefold-reviewed; the sweep finds and records defects in run artifacts - fixes go through revision changes, no packet content is changed by this plan | None - no new figures, no budget lines; this plan modifies no packet document | Recorded: sweep plan adopted as change 016; the reviews and any fixes are separate subsequent changes | Documentation/Plan/016-review-sweep.md (new), Logs/changes.md, Plan/000-index.md | 016 |

## 6. Plan index row (000-index.md, INSIDE the Index table after row 015)

| 016 | `Documentation/Plan/016-review-sweep.md` | Review sweep: per-section threefold review of the five pre-review packet files (00/01/03/04/05) - 18 units, 6 batches, run 016-review-sweep | planned | Plan file only; sweep execution and fixes are follow-on changes |

## 7. Verification (pass rules)

| # | Check | Pass rule |
|---|---|---|
| V1 | Unit table complete | Exactly 18 units: 00=11, 01=1, 03=4, 04=1, 05=1; every unit slug unique; every row carries file \| unit \| slug \| batch |
| V2 | Every target file covered | All five file stems appear in the File column; exclusions (02, 06-10, READMEs, Refinement) stated explicitly |
| V3 | Artifact paths follow convention | Every unit's artifact dir matches `Documentation/Reviews/016-review-sweep/<doc-slug>[-<unit-slug>]/` with `comprehension.md`/`rubric.md`/`evidence.md`; run `index.md` at run root; master-index row added to `Reviews/README.md` when the run starts |
| V4 | Revision flow documented | §11.4 cycle named: pre-plan→execute per FAIL unit, scoped re-review, 3-round cap per facet, blocked status, orchestrator consolidates and never overrides a FAIL without a new round |
| V5 | No file modified by this plan itself | `git status --porcelain` shows only the new `Documentation/Plan/016-review-sweep.md`; no packet, log, or index file touched by this pre-plan step |
| V6 | Sequencing respects dependencies | Batches ordered registers/source-case → prospectus → delivery/budget → durability/risks/rights (batch table §2) |