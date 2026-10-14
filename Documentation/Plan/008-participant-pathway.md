# 008 - Participant Pathway Framework: Who Participates, Entry Points, Step Table, Exit Points (T05)

> **For Hermes:** Execute this plan with an execute agent. Orchestrator reviews and commits once (`docs(grant): <change>`). This change creates `Documentation/Prospectus/06-participant-pathway.md` as a **structured framework - not a draft pathway** - because DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided as of 2026-10-14** (`03-registers.md` §1.1). The executor writes the framework, tables, and placeholders exactly as specified in Section 2; **inventing any pathway step, owner, or SF location is forbidden**.

**Goal:** Satisfy plan 001 task T05 (bucket CONTENT) by creating `Documentation/Prospectus/06-participant-pathway.md` - a STRUCTURED FRAMEWORK document: (1) participant definition carrying the DR-01 undecided state + options; (2) entry points; (3) pathway step table `step | who | action | owner | SF source | evidence grade`; (4) exit/drop-off points; (5) unknowns as `[INFORMATION NEEDED]`; plus a decision-gate note (the pathway becomes draftable once DR-01/DR-06/DR-07 close) - and appending the changes.md row and the 000-index.md row. No pathway content is invented: every intervention-specific cell is a placeholder or `[INFORMATION NEEDED: ...]` marker, and the document states plainly that no intervention is defined.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and the T05 task detail): no scope change occurs - no option of DR-01/DR-06/DR-07 is chosen or redefined; the change adds missing information (the pathway framework and the propagated decision states) and creates one new packet document. This mirrors the Clarifying precedent of changes 004/005/006/007, which recorded undecided decision states. Foundational would apply only if the decisions were made and changed scope; they are not. Operational would apply to delivery/budget numbers; the document adds none (zero dollar figures).

**Scope - in:** the 3 files listed in Section 1 (F2-F4) plus this plan file (F1, already written by the pre-plan agent).
**Scope - out:** choosing or recommending any option of DR-01/DR-06/DR-07; inventing pathway steps, owners, or SF locations; edits to `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `04-delivery-and-budget.md`, root `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/008-participant-pathway.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/06-participant-pathway.md` | **New file** (verified absent): the participant pathway framework - write the Section 2.2 content verbatim |
| F3 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 008) after the plan-007 row (currently line 16) |
| F4 | `Documentation/Plan/000-index.md` | Modify: append row 008, status `planned`, after the plan-007 row (currently line 15) |

---

## 2. F2 - `Documentation/Prospectus/06-participant-pathway.md` (NEW FILE)

### 2.1 File-level rules (binding)

- Write the file exactly as the fenced content in §2.2: headers verbatim, tables verbatim, cell text verbatim, relative links only. Do not add, remove, or reword any section, row, cell, or marker.
- All owners are **roles** (per `03-registers.md` rules: "All owners are roles; named persons are `[INFORMATION NEEDED: ...]`"). No person's name, no organization name (beyond the delivery-map role labels "named org (TBD)", "named team (TBD)", "named evaluator (TBD)"), and no SF location may be invented.
- No causal claims: the only causal wording is inside quoted decision-state references; no dollar figures.
- No prohibited words (instructions.md §6): revolutionary, world-class, unique, cutting-edge, empower, unlock, transform, scalable, sustainable, "partners include", "data shows" - 0 hits.
- Before writing the decision-state sentence in Section 1 and the gate references in Section 6, re-read `03-registers.md` §1.1 DR-01/DR-06/DR-07 entries; if the recorded wording drifted from what §2.2 quotes, stop and report - do not paraphrase or patch blind (mirrors plan 007's quote-fidelity rule).
- Cross-links to planned files (`07-platform-boundary.md`, `08-first-year-operating-plan.md`, `02-claim-ledger.md`) are plain backticked text, NOT markdown links - they do not exist yet, and dangling links fail V9.

### 2.2 Complete file content (write exactly this)

```
# Participant Pathway - FTSArcade / Boundless San Francisco

