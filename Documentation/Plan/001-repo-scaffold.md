# 001 - Repo Scaffold: Packet Structure, Plan/Log Infrastructure, First Build Roadmap

> **For Hermes:** Execute this plan with subagent-driven-development (one execute agent for the whole scaffold). The orchestrator reviews and commits once per version. This plan only creates the scaffold; it does NOT change any packet document.

**Goal:** Create the repository scaffold - root README index, plan index, and log files encoding the operating protocol - so that every later grant-packet change is planned, delegated, executed, and recorded one version at a time, with the first build from S0 to a draftable D1 packet laid out as an ordered task list.

**Scope - in:** the 6 files in Section 1 only.
**Scope - out:** any change to existing packet documents under `Documentation/Reference|Research|Prospectus|Refinement` (those are future plans, Section 2); email or promotional drafting (prohibited by protocol R1); git commits (orchestrator-only, rule R2).

---

## 0. Repo conventions (established by this plan)

### 0.1 Version label scheme

| Scope | Scheme | Current | Example |
|---|---|---|---|
| Grant packet | S0 → D1 → D2 → … (letter = stage, number = iteration) | S0 (incomplete source packet) | D1 = first draftable packet |
| Plan files | `NNN-<slug>.md`, monotonic 001, 002, … | - | `001-repo-scaffold.md` |
| Commits | `docs(grant): <change>` - one commit per version | - | `docs(grant): scaffold repo with plan and log structure` |

Commit discipline: the executor never commits; the orchestrator makes exactly one commit per executed version, message `docs(grant): <change>`.

### 0.2 Change-class model (per the Reference export's change control; reconcile wording against the export if the executor reads a difference)

| Class | Meaning | Typical trigger | Example |
|---|---|---|---|
| Editorial | Wording, formatting, style only; no fact, number, or decision changes | Typo, tone, table layout | Reflow a table |
| Clarifying | Adds missing information, resolves an unknown, records a decision or evidence grade | `[INFORMATION NEEDED]` resolved; evidence upgraded | New decision-register entry |
| Operational | Changes plans, delivery, budget, or unit-cost numbers | New cost figure, revised schedule | First-year budget update |
| Foundational | Changes scope, beneficiary, charitable frame, eligibility posture, or core claims | Scope-lock decision (DR-01/06/07) | Beneficiary redefined |

Every executed task appends one row to `Documentation/Logs/changes.md` with its class.

### 0.3 Packet state facts (referenced by the scaffold; do not re-derive)

| Fact | Value | Source file |
|---|---|---|
| Packet version label | S0 (incomplete source packet) | `Documentation/Prospectus/README.md` |
| Readiness | Not ready (content) | `Documentation/Prospectus/README.md` |
| Eligibility/registration gate | Blocked | `Documentation/Refinement/00-alignment-matrix.md` |
| Registration closed | Sep 11 2026; only registrants submit | `Documentation/Research/facts-pack.md` |
| Application deadline | Oct 15 2026, 5:00 p.m. PT = Oct 16 2026, 03:00 EEST | `Documentation/Research/facts-pack.md` |
| Competition facts | 41 verified, 6 conflicts flagged (C1-C6) | `Documentation/Research/facts-pack.md` |
| Open decisions | DR-01 … DR-10 + participant pathway + SF delivery capacity (inputs) | `Documentation/Prospectus/03-registers.md` |

---

## 1. Target file tree (this change)

| # | Path | Purpose |
|---|---|---|
| F1 | `README.md` (repo root) | Master index: what the repo is, packet tree, current version label + readiness, deadline banner, next actions. New file (verified absent). |
| F2 | `Documentation/Plan/000-index.md` | Index of all plans with lifecycle status. New. |
| F3 | `Documentation/Plan/001-repo-scaffold.md` | This plan. New. |
| F4 | `Documentation/Logs/instructions.md` | The repo's constitution: operating protocol, writing/style spec, delegation model, commit discipline. New. |
| F5 | `Documentation/Logs/research-log.md` | Research steps: what was researched, what remains to verify. New. |
| F6 | `Documentation/Logs/changes.md` | Revision record: one row per change (methodology revision-record table). New. |

