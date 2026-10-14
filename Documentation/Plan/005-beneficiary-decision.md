# 005 - Beneficiary Scope Lock: Record DR-01 Decision State and Options (T02)

> **For Hermes:** Execute this plan with an execute agent. Orchestrator reviews and commits once (`docs(grant): <change>`). This change records the DR-01 (beneficiary) decision **state** - undecided as of 2026-10-14 - and the candidate options, **without choosing a beneficiary** (none is defined anywhere in the packet; inventing one is forbidden).

**Goal:** Satisfy plan 001 task T02 (bucket SCOPE-LOCK): record the DR-01 beneficiary decision honestly in `Documentation/Prospectus/03-registers.md` §1.1 (decision state, options table, decision rule, needed evidence, owner, deadline, consequence), and apply the record where the decision bites in `01-source-case.md` (beneficiary row, ten-statement #2, revision record) and `00-prospectus.md` (Decision summary beneficiary line, Need section, §3.1 candidate directions, §11 blocking-unknowns row), plus the `changes.md` row and `000-index.md` row.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and T02 task detail): no scope change occurs - no beneficiary is defined or redefined; the change adds missing information (the decision state) and records a decision-register entry, exactly mirroring change 004 (DR-11, "Unknown as of 2026-10-14", class Clarifying). Foundational would apply only if the decision were made and changed scope; it is not.

**Scope - in:** the 6 files listed in Section 1 (1 new plan file exists already; 5 documents edited).
**Scope - out:** choosing a beneficiary; any edit to `00-alignment-matrix.md`, `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/005-beneficiary-decision.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/03-registers.md` | Modify: DR-01 live row; §1.1 intro sentence; append DR-01 §1.1 entry + options-detail block |
| F3 | `Documentation/Prospectus/01-source-case.md` | Modify: row 1 (Beneficiary) status; ten-statement #2; append revision-record row |
| F4 | `Documentation/Prospectus/00-prospectus.md` | Modify: §1 Beneficiary line; §2 "What is missing" bullet 1; §3.1 candidate-directions line; §11 row 3 |
| F5 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 005) |
| F6 | `Documentation/Plan/000-index.md` | Modify: append row 005, status `planned` |

---

## 2. F2 - `Documentation/Prospectus/03-registers.md`

### 2.1 Replace the live DR-01 row (Section 1 table, currently line 12)

**Current text (quote):**
```
| DR-01 | **Beneficiary** | (a) Creative workforce pathways (16-24 etc., TBD); (b) Accessible community learning; (c) Community connection; (d) Public cultural-installation program; (e) none approved | Greatest demonstrated need + reachable population; must fit the ≤25%-outside-SF rule | Local SF evidence, delivery access, population estimate + source | Program lead | Before scope lock (not achieved) | All downstream work pauses; packet stays Not ready |
```

**Replacement:**
```
| DR-01 | **Beneficiary** | (a) Creative workforce pathways (structured game-development training, paid projects, employment support); (b) Accessible community learning (facilitated digital-literacy / creative-technology programs); (c) Community connection (recurring facilitated neighborhood activities); (d) Public cultural-installation program (free public installations; linked to DR-06); (e) none approved - **all recorded, not chosen** (see §1.1) | One primary purpose; defined population with inclusion/exclusion rules and geography; greatest demonstrated need + reachable-population estimate (F-11) as planning target; must fit the ≤25%-outside-SF rule | Local SF evidence (city-source problem analysis), delivery access, population estimate + source | Program lead | Before scope lock (not achieved) | All downstream work pauses; packet stays Not ready |
```

The Options cell drops the "16-24 etc., TBD" placeholder (an invented age band, never sourced) and appends the export's role descriptions; the Decision rule cell adds the one-primary-purpose and defined-population (inclusion/exclusion/geography) requirements and the F-11 planning-target cross-reference.

### 2.2 §1.1 intro sentence (currently line 25)

**Current text (quote):** `Entries are appended as decisions are made. An entry records the decided value, the deciding owner, the date, the evidence grade, the gate effect, and the named next action. Open rows (DR-01…DR-10) remain the live register; recorded entries are the audit trail.`

**Replacement:** `Entries are appended as decisions are made or decision states are recorded. An entry records the decided value or state, the deciding owner, the date, the evidence grade, the gate effect, and the named next action. Open rows (DR-01…DR-10) remain the live register; recorded entries are the audit trail.`

(Keeps §1.1 semantics honest for an undecided-state record, per the DR-11 precedent.)

### 2.3 Append the DR-01 recorded entry to the §1.1 table (after the DR-11 row, currently line 29)

