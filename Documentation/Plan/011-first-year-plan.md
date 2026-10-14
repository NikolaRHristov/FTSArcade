# 011 - First-Year Operating Plan: Year-1 Objectives, Quarter Plan, Staffing, Survivors (T08)

> **For Hermes:** Execute this plan with one execute agent. The executor writes `Documentation/Prospectus/08-first-year-operating-plan.md` as a **structured operating-plan framework - not a draft plan** - because DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided as of 2026-10-14** (`03-registers.md` §1.1) and DR-04 (funding scenario) is unselected. The executor edits exactly three files (F2-F4), never commits, and reports the verified marker count. The orchestrator reviews, commits once (`docs(grant): first-year operating plan framework (T08)`), and flips the 000-index row through the lifecycle.

**Goal:** Satisfy plan 001 task T08 (bucket CONTENT) by creating `Documentation/Prospectus/08-first-year-operating-plan.md` - a STRUCTURED FIRST-YEAR OPERATING PLAN FRAMEWORK: (1) year-1 objectives mapped to claims; (2) quarter table `Q | outputs | owner | cost line`; (3) staffing and partners with statuses; (4) durability/survivor plan; (5) risks with decision triggers; (6) decision-gate note - and appending the changes.md row and the 000-index.md row. No output, owner, cost figure, or partner is invented: E1 claims (C01-C05, C27) carry the only concrete objectives and the only named survivors (retained assets); every other cell is `[INFORMATION NEEDED: ...]`; every cost line is a named line category from `04-delivery-and-budget.md` §2.2 with a `[INFORMATION NEEDED: budget owner; cost source - DR-04]` marker or an explicit zero-cost explanation; zero dollar figures.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and the T08 task detail): no scope change occurs - no option of DR-01/DR-06/DR-07 is chosen or redefined; the change adds missing information (the operating-plan framework and the propagated decision states) and creates one new packet document. This mirrors the Clarifying precedent of changes 004-010 (recorded undecided decision states; pathway, boundary, and claim-ledger frameworks). Foundational would apply only if the decisions were made and changed scope; they are not. Operational would apply to delivery/budget numbers; the document adds none (zero dollar figures).

**Scope - in:** the 3 files listed in Section 1 (F2-F4) plus this plan file (F1, already written by the pre-plan agent).
**Scope - out:** choosing or recommending any option of DR-01/DR-06/DR-07 (including naming an indicator, population, site, partner, or provider); inventing outputs, owners, cost figures, or partners; edits to `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `02-claim-ledger.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, root `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/011-first-year-plan.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/08-first-year-operating-plan.md` | **New file** (verified absent): the first-year operating plan framework - write the Section 2.2 content verbatim |
| F3 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 011) after the plan-010 row (currently line 18) |
| F4 | `Documentation/Plan/000-index.md` | Modify: append row 011, status `planned`, after the plan-010 row (currently line 18) |

---

## 2. F2 - `Documentation/Prospectus/08-first-year-operating-plan.md` (NEW FILE)

### 2.1 File-level rules (binding)