**Version:** S0 (framework only) · **Date:** 2026-10-14
**Status:** **FRAMEWORK ONLY - NOT DRAFTABLE.** As of 2026-10-14, DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided** (`03-registers.md` §1.1); no intervention is defined anywhere (`01-source-case.md` rows 1, 3, 5). Every intervention-specific cell below is a placeholder or `[INFORMATION NEEDED: ...]`; **no pathway step, owner, or SF location is invented.** The pathway becomes draftable only when the three scope-lock decisions close (Section 6).
**Purpose:** Define who participates, entry points, and the step-by-step pathway - with a named owner per step and SF grounding - as the **framework** the concrete intervention attaches to once DR-01/DR-06/DR-07 close. This file is the T05 deliverable of plan 001 (bucket CONTENT) and feeds T06 (platform boundary) and T08 (first-year operating plan).
**Sources:** `03-registers.md` §1.1 (DR-01/DR-06/DR-07 decision states), `01-source-case.md` rows 1/3/4/6, `04-delivery-and-budget.md` workstreams W-03/W-05/W-06/W-08/W-10, `../Research/facts-pack.md` facts #21 (25% SF-locality rule) and §(d) (platform facts).
**Cross-links:** planned files `07-platform-boundary.md` (T06), `08-first-year-operating-plan.md` (T08), `02-claim-ledger.md` (T07). All owners are roles (per `03-registers.md` rules); named persons are `[INFORMATION NEEDED: program lead; required to name the person for each role (owner test); blocks the whole document - DR-01]`.

## 1. Participant definition (from DR-01)

**Decision state (carried from `03-registers.md` §1.1, DR-01):** **Undecided as of 2026-10-14** - as of 2026-10-14, no packet document defines a beneficiary population: no population, inclusion/exclusion rules, geography, or estimated reachable population exists anywhere. The candidate options below are **options, not chosen**; no positive claim is made about who benefits.

| Option | Participant as the option defines them | What this option requires of the pathway | Status |
|---|---|---|---|
| (a) Creative workforce pathways | People entering structured game-development training, paid projects, and employment support | Training/placement steps; employer-demand evidence (E4, untested) | Recorded, not chosen |
| (b) Accessible community learning | People in facilitated digital-literacy and creative-technology programs | Facilitated-learning steps; accessibility testing (E4, untested) | Recorded, not chosen |
| (c) Community connection | People in recurring facilitated activities through neighborhood organizations | Recurring-activity steps; confirmed neighborhood partners (E4, untested) | Recorded, not chosen |
| (d) Public cultural-installation program | Users of free public cultural/recreational installations | Access rules, site plan, engagement steps (E4, untested; links to DR-06) | Recorded, not chosen |
| (e) None approved | No participant defined | No pathway | Recorded base case |

**Inclusion/exclusion rules:** `[INFORMATION NEEDED: program lead; required to define who is included and excluded per the DR-01 decision rule; blocks Section 1 - DR-01]`
**Geography:** `[INFORMATION NEEDED: program lead; required to name the SF geography and comply with the ≤25%-outside-SF rule (facts-pack #21, E1); blocks Section 1 - DR-01]`
**Reachable-population estimate (F-11):** `[INFORMATION NEEDED: program lead; required as the planning target with source and method; blocks Section 1 - DR-01]`
**Figure discipline (data dictionary, `03-registers.md` §2):** "participants", "beneficiaries", and "users" are not interchangeable; this document uses "participant" only for the enrolled population (F-01), never for website visitors (F-02).

## 2. Entry points

**Definition:** An entry point is the first action a participant takes on the pathway - the channel by which a person becomes a prospective participant. The table below is the entry-point **taxonomy** (decision-independent); the concrete entry points for the chosen beneficiary attach later (IN-03).