Directories `Documentation/Plan/` and `Documentation/Logs/` are created by this change (verified absent).

### 1.1 F1 - `README.md` (repo root)

**Draws from:** file tree of the packet (below), `Documentation/Prospectus/README.md` (label/readiness), Section 0.3 facts.

Outline (headers verbatim):

```
# FTSArcade - Grant Prospectus Repository

One-paragraph purpose: this repo holds PLANS and prospectus documents for an
SF (San Francisco) grant application ("h.md"). It contains no drafts, no
promotional copy, and no email text - only what we will build, planned,
refined, and recorded over versions.

## ⚠ Deadline & Gate
Blockquote banner, verbatim:
> **Application deadline: Oct 15 2026, 5:00 p.m. PT (= Oct 16 2026, 03:00 EEST).**
> Registration closed Sep 11 2026; only registered entities may submit.
> Current gate status: **Blocked** - see `Documentation/Prospectus/03-registers.md`.

## Packet Status
| Item | Value |
|---|---|
| Version label | S0 (incomplete source packet) |
| Readiness | Not ready (content) |
| Eligibility/registration gate | Blocked |
| Next milestone | D1 - first draftable packet (roadmap: `Documentation/Plan/000-index.md`) |

## Packet Tree
Table: Path | What it is | Status
- Documentation/Reference/ - grant-writing methodology export (2,657-line
  conversation) + PDF - source of the style/validity spec
- Documentation/Research/facts-pack.md - 41 verified competition facts,
  conflicts C1-C6 - verified (6 conflicts)
- Documentation/Research/sources.md - source list - verified
- Documentation/Prospectus/README.md - packet index - S0
- Documentation/Prospectus/00-prospectus.md - master 10-section prospectus - S0
- Documentation/Prospectus/01-source-case.md - source case (SF facts) - S0
- Documentation/Prospectus/02-claim-ledger.md - claim ledger - S0
- Documentation/Prospectus/03-registers.md - decision register DR-01…DR-10 - S0
- Documentation/Prospectus/04-delivery-and-budget.md - delivery & budget - S0
- Documentation/Prospectus/05-durability-risks-rights.md - durability/risks/rights - S0
- Documentation/Refinement/ - alignment matrix, gap report, 21-test checklist - current
- Documentation/Plan/000-index.md - plan index - current
- Documentation/Logs/instructions.md - operating protocol (constitution) - current
- Documentation/Logs/research-log.md - research steps & open verification - current
- Documentation/Logs/changes.md - revision record - current

## Next Actions
1. Resolve the eligibility/registration gate (plan task T01, Section 2 of
   `Documentation/Plan/001-repo-scaffold.md`).
2. Read `Documentation/Logs/instructions.md` before touching any document.
3. Track plans in `Documentation/Plan/000-index.md`.

## For Agents
- Operating protocol: `Documentation/Logs/instructions.md`
- Revision record: `Documentation/Logs/changes.md`
```

Rules: relative links only; no prohibited words (Section 2 of F4); deadline banner verbatim.

### 1.2 F2 - `Documentation/Plan/000-index.md`

**Draws from:** Section 0.1 schemes.

Outline:

```
# Plan Index

Purpose line: every change is first designed as a plan file here, then
executed. Statuses: planned → approved → executed → committed.

## Index
| # | Plan file | Title | Status | Notes |
|---|---|---|---|---|
| 001 | Documentation/Plan/001-repo-scaffold.md | Repo scaffold: structure, plan/log infrastructure, first build roadmap | executed | Flipped to "committed" by the orchestrator in the scaffold's single commit |

## Status Lifecycle
planned - pre-plan agent wrote the plan file
approved - orchestrator accepted the design
executed - execute agent finished, changes.md row appended
committed - orchestrator committed the version
```