- Write the file exactly as the fenced content in §2.2: headers verbatim, tables verbatim, cell text verbatim, relative links only. Do not add, remove, or reword any section, row, cell, or marker.
- All owners are **roles** (per `03-registers.md` rules: "All owners are roles; named persons are `[INFORMATION NEEDED: ...]`"). No person's name, no organization name beyond the delivery-map role labels ("technical owner", "program lead", "budget owner", "evidence reviewer", "authorized officer", "executive owner", "rights owner", "counsel", "decision owner", "named org (TBD - W-05)", "named team (TBD - W-06)", "named evaluator (TBD - W-10)") and the two recorded fiscal-sponsor candidates (Community Initiatives, Intersection for the Arts - proposed only), and no SF location may be invented.
- Year-1 boundary (binding, from `04-delivery-and-budget.md` §3.1): year-1 = **named capacity only**; must not include scale dependent on unsigned partners; no automatic post-grant continuation (§3.3: retained assets, adopted activities, funded operations - only retained assets can be named today).
- Zero dollar figures: the string `$` must not appear in the file (V1). The only cost rule quoted is the indirect-cost cap (≤29% of direct project/activity costs, E1, rules §7), named as a line rule, not an amount.
- No causal claims: the only causal wording is inside quoted decision-state references and claim refs; no gameplay-to-outcome statement.
- No prohibited words (instructions.md §6): revolutionary, world-class, unique, cutting-edge, empower, unlock, transform, scalable, sustainable, "partners include", "data shows" - 0 hits. In particular, "sustainable" never appears (the survivor plan says "post-grant").
- Quote fidelity: before writing, re-read `Documentation/Prospectus/03-registers.md` §1.1 (DR-01/DR-06/DR-07 undecided wording) and §1 rows (DR-04/DR-08/DR-09/DR-10), `04-delivery-and-budget.md` §1 (role labels), §2.2 (line category names), §3 (first-year boundary), and `05-durability-risks-rights.md` §2 (risk register). If the recorded wording drifted from what §2.2 quotes, **stop and report - do not paraphrase or patch blind** (mirrors plans 008/009's quote-fidelity rule).
- Cross-links to planned files (`09-unit-cost-model.md`, `10-narrative.md`) are plain backticked text, NOT markdown links - they do not exist yet, and dangling links fail V9.

### 2.2 Complete file content (write exactly this)

```
# First-Year Operating Plan - FTSArcade / Boundless San Francisco

**Version:** S0 (framework only) · **Date:** 2026-10-14
**Status:** **FRAMEWORK ONLY - NOT DRAFTABLE.** As of 2026-10-14, DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided** (`03-registers.md` §1.1) and DR-04 (funding scenario) is unselected; no beneficiary, intervention, cost source, or partner is defined anywhere. The year-1 boundary is **named capacity only** (`04-delivery-and-budget.md` §3.1: "capacity that named people and partners can deliver"; expansion beyond unsigned capacity is out of scope). Every year-1 objective, quarter output, staffing row, and survivor row below is either grounded in an E1 claim or carries `[INFORMATION NEEDED: ...]`; **no output, owner, cost figure, or partner is invented.** The first-year plan becomes draftable only when the three scope-lock decisions close (Section 6).
**Purpose:** Define the first-year operating plan - year-1 objectives mapped to claims, the quarter plan (`Q | outputs | owner | cost line`), staffing and partners with statuses, the durability/survivor plan with named survivors, and risks with decision triggers - as the **framework** the concrete operating plan attaches to once DR-01/DR-06/DR-07 close. This file is the T08 deliverable of plan 001 (bucket CONTENT) and feeds T09 (unit-cost model + funding scenario).
**Sources:** `02-claim-ledger.md` (25 live claims C01-C28; E5 prohibition records C21/C22/C24), `04-delivery-and-budget.md` (delivery map W-01-W-13; budget workbook §2.1-§2.4; first-year boundary §3), `05-durability-risks-rights.md` (post-grant owner §1; risk register §2), `06-participant-pathway.md` (T05 framework), `07-platform-boundary.md` (T06 framework), `03-registers.md` (decision register rows DR-01/DR-04/DR-06/DR-07/DR-08/DR-09/DR-10).
**Cross-links:** `04-delivery-and-budget.md` §3 names this file as the first-year operating plan (cross-link target; "Nothing named yet → first-year plan cannot be built"); `02-claim-ledger.md` supplies the claims the objectives map to; `03-registers.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md` supply the carried states and frameworks. Planned files `09-unit-cost-model.md` (T09), `10-narrative.md` (T10) - backticked text, not links (do not exist yet). All owners are roles (per `03-registers.md` rules); named persons are `[INFORMATION NEEDED: program lead; required to name the person for each role (owner test); blocks the whole document - DR-01]`.

## 1. Year-1 objectives mapped to claims

**Reading note:** year-1 objectives cannot be concrete while DR-01/DR-06/DR-07 are undecided (all recorded **undecided as of 2026-10-14**, `03-registers.md` §1.1). Rows FY-01-FY-04 are carried by E1 claims and are therefore **concrete sustainment objectives** - the platform operates and the site stays accessible, conditions that hold as of 2026-10-14 (`02-claim-ledger.md` C01-C05, C27). Rows FY-05-FY-11 are carried by E4 option claims and are **markers**: the objective is to resolve the recorded decision or run the recorded test, never to assert the option's effect (C28: options recorded, not chosen). The year-1 boundary is **named capacity only** (`04-delivery-and-budget.md` §3.1); no objective implies expansion beyond unsigned capacity.

| ID | Year-1 objective | Claim ref | Grade | Owner (delivery-map role) | Cost line | Status |
|---|---|---|---|---|---|---|
| FY-01 | Platform operates: 15 live cabinets playable free, no account or payment gate | C01, C02, C03 | E1 | Technical owner (W-07) | Technology development, accessibility, security, maintenance | Sustained - holds as of 2026-10-14 |
| FY-02 | Site stays accessible: reduced-motion option, audio routing, browser-local preferences | C04 | E1 | Technical owner (W-07) | Technology development, accessibility, security, maintenance | Sustained - holds as of 2026-10-14 |
| FY-03 | Workbench honesty: 9 WIP builds stay labeled "COMING SOON"/"WIP BUILD" with the warning dialog | C27 | E1 | Technical owner (W-07) | Technology development, accessibility, security, maintenance - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Sustained - holds as of 2026-10-14 |
| FY-04 | No-outcome-claim discipline: engagement metrics never relabeled as outcomes; E5 prohibitions (C21/C22) honored | C05, C28; C21/C22 (E5 prohibition records) | E1/E4 (prohibitions E5) | Evidence reviewer (W-10) | Independent evaluation and data collection | Sustained - compliance objective |
| FY-05 | Define one beneficiary population with inclusion/exclusion rules and geography (DR-01 decision rule) | C10, C28 | E4 | Program lead | Participant support or compensation (where appropriate) - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker - blocks concrete planning |
| FY-06 | Choose one intervention with a defined participant pathway (delivery-map W-03) | C11 | E4 | Program lead | Community delivery and local partner costs - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker |
| FY-07 | Identify an eligible Lead Organization with actual control of funds (DR-02) | C09 | E4 | Authorized officer | Legal, safeguarding, insurance, financial administration - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker |
| FY-08 | Test the charitable-frame hypothesis and design incidental-private-benefit controls (DR-06) | C19, C20 | E4 | Decision owner + counsel | Legal, safeguarding, insurance, financial administration - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker |
| FY-09 | Test the outcome hypothesis under a pre-registered indicator at capability/progression/system level (DR-07 decision rule) | C28 | E4 | Program lead; named evaluator (TBD - W-10) | Independent evaluation and data collection - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker |
| FY-10 | Document the SF-establishment sequence: presence, locations, partner statuses (delivery-map W-08) | C23 | E1 (absence) | Program lead | Community delivery and local partner costs - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` | Marker - no SF capacity confirmed as of 2026-10-14 |
| FY-11 | Resolve the scope-lock decision gate: DR-01/DR-06/DR-07 closed with written rationale (Section 6) | C28; DR-01/DR-06/DR-07 rows | E1 (recorded states) | Program lead | None (decision; zero cost) | Marker - gate open as of 2026-10-14 |

**Objective-to-claim rule (binding):** no objective may appear in this table (or in any year-1 prose derived from it) without a claim reference from `02-claim-ledger.md`; a claim may move down in confidence, never up (ledger rules). Rows marked "Marker" become concrete only after the gate closes (Section 6).

## 2. Quarter plan (Q | outputs | owner | cost line)

**Reading note:** the quarter rows carry only framework outputs - decision-independent sustainment (grounded in E1 claims, FY-01-FY-04) and decision/process outputs with markers. The budget test (instructions.md §7.5) is satisfied by construction: every output has a cost line - either a named line category from `04-delivery-and-budget.md` §2.2 carrying `[INFORMATION NEEDED: budget owner; cost source - DR-04]` (DR-04 unselected, no amounts; indirect-cost line capped at 29% of direct project/activity costs, E1, rules §7) or an explicit zero-cost explanation. **No dollar figure appears anywhere.**

| Q | Outputs | Owner | Cost line |
|---|---|---|---|
| Q1 | Platform continuity verified: 15 live cabinets playable, site accessible, WIP labels intact (FY-01/FY-02/FY-03) | Technical owner (W-07) | Technology development, accessibility, security, maintenance - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q1 | Evidence-register rows added for C25-C28 in `03-registers.md` §3 (follow-up recorded in plan 010) | Evidence reviewer (W-10) | Independent evaluation and data collection - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q1 | Named-capacity inventory: which named people and partners can deliver which year-1 outputs (year-1 boundary, `04-delivery-and-budget.md` §3.1) | Program lead | `[INFORMATION NEEDED: program lead; named capacity - DR-01]` |
| Q1 | Decision-gate check: are DR-01/DR-06/DR-07 closed with rationale? (Section 6) | Program lead | None (decision; zero cost) |
| Q2 | Cost sources supplied for every named line category (L1-L4 build order, `04-delivery-and-budget.md` §2.1) | Budget owner (W-11) | All lines - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q2 | Platform maintenance continued; WIP builds remain honestly labeled (completion is a funded decision, not automatic) | Technical owner (W-07) | Technology development, accessibility, security, maintenance - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q2 | If the gate closed (Section 6): pathway and boundary cells replaced with concrete content (successor plans) | Program lead | Community delivery and local partner costs; participant support or compensation (where appropriate) - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q3 | Staffing plan with named persons per role (owner test; OY-01) | Program lead | Program staff and management - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q3 | Partner statuses updated to confirmed / in discussion / proposed per written confirmations (W-09; none confirmed as of 2026-10-14) | Program lead | Community delivery and local partner costs - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q3 | Evaluation instrument pre-registered (only if DR-07 closed; baseline defined before scaling, W-10) | Named evaluator (TBD - W-10) | Independent evaluation and data collection - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q4 | Year-1 review against objectives FY-01-FY-11; failures reported as follow-up plans, never silently fixed | Program lead | None (decision; zero cost) |
| Q4 | Unit-cost model inputs handed to T09 (`09-unit-cost-model.md`): quantities and cost sources per line | Budget owner (W-11) | All lines - `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| Q4 | Survivor plan updated with named payers and a retained-access rule (Section 4) | Executive owner | `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]` |

**Expansion rule (binding, `04-delivery-and-budget.md` §3.1):** expansion beyond year-1 named capacity is a decision, not an assumption - each expansion trigger needs a metric, threshold, review date, and the person authorized to approve it. No trigger is defined in this framework; triggers are `[INFORMATION NEEDED: program lead; metric, threshold, review date, approver - DR-01]`.

## 3. Staffing and partners (with statuses)

**Status rule (binding, from `04-delivery-and-budget.md` §1):** confirmed (**none**), in discussion (**none**), proposed (as marked). No person is named anywhere; every role below is a delivery-map role label and every named-person cell is `[INFORMATION NEEDED]` (OY-01). "No San Francisco delivery capacity or confirmed partner exists as of October 14, 2026" (`02-claim-ledger.md` C23).

### 3.1 Staffing (year-1 roles; delivery-map W-04-W-13)

| Role | Workstream | Year-1 function | Status | Named person |
|---|---|---|---|---|
| Technical owner | W-04, W-07 | Platform operation, maintenance, WIP labeling, acceptance tests | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead; named person for the role (owner test) - DR-01]` |
| Program lead | W-03, W-08, W-09 | Pathway design, SF establishment, partner engagement | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead; named person for the role (owner test) - DR-01]` |
| Budget owner | W-11 | Cost model, funding scenario (DR-04), cost sources | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead; named person for the role (owner test) - DR-01]` |
| Evidence reviewer / named evaluator | W-10 | Evaluation, pre-registered indicator (FY-09) | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead; named evaluator - DR-07]` |
| Authorized officer | W-01, W-13 | Lead-organization eligibility (DR-02); peer-review assignment (DR-08) | Proposed (role unnamed) | `[INFORMATION NEEDED: authorized officer; named person; named peer reviewer - DR-02/DR-08]` |
| Rights owner | W-12 | Rights/IP schedule (DR-09) | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead; named person for the role (owner test) - DR-01]` |
| Counsel | - | Charity-law review of incidental-private-benefit controls (DR-06) | Proposed (role unnamed) | `[INFORMATION NEEDED: program lead + counsel; named persons - DR-06]` |