| Entry point | Who acts | What happens | SF source | Evidence grade |
|---|---|---|---|---|
| Passive discovery | Prospective participant | Person finds the platform/site and starts free play - web entry exists today | `../Research/facts-pack.md` §(d) fact 3: free play, no login or payment gate (E1) | E1 (entry-channel fact only); pathway effect ungraded - no claim |
| Active outreach | Program lead; recruitment org (named org TBD - W-05) | Program-led recruitment of the defined population | `[INFORMATION NEEDED: program lead; required to cite the city-source evidence grounding recruitment - DR-01]` | Ungraded - placeholder |
| Referral | Community or neighborhood organization (status: none confirmed) | Referral of prospective participants | `[INFORMATION NEEDED: program lead; required to cite the referral partner and its SF grounding - DR-01]` | Ungraded - placeholder |
| Open access / walk-in | Prospective participant | Arrival at a defined site or activity | `[INFORMATION NEEDED: program lead; required for the site plan - DR-06/DR-01]` | Ungraded - placeholder |

**Per-option entry-point specifics:** `[INFORMATION NEEDED: program lead; required to specify the concrete entry points for the chosen DR-01 option; blocks Section 2 - DR-01]`
**Recruitment workstream:** delivery-map W-05 (`04-delivery-and-budget.md` §1): output = eligible participants enrolled; responsible party = named org (TBD); start condition = access to population + agreed partner.

## 3. Pathway step table (step | who | action | owner | SF source | evidence grade)

**Reading note:** the table is the **framework**: the rows are the pathway stages - the decision-independent phases from `04-delivery-and-budget.md` W-03 (first contact → completion, with dose, setting, staffing, completion rule) plus endpoint and follow-up per the data dictionary (F-01/F-03/F-05). The action, owner, SF-source, and grade cells are placeholders; they become concrete only after DR-01/DR-06/DR-07 close (Section 6). Every party named is a **role**; named persons are `[INFORMATION NEEDED]` (IN-09).

| Step | Who | Action | Owner | SF source | Evidence grade |
|---|---|---|---|---|---|
| 1. First contact | Prospective participant | `[INFORMATION NEEDED: program lead; required to specify the concrete first-contact action once DR-01/DR-06/DR-07 close; blocks step 1 - DR-01/DR-06/DR-07]` | Program lead (named person IN-09); recruitment org (TBD - W-05) | Web entry: `../Research/facts-pack.md` §(d) fact 3 (E1); otherwise `[INFORMATION NEEDED: program lead; SF source per entry channel - DR-01]` | E1 (entry-channel facts only); cell otherwise ungraded - no claim |
| 2. Enrollment | Prospective participant | `[INFORMATION NEEDED: program lead; required to specify the enrollment action, data collected, and eligibility check per the DR-01 decision rule (≤25% rule, facts-pack #21, E1); blocks step 2 - DR-01]` | Program lead; named org (TBD - W-05) | `[INFORMATION NEEDED: program lead; SF-locality verification method - DR-01]` | Ungraded - placeholder |
| 3. Participation | Participant | `[INFORMATION NEEDED: program lead; required to specify dose, setting, and duration per the chosen intervention (source case row 3); blocks step 3 - DR-01/DR-05]` | Program lead; named team (TBD - W-06) | `[INFORMATION NEEDED: program lead; city-source evidence for the activity's SF grounding - DR-01]` | Ungraded - placeholder |
| 4. Completion | Participant | `[INFORMATION NEEDED: program lead; required to define the completion rule and endpoint (F-03); blocks step 4 - DR-05]` | Program lead | `[INFORMATION NEEDED: program lead; SF grounding of the completion record - DR-01]` | Ungraded - placeholder |
| 5. Follow-up / outcome measurement | Completer | `[INFORMATION NEEDED: named evaluator; required to specify the pre-registered outcome indicator (F-05) once DR-07 closes; blocks step 5 - DR-07/DR-05]` | Named evaluator (TBD - W-10) | `[INFORMATION NEEDED: named evaluator; measurement instrument and collection timing - DR-07]` | Ungraded - placeholder |