### 1.3 F3 - `Documentation/Plan/001-repo-scaffold.md`

This file. Self-referential; no action.

### 1.4 F4 - `Documentation/Logs/instructions.md` (the constitution)

**Draws from:** user's operating protocol (verbatim essence below), `Documentation/Reference/` export (evidence grades, uncertainty language, editing tests, build order, revision-record table - copy wording verbatim from the export where it defines them), `Documentation/Refinement/02-refinement-checklist.md`.

Outline (headers verbatim; each numbered section is 3-8 lines, imperative, enforceable):

```
# Operating Protocol - Instructions for All Agents Working in This Repo

## 1. What this repo is
Plans only. The repo holds PLANS of what we will build - formatted,
presented, and refined neatly OVER VERSIONS, one commit per version.
No email drafting. No promotional content drafting. If a task asks for
either, stop and report the protocol violation.

## 2. The four operating rules
R1  No drafting - see §1. Every artifact is a plan, a register, a log,
    or a refinement of one.
R2  Delegation - the orchestrator does not manage content; it re-orders
    and delegates. Every change to a document is delegated:
    FIRST a pre-plan agent designs the change (writes Plan/NNN),
    THEN an execute agent implements it. One step of separation for
    every change, every time.
R3  Progress is saved after each change in SEPARATE files: planning
    steps, research steps, instructions, and changes - so later
    commits can be distilled easily.
R4  Writing quality - a chosen, consistent style (this spec); validity
    checks applied always (§5-§7).

## 3. Delegation model
pre-plan agent: designs the change, writes Documentation/Plan/NNN-*.md,
never edits packet documents.
execute agent: implements the approved plan exactly, appends the
changes.md row, never commits.
orchestrator: re-orders and delegates, reviews, commits exactly one
commit per version (`docs(grant): <change>`). Agents never commit, never
push.

## 4. Commit discipline
One commit per version. Message: `docs(grant): <change>`. The commit is
made by the orchestrator only, after the execute agent's handoff.

## 5. Evidence & uncertainty language
- Evidence grades E1-E5 on every material claim (definitions copied
  verbatim from the Reference export, §writing methodology).
- Partner statuses: confirmed / in discussion / proposed - never a bare
  partner name without a status.
- Unknowns: `[INFORMATION NEEDED: <owner>; why; decision blocked]` -
  never silently resolved.
- Uncertainty phrases (use verbatim):
  - "As of [date], [source] shows…"
  - "Comparable evidence suggests…"
  - "The project will test whether…"
  - "The planning target is…"

## 6. Prohibited words & phrases
revolutionary, world-class, unique, cutting-edge;
empower / unlock / transform - only with a defined change;
scalable - only with a unit cost;
sustainable - only with a named payer;
"partners include" - when the list is incomplete;
"data shows" - when the statement is an assumption.

## 7. Editing tests (validity) - apply to every document
1. Deletion - project name removed → intervention still stands
2. Substitution - city changed → SF facts still hold
3. Owner - every action verb has a named party
4. Evidence - every causal verb has an evidence grade
5. Budget - every promised output has a cost
6. Durability - grant ends → named survivors
7. Proportionality - halved request → stated losses
8. Adversarial - weakest assumption acknowledged in writing

## 8. Build order for the grant packet
participant pathway → platform boundary → claim ledger (15-25 claims) →
first-year operating plan → unit-cost model → narrative LAST.

## 9. Version labels & change classes
Copy the two tables from Documentation/Plan/001-repo-scaffold.md §0.1-§0.2.
Every change is labeled with its class (Editorial / Clarifying /
Operational / Foundational) and recorded in changes.md.

## 10. File map
Documentation/Reference/   - methodology export (the source of this spec)
Documentation/Research/    - verified facts, sources, conflicts
Documentation/Prospectus/  - the packet itself (00-05; 06+ planned)
Documentation/Refinement/  - alignment matrix, gap report, editing checklist
Documentation/Plan/        - plan files (this repo's change designs)
Documentation/Logs/        - instructions, research log, changes
```