### 3.2 Partners (statuses: confirmed (none) / in discussion (none) / proposed (as marked))

| Partner / organization | Proposed role | Status | Basis |
|---|---|---|---|
| Community Initiatives | Fiscal-sponsor candidate (DR-02 option c) | **proposed** - unapproached; capacity for the competition's award range (C06, E1) unverified | `03-registers.md` §1 DR-02; `04-delivery-and-budget.md` §1 W-09; `02-claim-ledger.md` C06 |
| Intersection for the Arts | Fiscal-sponsor candidate (DR-02 option c) | **proposed** - unapproached | `03-registers.md` §1 DR-02; `04-delivery-and-budget.md` §1 W-09 |
| SF city-source institutions (SF Arts Commission; Cultural Districts Program; OEWD; Rec & Park) | Evidence sources for the SF problem analysis - **not partners** | proposed (as evidence sources only; Rec & Park archived - conflict C6) | `03-registers.md` §1.1 DR-01 next action; `07-platform-boundary.md` §3 |
| Neighborhood / community organizations | Referral and supervision of participants (`06-participant-pathway.md` §2) | none named | `[INFORMATION NEEDED: program lead; partner targets and statuses - DR-01/DR-06]` |
| Business / landmark owners | Permissions for SF depictions (C15; DR-06 frame) | none named | `[INFORMATION NEEDED: program lead; permissions - DR-06]` |
| Other applicants (competition) | Peer-review obligation: 4 (up to 6) applications reviewed, ~2.5 h, Nov-Dec 2026 (C06; W-13) | obligation, not a partnership | `[INFORMATION NEEDED: authorized officer; named reviewer - DR-08]` |