**New row (DR-11 column format, quote to insert):**
```
| DR-01 | Beneficiary | **Undecided as of 2026-10-14** - as of 2026-10-14, no packet document defines a beneficiary population: no population, inclusion/exclusion rules, geography, or estimated reachable population exists anywhere (`01-source-case.md` row 1, `00-prospectus.md` §2, data dictionary F-11 all carry `[INFORMATION NEEDED: program lead; ...]`). The candidate options below are recorded from the export (`Documentation/Reference/we're looking to prepare a grant application for h.md`, §1 "Choose one primary purpose") and from the DR-01 register row; they are **options, not chosen**: (a) creative workforce pathways - participants in structured game-development training, paid projects, and employment support; (b) accessible community learning - participants in facilitated digital-literacy and creative-technology programs; (c) community connection - participants in recurring, facilitated activities through neighborhood organizations; (d) public cultural-installation program - users of free public cultural/recreational installations (admissible-frame hypothesis, DR-06); (e) none approved. No positive claim is made about who benefits; the status is recorded as undecided. | Program lead `[INFORMATION NEEDED: named person; required to own the SF problem analysis and the reachable-population estimate and to choose the beneficiary; blocks Need, Solution, Measurement, Budget - DR-01]` | 2026-10-14 | E1 (option list sourced from the export and the existing register row, verified 2026-10-14; the undecided status itself is ungraded - no positive claim, mirroring DR-11) | **Open** (scope not locked; downstream work paused) | Program lead: (1) produce the SF problem analysis from city sources (per `00-alignment-matrix.md` criterion 1: SF Arts Commission, Cultural Districts, OEWD, Rec & Park - as evidence sources, not partners) and a reachable-population estimate with source and method (data dictionary F-11); (2) choose ONE option by the decision rule in §2.1 (one primary purpose; defined population with inclusion/exclusion and geography; greatest demonstrated need + reachable population as planning target; fits the ≤25%-outside-SF rule) before scope lock; (3) record the chosen value as a new DR-01 entry or addendum, including the adversarial test of its weakest assumption. |
```

### 2.4 Append the DR-01 options-detail block immediately after the §1.1 table, before the `---` separator preceding Section 2

**Insert (quote):**
```
**DR-01 option detail (recorded 2026-10-14, not chosen).** Sources: export `Documentation/Reference/we're looking to prepare a grant application for h.md` §1 (options a-c: proposed role + evidence columns verbatim); option (d) from the DR-01 register row (links to DR-06); option (e) is the base case. Weakest-assumption column is the adversarial test (instructions.md §7.8) applied per option.

| Option | Proposed role for FTSArcade | Evidence you would need (export) | Weakest assumption (adversarial test) |
|---|---|---|---|
| (a) Creative workforce pathways | Entry point into structured game-development training, paid projects, and employment support | Participant learning, completed portfolios, paid placements, employer demand | Employer demand and training/employment-support capacity exist and the team can deliver them - no employer, trainer, or placement partner is named (E4, untested) |
| (b) Accessible community learning | Platform for facilitated digital-literacy and creative-technology programs | Demonstrated learning gains, accessibility testing, partner delivery capacity | The team can deliver facilitated learning with measurable gains - no accessibility audit, no partner delivery capacity, no learning-gain evidence exists (E4, untested) |
| (c) Community connection | Tool for recurring, facilitated activities through neighborhood organizations | Repeat participation, validated belonging measures, evidence beyond website traffic | Neighborhood organizations will host and sustain recurring activities - no neighborhood organization is confirmed; repeat participation is unmeasured (E4, untested) |
| (d) Public cultural-installation program | Free public cultural/recreational installations documenting SF places (admissible-frame hypothesis) | Site plan, access rules, business-selection rules, engagement measures (DR-06) | Commerce can fund free public access while private benefit stays incidental - no site plan, access rules, or advertising controls exist (E4, untested) |
| (e) None approved | No beneficiary defined | - | No defined beneficiary leaves rubric criteria 1-2 unscorable (score 1-2) and the packet Not ready - the recorded base case, not a plan |