**Framework constraints (binding regardless of the intervention):**
- Dose, setting, and duration must be stated per step before any claim (source case row 3 completion test: "someone else could understand what happens").
- Completion must be defined before any completion figure is used (F-03: define acceptable absence before use).
- Outcome claims require a pre-registered indicator at capability/progression/system level; engagement metrics are never outcomes (DR-07 decision rule, `03-registers.md`).
- Geographic compliance: no more than 25% of project activities may benefit beyond SF city limits (facts-pack #21, E1); every step needs activity-level tagging (F-08).

## 4. Exit / drop-off points

**Definition:** Points where a participant leaves the pathway before completion, and the defined recording response. Exit accounting feeds F-03 (completion) and F-05 (outcome); exit events are never relabeled as outcomes (DR-07 decision rule).

| Exit point | Who | What is recorded | Owner | Data-dictionary figure | Evidence grade |
|---|---|---|---|---|---|
| Non-enrollment after first contact | Prospective participant | Contact without enrollment; reason (if given) | Program lead; named org (TBD - W-05) | F-01 (reach = enrolled; not website users) | Ungraded - placeholder |
| Drop-off mid-pathway | Participant | Last attended step; absence rule applied | Named team (TBD - W-06) | F-03 (completion rate; acceptable absence defined before use) | Ungraded - placeholder |
| Non-completion at endpoint | Participant | Endpoint not met; reason | Program lead | F-03 | Ungraded - placeholder |
| Withdrawal | Participant | Voluntary exit; date; reason (if given) | Program lead | F-03 | Ungraded - placeholder |
| Referral out | Participant | Referral to another service; destination status | Program lead; named org (TBD) | `[INFORMATION NEEDED: named evaluator; recording consent and instrument - DR-05]` | Ungraded - placeholder |

**Exit-point recording:** `[INFORMATION NEEDED: named evaluator; required to specify attendance/consent recording per exit point (data dictionary F-03, F-05); blocks Section 4 - DR-05]`
**Contradiction-audit constraints (`03-registers.md` §4):** beneficiary count must match enrollment capacity; evaluation measures must match promised outcomes; budget quantities must match delivery volume. The pathway's exit accounting must not contradict these rows once the delivery plan (T08) is built.

## 5. Unknowns - INFORMATION NEEDED list

| # | Unknown | Owner | Why | Decision blocked | Unblocks |
|---|---|---|---|---|---|
| IN-01 | Participant definition (population, inclusion/exclusion, geography) | Program lead | No beneficiary defined (DR-01 undecided as of 2026-10-14) | DR-01 | Section 1 |
| IN-02 | Reachable-population estimate (F-11) | Program lead | Planning target missing; no estimate with source and method | DR-01 | Section 1 |
| IN-03 | Concrete entry points per option | Program lead | Taxonomy exists; specifics need the chosen beneficiary | DR-01 | Section 2 |
| IN-04 | Concrete action per step (1-5) | Program lead | Intervention undefined (DR-01/DR-06/DR-07 open) | DR-01/DR-06/DR-07 | Section 3 |
| IN-05 | Dose, setting, duration | Program lead | Source case row 3 empty | DR-05 | Section 3 (step 3) |
| IN-06 | Completion rule and endpoint | Program lead | F-03 requires a defined endpoint | DR-05 | Section 3 (step 4) |
| IN-07 | SF grounding per step (city sources) | Program lead | Substitution test unsatisfiable without sources | DR-01 | Sections 2-3 |
| IN-08 | Exit-point recording (attendance, consent) | Named evaluator | F-03/F-05 need instruments and consent | DR-05 | Section 4 |
| IN-09 | Named person per role | Program lead | Owner test needs named parties | DR-01 | Whole document |
| IN-10 | Site plan (open-access entry) | Program lead + counsel | DR-06 frame requires a defined site plan | DR-06 | Section 2 |

## 6. Decision gate - when the pathway becomes draftable

The pathway **cannot be drafted while DR-01, DR-06, and DR-07 are undecided** (all recorded **undecided as of 2026-10-14**, `03-registers.md` §1.1; consequence of delay: all downstream work pauses; the packet stays Not ready). This document is the framework those decisions attach to.

**Gate:** DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) each closed in `03-registers.md` §1.1 with a decided value, deciding owner, date, and evidence grade (plans 001 T02-T04 recorded the undecided states; changes 005/006/007).