## 4. Durability / survivor plan (grant ends → named survivors)

**Reading note:** the durability test (instructions.md §7.6) requires named survivors. Per `04-delivery-and-budget.md` §3.3 (after grant: **retained assets**, **adopted activities**, **funded operations**), only **retained assets** can be named today - the platform and its settings, which exist independent of any grant (E1 claims C01-C04, C27). Adopted activities and funded operations carry markers: nothing is adopted or funded by default (DR-10 undecided; `05-durability-risks-rights.md` §1: "What survives if the company changes or exits" and "who pays operating costs after the grant" both `[INFORMATION NEEDED]`).

| Survivor | Type | Evidence basis | Continuity condition | Owner |
|---|---|---|---|---|
| Live platform: 15 playable cabinets, free browser access, no account gate | Retained asset | E1 (C01-C03; exists as of 2026-10-14) | Hosting/domain continuity; rights schedule (DR-09); post-grant payer | Technical owner; payer `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]` |
| Workbench: 9 WIP builds, honestly labeled with the warning dialog | Retained asset (as-is) | E1 (C27) | Completion is a funded decision, not an automatic survivor | Technical owner |
| Accessibility settings: reduced motion, audio routing, browser-local preferences | Retained asset | E1 (C04) | Built-in; no maintenance cost documented | Technical owner |
| Adopted activities (recruitment, sessions, instruction, assessment, safeguarding) | Adopted activity | None - no activity defined (DR-01/DR-06/DR-07 undecided) | `[INFORMATION NEEDED: program lead; adoption commitments - DR-01/DR-10]` | Program lead |
| Funded operations (staff, sites, evaluation) | Funded operation | None - no operating-cost model exists | `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]` | Executive owner |
| Retained public access rule | Funded operation | None - no free-access rule (DR-06) | `[INFORMATION NEEDED: program lead; free-access rules - DR-06]` | Program lead |
| Continuity if the company changes or exits | Retained asset (conditional) | None - assignment/continuity terms unknown | `[INFORMATION NEEDED: rights owner; license continuity - DR-09]` | Rights owner |