### 1.5 F5 - `Documentation/Logs/research-log.md`

**Draws from:** `Documentation/Research/facts-pack.md` (41 facts, conflicts C1-C6), `Documentation/Research/sources.md`. Do NOT duplicate facts - link.

Outline:

```
# Research Log

Purpose: what was researched, when, with what outcome and verification
state. Facts live in Documentation/Research/; this log records steps.

## Log
| Date | Step | What was researched | Source(s) | Outcome | Status | Evidence grade |
(Seed rows, from the completed fan-out; date = the packet files' creation
date, taken from git: `git log --diff-filter=A --format=%ad -- Documentation/Research/facts-pack.md`.)
- facts-pack.md: 41 competition facts, each with source URL + status;
  6 conflicts flagged (C1-C6) - status: verified (6 conflicts)
- sources.md: source list compiled - status: verified
- Full Application PDF link returned 404 - status: unverified
- SF Travel / Recreation & Parks archives - status: unverified
- Bulgarian-entity registration status - status: unverified

## Open verification items (do not resolve silently)
| Item | [INFORMATION NEEDED: owner; why; decision blocked] | Unblocks |
- Full Application PDF (official form contents) -
  owner: research; why: link 404s; decision blocked: submission form
  fields unknown → blocks: gate
- SF Travel / Rec & Park archives - owner: research; why: SF facts
  provenance; decision blocked: substitution test for SF claims →
  blocks: source case
- Bulgarian-entity registration - owner: FTSArcade principal; why: only
  registrants submit; decision blocked: eligibility gate → blocks: gate
```

### 1.6 F6 - `Documentation/Logs/changes.md`

**Draws from:** methodology's revision-record table (Reference export). One row per change, appended by the execute agent of each version.

Outline:

```
# Changes - Revision Record

Purpose: one row per change; the distillation source for later commits.

## Record
| Date | Change class | What changed | Why | Evidence/budget affected | Decision | Documents updated | Plan ref |
(Seed rows - date = commit date of each version.)
1. Foundational | Initial packet build (source packet S0) | research + prospectus fan-out | - | - | Reference/, Research/, Prospectus/ (00-05), Refinement/ | (fan-out, no plan file) |
2. Foundational | Repo scaffold | encode operating protocol; add index/logs | - | - | README.md, Plan/000, Plan/001, Logs/* | 001 |
```

---

## 2. First build plan: S0 → D1 (the "what we'll build" content)

This section is the roadmap for the packet itself. Each task is a change and is therefore executed ONLY after this plan is approved (delegation rule R2); tasks needing deeper design produce their own plan files 002+ before execution. Buckets: **GATE** = before Oct 15 2026, 03:00 EEST (deadline); **SCOPE-LOCK** = immediately after the gate, date-agnostic; **CONTENT** = Aug 2027 prospectus cycle unless the gate resolves otherwise (plan does not assume the outcome); **VERIFY** = after content.

Every task's verification includes: append a changes.md row (class + documents updated) and re-run §7 editing tests named in the task.