**Once the gate opens:** a follow-on plan (successor to this plan, still T05 content) replaces every placeholder and `[INFORMATION NEEDED]` cell in Sections 1-4 with concrete content, per delivery-map workstream W-03 (`04-delivery-and-budget.md` §1: start condition = scope lock W-02; output = one approved pathway with dose, setting, staffing, completion rule). This file is then re-verified with the full editing-test set (instructions.md §7).

**Until then:** no draftable pathway exists; this framework stands on its own - the deletion test passes (the framework does not depend on the FTSArcade name) and the substitution test passes (placeholder cells carry no invented SF facts).

## 7. Revision record (per methodology)

| Date | Proposed change | Class | Reason | Evidence affected | Budget affected | Decision | Updated documents |
|---|---|---|---|---|---|---|---|
| 2026-10-14 | Participant pathway framework created (framework-only: participant definition carries the DR-01 undecided state and options; entry-point taxonomy; step table format step \| who \| action \| owner \| SF source \| evidence grade; exit/drop-off points; INFORMATION NEEDED list; decision-gate note) | Clarifying | Plan 001 T05 (CONTENT) requires the pathway; the intervention is undefined while DR-01/DR-06/DR-07 are open, so the framework - not a pathway - is recorded | DR-01/DR-06/DR-07 decision states (E1, source: `03-registers.md` §1.1; ungraded - undecided); E1 platform facts (`../Research/facts-pack.md` §(d)); no new figures | None - zero dollar figures | No decision closed; pathway draftable only after DR-01/DR-06/DR-07 | 06-participant-pathway.md (new), Logs/changes.md, Plan/000-index.md |
```

### 2.3 INFORMATION NEEDED markers list (must appear in the file)

The file's Section 5 table (IN-01…IN-10) is the consolidated markers list; the complete inline marker texts appear in Sections 1-4 exactly as written in §2.2. Count: **20 inline `[INFORMATION NEEDED: ...]` markers** (1 in the preamble, 3 in Section 1, 4 in Section 2, 10 in the Section 3 step table, 2 in Section 4), each with owner + why + decision-blocked fields per instructions.md §5, each grouped into exactly one of: (the Status-line phrase "`[INFORMATION NEEDED: ...]`" is a format description, not a marker; `grep -c` on the file will read 21 hits including it - V3 accounts for this)

| ID | Owner | Decision blocked | Unblocks |
|---|---|---|---|
| IN-01 | Program lead | DR-01 | Section 1 (participant definition) |
| IN-02 | Program lead | DR-01 | Section 1 (reachable population, F-11) |
| IN-03 | Program lead | DR-01 | Section 2 (entry-point specifics) |
| IN-04 | Program lead | DR-01/DR-06/DR-07 | Section 3 (action per step) |
| IN-05 | Program lead | DR-05 | Section 3 (dose, setting, duration) |
| IN-06 | Program lead | DR-05 | Section 3 (completion rule, endpoint) |
| IN-07 | Program lead | DR-01 | Sections 2-3 (SF grounding per step) |
| IN-08 | Named evaluator | DR-05 | Section 4 (exit-point recording) |
| IN-09 | Program lead | DR-01 | Whole document (named persons) |
| IN-10 | Program lead + counsel | DR-06 | Section 2 (site plan) |

---

## 3. F3 - `Documentation/Logs/changes.md`

**Append one row after the plan-007 row (currently line 16), same column format (8 columns; pipes inside cells escaped as `\|` where the step-table format is named):**

```
| 2026-10-14 | Clarifying | Create participant pathway framework document (`Prospectus/06-participant-pathway.md`, new): framework-only - participant definition carries the DR-01 undecided state and options (recorded, not chosen); entry-point taxonomy; pathway step table format step \| who \| action \| owner \| SF source \| evidence grade with placeholder cells; exit/drop-off points; consolidated INFORMATION NEEDED list (IN-01-IN-10); decision-gate note (pathway draftable only after DR-01/DR-06/DR-07 close) | Plan 001 T05 (CONTENT) requires the participant pathway; DR-01/DR-06/DR-07 are all undecided as of 2026-10-14, so the change records the framework the intervention attaches to - no pathway step, owner, or SF location invented | DR-01/DR-06/DR-07 decision states propagated (E1, source: 03-registers.md §1.1; ungraded - undecided); E1 platform facts (facts-pack §(d) fact 3) used for the web-entry cell; no new figures; no budget affected | No decision closed - pathway stays not draftable until scope lock | Prospectus/06-participant-pathway.md (new), Logs/changes.md, Plan/000-index.md | 008 |
```

---

## 4. F4 - `Documentation/Plan/000-index.md`

**Append one row after the plan-007 row (currently line 15):**

```
| 008 | `Documentation/Plan/008-participant-pathway.md` | Participant pathway framework: who participates, entry points, step table, exit points (plan 001 T05) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 5. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T05: owner test; deletion test; evidence test; substitution test; plus the framework-honesty checks below. Per instructions.md §11.6, the orchestrator starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T05; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No invented pathway content | Read `Documentation/Prospectus/06-participant-pathway.md` against §2.2 of this plan | The file matches §2.2 verbatim: the only steps are the 5 framework stages (first contact, enrollment, participation, completion, follow-up/outcome measurement) and the 4 entry-point taxonomy rows; every intervention-specific cell is exactly the `[INFORMATION NEEDED: ...]` text or the "Ungraded - placeholder" wording specified; 0 concrete interventions, 0 named persons, 0 organization names beyond the delivery-map "TBD" role labels, 0 SF locations appear anywhere |
| V2 | Undecided states propagated | `grep -c "undecided as of 2026-10-14" Documentation/Prospectus/06-participant-pathway.md` + inspect §1/§6 | ≥ 3 hits (DR-01, DR-06, DR-07); "recorded, not chosen"/"options, not chosen" language present in §1; no positive claim of a chosen beneficiary, frame, or outcome; the document recommends no option of DR-01 (a)-(e), DR-06 (a)-(c), or DR-07 (a)-(g) |
| V3 | INFORMATION NEEDED markers complete | `grep -c "\[INFORMATION NEEDED:" Documentation/Prospectus/06-participant-pathway.md` + inspect each marker | ≥ 20 markers (a 21st hit is the Status-line format description "`[INFORMATION NEEDED: ...]`" - not a marker, no owner field); every marker has the format `[INFORMATION NEEDED: <owner>; <why>; ... <decision blocked>]` with a named role owner and a blocked decision; the §5 table contains exactly rows IN-01…IN-10 and every inline marker maps to one of them |
| V4 | Owner test (every action verb has a named party) | Underline every action verb in the new file | Each action is either (a) performed by a named role (prospective participant, participant, completer, program lead, named org/team/evaluator TBD) or (b) inside an `[INFORMATION NEEDED: <owner>; ...]` marker naming the owner; 0 unattributed action verbs |
| V5 | Deletion test (project name removed) | Delete "FTSArcade"/the project name from a copy of the file | Sections 1-6 remain intelligible: participant-definition carrier, entry-point taxonomy, 5-stage step table, exit points, and decision gate all stand without the project name |
| V6 | Evidence test (causal verbs graded) | `grep -niE "improves|leads to|enables|increases|drives|creates|produces" Documentation/Prospectus/06-participant-pathway.md` | 0 causal-claim hits; any hit that remains is inside a quoted decision-state phrase (e.g. "consequence of delay") and carries an explicit reference; "outcome" appears only in the DR-07 rule context ("engagement metrics are never outcomes") and the step-5 placeholder |
| V7 | Substitution test (city changed → SF facts remain) | Replace "San Francisco"/"SF" with another city in a copy of the file | Every cell that names SF either cites an E1 source (facts-pack #21 rule; platform web-entry fact §(d) fact 3) or carries `[INFORMATION NEEDED: ...]`; 0 city-specific facts stated without a source; the platform web-entry fact (free play, no access gate) remains true under substitution |
| V8 | Tables render | For every table in the new file (Sections 1, 2, 3, 4, 5, 7): header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each; the `\|` escapes inside the §7 revision-record cell render as a literal pipe without breaking the row |
| V9 | Cross-links resolve | `test -f Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/04-delivery-and-budget.md Documentation/Research/facts-pack.md; echo "EXIT:$?"` + extract every `](…)` target from the new file | All four files exist (EXIT:0); every relative link target in the file resolves with `test -f`; 0 dangling links (planned-file cross-links are backticked text, not links) |
| V10 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/06-participant-pathway.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits in the three executed files (the plan file and instructions.md §6's own list are exempt by construction); grep "unique" likewise - 0 hits |
| V11 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | The change touches exactly 1 new file (`Documentation/Prospectus/06-participant-pathway.md`) + exactly 2 modified files (`Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md`); `Documentation/Plan/008-participant-pathway.md` appears as the pre-plan artifact (added/untracked); no other file touched; no deletions |
| V12 | changes.md row | Inspect `Documentation/Logs/changes.md` | One new row: class **Clarifying**, plan ref 008, date 2026-10-14, documents updated listing the new file + `Plan/000-index.md`; appended after the plan-007 row; existing rows unchanged |
| V13 | Index self-consistency | Inspect `Documentation/Plan/000-index.md` | Row 008 present, status `planned`; existing rows 001-007 unchanged |

---

## 6. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| DR-01/DR-06/DR-07 recorded entries (verbatim undecided wording) | `Documentation/Prospectus/03-registers.md` §1.1 | Section 1 and Section 6 carry the states; quote-fidelity rule (stop if drifted, do not patch blind) |
| Role names for owner cells | `Documentation/Prospectus/04-delivery-and-budget.md` §1 (W-03, W-05, W-06, W-08, W-10) | Owner cells must match the delivery map's roles exactly (program lead, named org TBD, named team TBD, named evaluator TBD) |
| Platform fact for the web-entry cell | `Documentation/Research/facts-pack.md` §(d) fact 3 (free play; no login/payment gate) | The only E1-grounded content cell in the framework |
| 25% SF-locality rule | `Documentation/Research/facts-pack.md` fact #21; `03-registers.md` §2 F-08 | Framework-constraint wording in §1/§3 |
| Data-dictionary figures F-01/F-03/F-05/F-11 | `Documentation/Prospectus/03-registers.md` §2 | Figure discipline (§1) and exit-point cells (§4) |
| Marker syntax + change-class definitions | `Documentation/Logs/instructions.md` §5, §9.2 | `[INFORMATION NEEDED: <owner>; why; decision blocked]` format; class Clarifying |
| Current row positions in F3/F4 | `Documentation/Logs/changes.md` (line 16), `Documentation/Plan/000-index.md` (line 15) | Append after the plan-007 rows; re-check at execution |

**Explicitly out of scope for the executor:** choosing or recommending any option of DR-01/DR-06/DR-07 (including naming an indicator, population, or site - any such action violates this plan); inventing any pathway step, owner, or SF location; editing `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `04-delivery-and-budget.md`, root `README.md`, `Documentation/Research/*`, or `Documentation/Refinement/*` (their undecided-state records already exist and are referenced, not duplicated); drafting any email or promotional copy (protocol R1); committing (orchestrator-only, rule R2).