**No-default-continuation rule (binding, `04-delivery-and-budget.md` §3.3):** "Every activity continuing unchanged by default" is excluded; an activity continues only when a named owner, payer, and retained-access condition exist (DR-10 decision rule).

## 5. Risks (with decision triggers)

**Reading note:** carried from `05-durability-risks-rights.md` §2 (7 categories + eligibility), year-1 framing. A risk without a decision trigger is only a description (05 §2 rule); every trigger threshold is `[INFORMATION NEEDED]` because no beneficiary, pathway, or cost model exists.

| Risk | Year-1 trigger (what result → what action) | Owner | Status |
|---|---|---|---|
| Demand - will intended participants enroll? | Enrollments below [threshold] in pilot period → reduce cohort, change channel, or revise beneficiary (DR-01) | Program lead | Thresholds `[INFORMATION NEEDED: program lead; DR-01]` |
| Delivery - can staff deliver the model? | Facilitator caseload/session quality below standard → pause cohort; do not expand | Program lead | No staff named (Section 3) |
| Mechanism - will activities produce outcomes? | Pre-registered outcome metric misses [threshold] → correct method or redesign intervention before scaling | Evidence reviewer | No outcome chosen (DR-05/DR-07) |
| Adoption - will institutions continue it? | No adoption commitment by [date] → pursue named alternative owner (DR-10) | Executive owner | No institutions named |
| Technical - will the platform support delivery? | Acceptance test fails → manual fallback or delay launch; feature stays outside the prospectus until tested | Technical owner | No acceptance tests defined (W-04) |
| Financial - will costs exceed assumptions? | Cost-model variance > [X%] → resize scenario or request (DR-04) | Budget owner | No cost model (DR-04 unselected) |
| Control - can the lead supervise funds and partners? | Control finding in [review period] → remediation plan; unresolved → stop spending | Authorized officer | Lead unresolved (DR-02) |
| Eligibility/registration - is there a valid route to submit? | No registration/exception by Oct 15 2026 → stop drafting; gap report only (DR-03) | Authorized officer | Immediate go/no-go |

**Scoring note (05 §2):** risks are scored by their effect on the project logic, not by general seriousness; each risk must be matched to a design choice, contingency, or evaluation question in the prospectus.

## 6. Decision gate - when the first-year plan becomes draftable

The year-1 objectives FY-05-FY-11, the quarter outputs Q2-Q4, staffing names, partner statuses, and survivor rows **cannot be drafted while DR-01, DR-06, and DR-07 are undecided** (all recorded **undecided as of 2026-10-14**, `03-registers.md` §1.1; consequence of delay: all downstream work pauses; the packet stays Not ready). This document is the framework those decisions attach to.

**Gate:** DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) each closed in `03-registers.md` §1.1 with a decided value, deciding owner, date, and evidence grade (plans 001 T02-T04 recorded the undecided states; changes 005/006/007).

**Once the gate opens:** a follow-on plan (successor to this plan, still T08 content) replaces every placeholder and `[INFORMATION NEEDED]` cell in Sections 1-4 with concrete content, per delivery-map workstreams W-03/W-05/W-06/W-08/W-09 (`04-delivery-and-budget.md` §1: start condition = scope lock W-02; outputs = approved pathway, enrolled participants, completed sessions, SF establishment, written confirmations), under the DR-04 funding-scenario selection (W-11). This file is then re-verified with the full editing-test set (instructions.md §7).

**Until then:** no draftable first-year plan exists; this framework stands on its own - the deletion test passes (the framework does not depend on the FTSArcade name) and the substitution test passes (E1-grounded rows are site facts that hold under substitution; all other cells carry no invented SF facts).

## 7. Revision record (per methodology)