**Decision rule:** one primary purpose; defined population with inclusion/exclusion rules and geography; greatest demonstrated need (city-source SF problem analysis) + reachable-population estimate (F-11) as planning target; must fit the ≤25%-outside-SF rule (rules page, E1).
**Needed evidence:** local SF evidence (problem analysis from city sources), delivery access, population estimate with source and method.
**Owner:** program lead (named person `[INFORMATION NEEDED]`).
**Deadline:** before scope lock (not achieved).
**Consequence of delay:** all downstream work pauses; packet stays Not ready.
```

---

## 3. F3 - `Documentation/Prospectus/01-source-case.md`

### 3.1 Replace row 1 (Beneficiary) status cell (currently line 9)

**Current text (quote):** `**NOT DEFINED.** No population, inclusion/exclusion rules, geography, or estimated reachable population. `[INFORMATION NEEDED: program lead; required to define who benefits and what changes; blocks Need, Solution, Measurement, Budget - DR-01]``

**Replacement:** `**NOT DEFINED.** Decision state recorded 2026-10-14 (`03-registers.md` §1.1, DR-01): **undecided** - no population is defined anywhere; candidate options (a) creative workforce pathways, (b) accessible community learning, (c) community connection, (d) public cultural-installation program, (e) none approved are recorded, **not chosen**. No inclusion/exclusion rules, geography, or estimated reachable population. `[INFORMATION NEEDED: program lead; required to define who benefits and what changes; blocks Need, Solution, Measurement, Budget - DR-01]``

### 3.2 Ten-statement #2 (currently line 25)

**Current text (quote):** `2. "The project serves [included population] in [San Francisco geography], excluding [groups]." → **UNKNOWN** `[DR-01]``

**Replacement:** `2. "The project serves [included population] in [San Francisco geography], excluding [groups]." → **UNKNOWN** - decision state recorded 2026-10-14 (undecided) `[DR-01]``

### 3.3 Append one row to the Revision record table (after line 43)

**New row (quote):**
```
| 2026-10-14 | DR-01 beneficiary decision state recorded (undecided; options listed, not chosen) | Clarifying | Plan 001 T02 requires the scope-lock record; no population is defined, so the state - not a beneficiary - is recorded | Export option list (E1, source); no new figures; F-11 estimate still INFORMATION NEEDED | Undecided as of 2026-10-14; owner program lead; deadline before scope lock | 03-registers.md, 01-source-case.md, 00-prospectus.md |
```

---

## 4. F4 - `Documentation/Prospectus/00-prospectus.md`

### 4.1 §1 Decision summary - Beneficiary line (currently line 16)

**Current text (quote):** `**Beneficiary:** Not yet defined. `[INFORMATION NEEDED: program lead; required to define who benefits and what changes; blocks the entire proposal - DR-01]``

**Replacement:** `**Beneficiary:** Not yet defined. Decision state recorded 2026-10-14 (`03-registers.md` §1.1, DR-01): **undecided** - candidate options recorded, none chosen. `[INFORMATION NEEDED: program lead; required to define who benefits and what changes; blocks the entire proposal - DR-01]``

### 4.2 §2 Need - "What is missing" bullet 1 (currently line 48)

**Current text (quote):** `- Beneficiary definition with inclusion/exclusion rules, geography, and estimated reachable population → `[DR-01]``

**Replacement:** `- Beneficiary definition with inclusion/exclusion rules, geography, and estimated reachable population → `[DR-01]` (decision state recorded 2026-10-14 as undecided - `03-registers.md` §1.1; no population is defined anywhere in the packet)`

### 4.3 §3.1 candidate-directions line (currently line 67)

**Current text (quote):** `Candidate directions from the export (options, **not chosen**): creative workforce pathways; accessible community learning; community connection. Each would give FTSArcade a different function (entry point into structured game-development training; platform for facilitated digital-literacy programs; tool for recurring facilitated neighborhood activities). Choosing one is `[DR-01]`.`

**Replacement:** `Candidate directions from the export (options, **not chosen**, recorded 2026-10-14 in `03-registers.md` §1.1 with roles, evidence needs, and weakest assumptions): creative workforce pathways; accessible community learning; community connection; public cultural-installation program (DR-06 frame hypothesis); none approved. Each would give FTSArcade a different function (entry point into structured game-development training; platform for facilitated digital-literacy programs; tool for recurring facilitated neighborhood activities). Choosing one is `[DR-01]`.`

### 4.4 §11 Blocking unknowns - row 3 (currently line 236)

**Current text (quote):** `| 3 | Beneficiary definition | Need, Solution, all downstream | Program lead | DR-01 |`

**Replacement:** `| 3 | Beneficiary definition | Need, Solution, all downstream | Program lead | DR-01 (undecided as of 2026-10-14 - recorded `03-registers.md` §1.1) |`

---

## 5. F5 - `Documentation/Logs/changes.md`

**Append one row after the plan-004 row (currently line 13), same column format:**

```
| 2026-10-14 | Clarifying | Record DR-01 beneficiary decision state (undecided as of 2026-10-14): candidate options (a)-(e) from the export recorded, not chosen; decision rule, needed evidence, owner (program lead), deadline (before scope lock), consequence (downstream pauses) | Plan 001 T02 (SCOPE-LOCK) requires the beneficiary record; no population is defined anywhere, so the record states the undecided state - no beneficiary invented | Export option list (E1, source); status itself ungraded (undecided); no budget affected | Recorded: undecided as of 2026-10-14; deciding owner = program lead; gate effect Open (scope not locked) | Prospectus/03-registers.md, Prospectus/01-source-case.md, Prospectus/00-prospectus.md, Plan/000-index.md | 005 |
```

---

## 6. F6 - `Documentation/Plan/000-index.md`

**Append one row after the plan-004 row (currently line 12):**

```
| 005 | `Documentation/Plan/005-beneficiary-decision.md` | Beneficiary scope lock: record DR-01 decision state and options (plan 001 T02) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 7. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T02: owner test; adversarial test (weakest assumption acknowledged); affected files updated and cross-linked; changes.md row. Per instructions.md §11.6, the orchestrator also starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T02; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No invented beneficiary | Read the four changed document cells (03-registers §1.1 entry + option table, source-case row 1, prospectus §1/§2) | 0 positive claims of a chosen population, reachable-population figure, or age band; the only population wording is inside the recorded option descriptions (a)-(d); "undecided"/"recorded, not chosen"/"options" language present in all four locations |
| V2 | Uncertainty language | `grep -n "Undecided as of 2026-10-14" Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md` | ≥1 hit in 03-registers.md §1.1; the status carries no evidence grade of its own (graded only as "ungraded - no positive claim", mirroring DR-11); phrase "as of 2026-10-14" present |
| V3 | Owner test | Inspect the §1.1 DR-01 entry | Deciding owner named = Program lead (role); named-person `[INFORMATION NEEDED: ...]` marker preserved; every next-action verb has the program lead as party |
| V4 | Adversarial test | Inspect the §1.1 options-detail table | Every option (a)-(e) has a weakest-assumption cell acknowledging the untested assumption (E4) |
| V5 | Cross-links | `test -f Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md Documentation/Logs/changes.md Documentation/Plan/000-index.md; echo "EXIT:$?"` + inspect `[DR-01]`/`[INFORMATION NEEDED]` references | All files exist (EXIT:0); §1.1 entry ↔ source-case row 1 ↔ prospectus §1/§2/§3.1/§11 references resolve; F-11 referenced in the decision rule; no dangling relative link |
| V6 | Tables render | For each edited table (03-registers §1 table, §1.1 table, §1.1 option table; changes.md; 000-index): header row, separator row, body rows have equal pipe counts | Equal pipe counts per table; separator row present in each |
| V7 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md Documentation/Logs/changes.md Documentation/Plan/000-index.md Documentation/Plan/005-beneficiary-decision.md` | 0 hits (this plan file included) |
| V8 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | Exactly 1 added file (`Documentation/Plan/005-beneficiary-decision.md` - written by the pre-plan agent) + exactly 5 modified files (F2-F6); no other file touched, no deletions |
| V9 | changes.md row | Inspect changes.md | One new row with class **Clarifying**, plan ref 005, date 2026-10-14, documents updated listing F2-F4 + F6 |
| V10 | Index self-consistency | Inspect 000-index.md | Row 005 present, status `planned`; existing rows 001-004 unchanged |

---

## 8. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| Exact current rows to replace | F2-F4 as quoted in Sections 2-4 (re-read at execution; if any quoted text drifted, stop and report - do not patch blind) | Precision requirement; quote fidelity |
| Export option table + framework | `Documentation/Reference/we're looking to prepare a grant application for h.md` §1 (lines ~60-77) and §"Decision register" methodology table (~line 1545) | Canonical source of options, roles, evidence needs, and the drafting-framework requirement (defined population with inclusion/exclusion + geography + reachable-population estimate) |
| §1.1 entry format | 03-registers.md DR-11 row | Column format and "unknown/undecided state" precedent |
| Change-class definition | `Documentation/Logs/instructions.md` §9.2; plan 001 §0.2 | Class Clarifying (no scope change) |

**Explicitly out of scope for the executor:** choosing or recommending a beneficiary (any such action violates this plan); editing `00-alignment-matrix.md` (its criterion-1 row already states the decision needed); editing root `README.md` (no status field changes - gate stays Blocked per DR-11, packet stays Not ready); drafting any email or promotional copy (protocol R1).