| # | Task | Bucket | Output file | Inputs |
|---|---|---|---|---|
| T01 | Record eligibility/registration gate decision | GATE | `Documentation/Prospectus/03-registers.md` (+ readiness fields in `00-prospectus.md`, root README banner if the decision changes them) | 03-registers.md, facts-pack.md, 00-alignment-matrix.md |
| T02 | Lock DR-01 (beneficiary) | SCOPE-LOCK | `Documentation/Prospectus/03-registers.md` (+ `01-source-case.md`, `00-prospectus.md` where the decision bites) | 03-registers.md, 01-source-case.md, 00-alignment-matrix.md |
| T03 | Lock DR-06 (charitable frame) | SCOPE-LOCK | same as T02 | same as T02 |
| T04 | Lock DR-07 (single public outcome) | SCOPE-LOCK | same as T02 | same as T02 |
| T05 | Participant pathway | CONTENT | `Documentation/Prospectus/06-participant-pathway.md` (new) | T02-T04 records, 01-source-case.md, facts-pack.md, 04-delivery-and-budget.md |
| T06 | Platform boundary | CONTENT | `Documentation/Prospectus/07-platform-boundary.md` (new) | T05, 01-source-case.md, facts-pack.md |
| T07 | Claim ledger build-out (15-25 claims) | CONTENT | `Documentation/Prospectus/02-claim-ledger.md` (extend) | facts-pack.md, sources.md, 06, 07 |
| T08 | First-year operating plan | CONTENT | `Documentation/Prospectus/08-first-year-operating-plan.md` (new; cross-link 04) | 02, 04-delivery-and-budget.md, 06, 07 |
| T09 | Unit-cost model + funding scenario | CONTENT | `Documentation/Prospectus/09-unit-cost-model.md` (new) | 08, 04-delivery-and-budget.md |
| T10 | Narrative (LAST) | CONTENT | `Documentation/Prospectus/10-narrative.md` (new) | 01, 02, 05, 06, 07, 08, 09 |
| T11 | Editing-test verification pass | VERIFY | `Documentation/Refinement/02-refinement-checklist.md` (update) | all packet files |
| T12 | Readiness relabel S0 → D1 + index sync | VERIFY | `Documentation/Prospectus/README.md`, root `README.md`, `Documentation/Plan/000-index.md` | all |

### Task detail

**T01 - Gate decision (GATE).** Objective: record the eligibility/registration decision as a decision-register entry - explicitly NOT an email draft (protocol R1; grep the change for `dear|subject:|sincerely` → 0 hits). Steps: read 03-registers.md for the next free DR number and entry format → append entry (decision: registered / not registered / unknown; deciding owner named; date; evidence grade; gate effect Open/Blocked/Closed; named next action). Verification: owner test (entry names who decided and who knows the registrant status); uncertainty language "As of [date], [source] shows…" where the status is unknown; deletion test passes; gate fields updated consistently in 00-prospectus.md and root README banner.

**T02/T03/T04 - Scope locks (SCOPE-LOCK).** Objective: each records its decision (DR-01 beneficiary, DR-06 charitable frame, DR-07 single public outcome) in 03-registers.md with date, owner, evidence grade, and applies the decision to 01-source-case.md / 00-prospectus.md where it bites (class: Clarifying, or Foundational if it changes scope). Verification: owner test; adversarial test (weakest assumption of the chosen frame acknowledged in writing); affected files updated and cross-linked; changes.md row per task.

**T05 - Participant pathway (CONTENT).** Objective: define who participates, entry points, and the step-by-step pathway with a named owner per step and SF grounding. Outline: (1) participant definition (from DR-01), (2) entry points, (3) pathway table `step | who | action | owner | SF source | evidence grade`, (4) exit/drop-off points, (5) unknowns as `[INFORMATION NEEDED]`. Verification: owner test (every action verb has a named party); deletion test (project name removed → pathway still stands); evidence test (causal verbs graded); substitution test (city changed → SF facts remain).

**T06 - Platform boundary (CONTENT).** Objective: define the platform's boundary - inside vs outside, who provides what, where it ends. Outline: (1) platform definition and function scope, (2) boundary table `inside platform | outside platform | provider of outside items`, (3) SF-ecosystem dependencies with source links, (4) boundary unknowns. Verification: substitution test; owner test; no "scalable" without a unit cost.

**T07 - Claim ledger 15-25 (CONTENT).** Objective: build the ledger to 15-25 claims. Outline: table `claim # | claim | evidence grade | source URL | status | conflict ref (C1-C6 if any)`. Verification: row count in [15, 25] (count programmatically: `grep -c '^|' Documentation/Prospectus/02-claim-ledger.md` adjusted for header rows - executor records the count in the changes.md row); every claim has grade + source; conflicts cross-referenced; no ungraded causal verbs.