| Date | Proposed change | Class | Reason | Evidence affected | Budget affected | Decision | Updated documents |
|---|---|---|---|---|---|---|---|
| 2026-10-14 | First-year operating plan framework created (framework-only: year-1 objectives mapped to claims - E1 rows FY-01-FY-04 concrete sustainment objectives, E4 rows FY-05-FY-11 markers; quarter table Q \| outputs \| owner \| cost line with named line categories and zero-cost explanations; staffing and partners with statuses (confirmed/in discussion: none; proposed as marked); durability/survivor plan with named survivors = retained assets only (live platform, workbench WIP builds, accessibility settings), adopted activities/funded operations as markers; risks with decision triggers (7 categories + eligibility, carried from 05 §2); decision-gate note (first-year plan draftable only after DR-01/DR-06/DR-07 close); DR-04/DR-08/DR-09/DR-10 states propagated) | Clarifying | Plan 001 T08 (CONTENT) requires the first-year operating plan; DR-01/DR-06/DR-07 undecided and DR-04 unselected as of 2026-10-14, so the change records the framework - no invented outputs, owners, costs, or partners | DR-01/DR-04/DR-06/DR-07/DR-08/DR-09/DR-10 decision states propagated (E1, source: `03-registers.md` §1.1/§1; ungraded - undecided); E1 platform claims (C01-C05, C27) carried; no new figures | None - zero dollar figures; every cost line carries `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation | No decision closed; first-year plan stays not draftable until scope lock | 08-first-year-operating-plan.md (new), Logs/changes.md, Plan/000-index.md |
```

### 2.3 INFORMATION NEEDED markers list (must appear in the file)

The OY-01…OY-11 table below is the consolidated unknowns list; the complete inline marker texts appear in Sections 1-4 and 6 of the file exactly as written in §2.2. Count: **38 inline `[INFORMATION NEEDED: ...]` markers** (1 in the preamble cross-links line, 7 in the Section 1 objective table, 13 in Section 2 - 11 in the quarter-table rows, 1 in the reading note, 1 in the expansion-rule line - 7 in the Section 3.1 staffing table, 3 in the Section 3.2 partners table, 5 in the Section 4 survivor table, 1 in the Section 5 risk table, 1 in the Section 7 revision record), each with owner + why + decision-blocked fields per instructions.md §5, each grouped into exactly one of the OY rows below. (The Status-line phrase "`[INFORMATION NEEDED: ...]`" is a format description, not a marker; `grep -c` on the file reads **39** hits including it - V5 accounts for this.)

| ID | Owner | Decision blocked | Unblocks |
|---|---|---|---|
| OY-01 | Program lead | DR-01 | Whole document (named persons per role) |
| OY-02 | Program lead | DR-01 | Section 1 (beneficiary definition; F-11 reachable-population estimate) |
| OY-03 | Program lead | DR-01/DR-05 | Section 1 (intervention + pathway; W-03) |
| OY-04 | Program lead + counsel | DR-06 | Sections 1/3/4 (charitable frame, site plan, access rules, free-access rule) |
| OY-05 | Named evaluator | DR-07/DR-05 | Sections 1/2 (pre-registered indicator; Q3 evaluation instrument) |
| OY-06 | Budget owner | DR-04 | Section 2 (cost sources per line; L1-L4 build order) |
| OY-07 | Program lead | DR-01 | Section 2 (named-capacity inventory; year-1 boundary) |
| OY-08 | Program lead | DR-06 | Section 3 (partner targets and statuses) |
| OY-09 | Executive owner | DR-10 | Section 4 (post-grant payer + operating-cost model) |
| OY-10 | Rights owner | DR-09 | Section 4 (rights/IP schedule; license continuity) |
| OY-11 | Authorized officer | DR-08 | Section 3 (named peer reviewer, W-13) |

---

## 3. F3 - `Documentation/Logs/changes.md`

**Append one row after the plan-010 row (currently line 18), same column format (8 columns; pipes inside cells escaped as `\|` where table formats are named):**

```
| 2026-10-14 | Clarifying | Create first-year operating plan (`Prospectus/08-first-year-operating-plan.md`, new): framework-only - year-1 objectives mapped to claims (E1 rows FY-01-FY-04 carry concrete sustainment objectives from claims C01-C05/C27; E4 rows FY-05-FY-11 carry markers - no objective asserted while DR-01/DR-06/DR-07 undecided); quarter table Q \| outputs \| owner \| cost line with named line categories (04 §2.2) and zero-cost explanations - zero dollar figures; staffing and partners with statuses (confirmed/in discussion: none; proposed as marked - fiscal-sponsor candidates only); durability/survivor plan with named survivors = retained assets only (live platform, workbench WIP builds, accessibility settings; adopted activities/funded operations as markers); risks with decision triggers (7 categories + eligibility, carried from 05 §2); decision-gate note (first-year plan draftable only after DR-01/DR-06/DR-07 close); DR-04/DR-08/DR-09/DR-10 states propagated | Plan 001 T08 (CONTENT) requires the first-year operating plan; DR-01/DR-06/DR-07 undecided and DR-04 unselected as of 2026-10-14, so the change records the framework - no invented outputs, owners, costs, or partners | DR-01/DR-04/DR-06/DR-07/DR-08/DR-09/DR-10 decision states propagated (E1, source: 03-registers.md §1.1/§1; ungraded - undecided); E1 platform claims (C01-C05, C27) carried; no new figures; no budget affected | No decision closed - first-year plan stays not draftable until scope lock | Prospectus/08-first-year-operating-plan.md (new), Logs/changes.md, Plan/000-index.md | 011 |
```