**T08 - First-year operating plan (CONTENT).** Objective: year-1 outputs, owners, costs, and named survivors. Outline: (1) year-1 objectives mapped to claims, (2) quarter table `Q | outputs | owner | cost line`, (3) staffing & partners with statuses (confirmed/in discussion/proposed), (4) durability/survivor plan, (5) risks. Verification: budget test (every promised output has a cost); durability test (grant ends → named survivors); owner test.

**T09 - Unit-cost model + funding scenario (CONTENT).** Objective: unit costs per output and funding-scenario losses. Outline: (1) unit definition and unit cost per output, (2) cost drivers, (3) funding scenarios table `request level | covered | lost` , (4) assumptions with grades. Verification: proportionality test (halved request → stated losses); every "scalable" claim has a unit cost; numbers trace to budget lines in 04.

**T10 - Narrative (CONTENT, LAST).** Objective: the narrative prose, written only after all evidence artifacts exist. Outline: problem (from 01) → intervention (06/07) → evidence (02) → plan (08) → budget (09) → durability (05). Verification: deletion + substitution tests; prohibited-words scan → 0 hits (Section 6 of instructions.md); uncertainty phrases used wherever evidence is below E3.

**T11 - Editing-test verification pass (VERIFY).** Objective: run all 8 editing tests plus the 21 checklist tests across the packet; record pass/fail per test. Verification: every test row has a verdict and an evidence reference; failing tests are reported to the orchestrator as follow-up tasks (never silently fixed); changes.md row lists fails.

**T12 - Readiness relabel S0 → D1 + index sync (VERIFY).** Objective: relabel the packet D1 and sync all indices. Verification: label D1 appears consistently in root README, Prospectus/README.md, 00-prospectus.md; all relative links in the three index files resolve (Section 3.2); plan index rows updated (T01-T12 statuses: executed/committed).

---

## 3. Verification - how the executor proves the scaffold is correct

Run in order; every check must pass before handoff.

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | Files exist | `for f in README.md Documentation/Plan/000-index.md Documentation/Plan/001-repo-scaffold.md Documentation/Logs/instructions.md Documentation/Logs/research-log.md Documentation/Logs/changes.md; do test -f "$f" || echo "MISSING $f"; done; echo "EXIT:$?"` | No MISSING lines; EXIT:0 |
| V2 | Links resolve | Extract every relative `](…)` target from README.md, Plan/000-index.md; `test -f` each | 0 dangling links |
| V3 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' README.md Documentation/Plan Documentation/Logs` | 0 hits outside instructions.md §6's own list (inspect that file for the list block only; grep "unique" likewise - allowed only inside the list) |
| V4 | Tables render | For every markdown table in the 6 files: header row, separator row, and body rows have equal pipe counts (check each file) | Equal pipe counts per table; separator row present in each |
| V5 | No collateral edits | `git status --porcelain` before and after; diff the file lists | Exactly the 6 new files added; no existing packet file modified; no deletions |
| V6 | Index self-consistency | Inspect Plan/000-index.md | Row 001 present, status `executed` (orchestrator flips to `committed` in the single commit) |
| V7 | Constitution completeness | Inspect instructions.md against §1.4 outline | All 10 numbered sections present with headers verbatim |
| V8 | One commit per version | Orchestrator, after handoff: `git add` the 6 files; `git commit -m "docs(grant): scaffold repo with plan and log structure"` | Exactly one commit; tree clean afterwards |

---

## 4. Executor inputs (not derivable from this plan - read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| E1-E5 evidence-grade definitions | Reference export, writing-methodology section - copy verbatim into instructions.md §5 | Definitions live in the export, not here |
| Change-class wording | Reference export change-control section - reconcile §0.2 if wording differs | Canonical source |
| Next free DR number | `Documentation/Prospectus/03-registers.md` | T01-T04 append entries |
| Seed-row dates for research-log.md / changes.md | `git log --diff-filter=A --format=%ad -- <file>` | Actual creation dates |
| Root README absence | `test -f README.md` | F1 is a new file (verified absent at plan time; re-check at execution) |