---

## 4. F4 - `Documentation/Plan/000-index.md`

**Append one row after the plan-010 row (currently line 18):**

```
| 011 | `Documentation/Plan/011-first-year-plan.md` | First-year operating plan framework: year-1 objectives mapped to claims, quarter plan, staffing/partners, survivors, risks (plan 001 T08) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 5. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T08: budget test; durability test; owner test; plus the honesty checks below. Per instructions.md §11.6, the orchestrator starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T08; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No invented outputs/owners/costs/partners | Read `Documentation/Prospectus/08-first-year-operating-plan.md` against §2.2 of this plan; `grep -nE '\$[0-9]' Documentation/Prospectus/08-first-year-operating-plan.md` | The file matches §2.2 verbatim: 0 dollar-figure hits; 0 named persons, 0 organization names beyond the delivery-map role labels and the two recorded fiscal-sponsor candidates (Community Initiatives, Intersection for the Arts - proposed), 0 SF locations, 0 partner statuses beyond proposed/none named; no objective, quarter output, or survivor beyond the FY/Q/survivor rows specified |
| V2 | Budget test (every promised output has a cost) | Parse the Section 2 quarter table (13 rows): each row's cost-line cell is non-empty and passes if it is (a) a named `04-delivery-and-budget.md` §2.2 line category (with the DR-04 marker), (b) an explicit zero-cost explanation (`None (decision; zero cost)`), or (c) a pure `[INFORMATION NEEDED: ...]` marker (Q1 named-capacity inventory, Q4 survivor-plan-update rows are valid) | 13/13 rows pass; 0 rows with an empty cost line; the 2 zero-cost rows (Q1 decision-gate check, Q4 year-1 review) carry explicit zero-cost explanations; the 2 pure-marker rows (Q1 named-capacity inventory, Q4 survivor-plan-update) pass as pure `[INFORMATION NEEDED]` cells; no dollar figure in any cost line |
| V3 | Durability test (grant ends → named survivors) | Inspect Section 4 | ≥ 3 named retained-asset survivors (live platform; workbench WIP builds; accessibility settings), each with an owner role and a continuity condition; adopted activities and funded operations are `[INFORMATION NEEDED]` markers, never defaults; no row asserts post-grant continuation without a condition |
| V4 | Owner test (every action verb has a named party) | Underline every action verb in the new file | Each action is either (a) performed by a named role (technical owner, program lead, budget owner, evidence reviewer, authorized officer, executive owner, rights owner, counsel, named org/team/evaluator TBD, etc.) or (b) inside an `[INFORMATION NEEDED: <owner>; ...]` marker naming the owner; 0 unattributed action verbs |
| V5 | INFORMATION NEEDED markers complete | `grep -c "\[INFORMATION NEEDED:" Documentation/Prospectus/08-first-year-operating-plan.md` + inspect each marker | Count **39** (38 markers + the Status-line format description, which is not a marker); every marker has the format `[INFORMATION NEEDED: <owner>; <why>; ... <decision blocked>]` with a named role owner and a blocked decision; the §2.3 table contains exactly rows OY-01…OY-11 and every inline marker maps to one of them. **Record the verified count in the changes.md row.** |
| V6 | Undecided states propagated | `grep -nE 'DR-01|DR-04|DR-06|DR-07|DR-08|DR-09|DR-10|undecided as of 2026-10-14' Documentation/Prospectus/08-first-year-operating-plan.md` | The wording "undecided as of 2026-10-14" appears for DR-01/DR-06/DR-07 (03 §1.1 wording); DR-04 unselected, DR-08 named-reviewer, DR-09 rights, DR-10 operating-model markers present; no decision is closed anywhere in the file |
| V7 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/08-first-year-operating-plan.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits in the three executed files (the plan file and instructions.md §6's own list are exempt by construction); grep "unique" likewise - 0 hits; "sustainable" must not appear in the survivor plan ("post-grant" is used) |
| V8 | Tables render | For every table in the new file (Sections 1, 2, 3.1, 3.2, 4, 5, 7): header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each; the `\|` escapes inside the §7 revision-record cell render as a literal pipe without breaking the row |
| V9 | Cross-links resolve | `test -f Documentation/Prospectus/02-claim-ledger.md Documentation/Prospectus/03-registers.md Documentation/Prospectus/04-delivery-and-budget.md Documentation/Prospectus/05-durability-risks-rights.md Documentation/Prospectus/06-participant-pathway.md Documentation/Prospectus/07-platform-boundary.md; echo "EXIT:$?"` + extract every `](…)` target from the new file | All six files exist (EXIT:0); every relative link target in the file resolves with `test -f`; 0 dangling links (planned-file cross-links `09-unit-cost-model.md` / `10-narrative.md` are backticked text, not links) |
| V10 | No drafting boundary | `grep -niE 'dear|subject:|sincerely' Documentation/Prospectus/08-first-year-operating-plan.md` | 0 hits (protocol R1; no email or promotional text introduced) |
| V11 | changes.md row | Inspect `Documentation/Logs/changes.md` | One new row: class **Clarifying**, plan ref 011, date 2026-10-14, documents updated listing the new file + `Logs/changes.md` + `Plan/000-index.md`; appended after the plan-010 row; existing rows unchanged |
| V12 | Index self-consistency | `grep -c '| 011 |' Documentation/Plan/000-index.md` | Output **1**; the row's status is `planned` (orchestrator flips it through the lifecycle after review); existing rows 001-010 unchanged |
| V13 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | Exactly 1 new file (`Documentation/Prospectus/08-first-year-operating-plan.md`) + exactly 2 modified files (`Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md`); `Documentation/Plan/011-first-year-plan.md` appears as the pre-plan artifact (untracked); no other file touched; no deletions |

---

## 6. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| DR-01/DR-04/DR-06/DR-07/DR-08/DR-09/DR-10 decision states, verbatim | `Documentation/Prospectus/03-registers.md` §1.1 (DR-01/DR-06/DR-07) and §1 rows (DR-04/DR-08/DR-09/DR-10) | Preamble and Sections 1, 3, 4, 6 carry the states; quote-fidelity rule (stop if drifted, do not patch blind) |
| Claim texts C01-C05, C09-C11, C19, C20, C23, C27, C28 (+ E5 prohibition records C21/C22) | `Documentation/Prospectus/02-claim-ledger.md` | Section 1 objective rows map to claim refs and grades; Section 4 survivor rows cite the E1 claims |
| Delivery-map role labels (W-01-W-13) and their statuses | `Documentation/Prospectus/04-delivery-and-budget.md` §1 | Staffing rows (Section 3.1) and partner rows (3.2) must match the delivery map's roles exactly; status rule "confirmed (none), in discussion (none), proposed (as marked)" |
| Line category names (L1-L4; §2.2 lines) and first-year boundary (§3) | `Documentation/Prospectus/04-delivery-and-budget.md` §2.1-§2.2, §3 | Quarter-table cost lines name the §2.2 categories verbatim; the year-1 boundary wording "capacity that named people and partners can deliver" is quoted in §1/§2 |
| Risk register rows (7 categories + eligibility) with triggers | `Documentation/Prospectus/05-durability-risks-rights.md` §2 | Section 5 carries the trigger→action pairs and owner roles |
| Post-grant owner table | `Documentation/Prospectus/05-durability-risks-rights.md` §1 | Section 4 survivor rows draw the payer/access/continuity markers |
| Marker syntax + change-class definitions | `Documentation/Logs/instructions.md` §5, §9.2 | `[INFORMATION NEEDED: <owner>; why; decision blocked]` format; class Clarifying |
| Current row positions in F3/F4 | `Documentation/Logs/changes.md` (line 18), `Documentation/Plan/000-index.md` (line 18) | Append after the plan-010 rows; re-check at execution |

**Explicitly out of scope for the executor:** choosing or recommending any option of DR-01/DR-06/DR-07 (including naming an indicator, population, site, partner, or provider - any such action violates this plan); inventing any output, owner, cost figure, or partner; editing `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `02-claim-ledger.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, root `README.md`, `Documentation/Research/*`, or `Documentation/Refinement/*` (their records already exist and are referenced, not duplicated); drafting any email or promotional copy (protocol R1); committing (orchestrator-only, rule R2).

---

## 7. Revision note (plan amendments)

| Date | Amendment | Class | Reason |
|---|---|---|---|
| 2026-10-14 | Round-2 plan amendment (orchestrator-approved): FY-03 cost line renamed to the recorded §2.2 category `Technology development, accessibility, security, maintenance` with the `[INFORMATION NEEDED: budget owner; cost source - DR-04]` marker added; FY-05 and the Q2 if-gate-closed cost lines renamed to `Participant support or compensation (where appropriate)`; V2 pass rule extended to accept pure INFORMATION NEEDED cells; §2.3/V5 marker counts updated (38 inline markers; 39 `grep -c` hits) | Clarifying | Quote fidelity: embedded §2.2 cost-line names must match the recorded `04-delivery-and-budget.md` §2.2 categories |