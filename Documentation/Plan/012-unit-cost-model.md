# 012 - Unit-Cost Model and Funding Scenario: Unit Definitions, Cost Drivers, Three Scenarios (T09)

> **For Hermes:** Execute this plan with one execute agent. The executor writes `Documentation/Prospectus/09-unit-cost-model.md` as a **structured unit-cost-model framework - not a draft budget** - because DR-04 (funding scenario) is **unselected as of 2026-10-14** (`03-registers.md` §1) and no cost figure exists anywhere (every amount in `04-delivery-and-budget.md` is `[INFORMATION NEEDED]`; changes 008-011 recorded zero dollar figures). The executor edits exactly three files (F2-F4), never commits, and reports the verified marker count. The orchestrator reviews, commits once (`docs(grant): unit-cost model and funding-scenario framework (T09)`), and flips the 000-index row through the lifecycle.

**Goal:** Satisfy plan 001 task T09 (bucket CONTENT) by creating `Documentation/Prospectus/09-unit-cost-model.md` - a STRUCTURED UNIT-COST MODEL AND FUNDING-SCENARIO FRAMEWORK: (1) unit definition and unit cost per output; (2) cost drivers; (3) funding scenarios table `request level | covered outputs | lost outputs | basis`; (4) assumptions with grades; (5) request-amount rule (never invented; DR-04 records it when chosen); (6) decision-gate note - and appending the changes.md row and the 000-index.md row. No unit cost, volume, or total is invented: every Figure cell is `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation; every scenario cell is structural or a marker; zero dollar figures.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and the T09 task detail): no scope change occurs - no option of DR-04 (funding scenario) is chosen or redefined, and no budget number changes; the change adds missing information (the unit-cost model framework and the propagated DR-04/DR-10 states) and creates one new packet document. This mirrors the Clarifying precedent of changes 004-011 (recorded undecided/unselected decision states; pathway, boundary, claim-ledger, and first-year-plan frameworks). Operational would apply to budget numbers; the document adds none (zero dollar figures). Foundational would apply only if the decisions were made and changed scope; they are not.

**Scope - in:** the 3 files listed in Section 1 (F2-F4) plus this plan file (F1, already written by the pre-plan agent).
**Scope - out:** choosing or recommending any DR-04 scenario or request amount (selecting the scenario and recording the amount is a **successor change** that edits `03-registers.md` - this plan explicitly does not choose it); inventing unit costs, volumes, or totals; edits to `03-registers.md`, `08-first-year-operating-plan.md`, `04-delivery-and-budget.md`, `02-claim-ledger.md`, `01-source-case.md`, `00-prospectus.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, root `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/012-unit-cost-model.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/09-unit-cost-model.md` | **New file** (verified absent at plan time): the unit-cost model and funding scenario framework - write the Section 2.2 content verbatim |
| F3 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 012) after the plan-011 row (currently line 19) |
| F4 | `Documentation/Plan/000-index.md` | Modify: append row 012, status `planned`, after the plan-011 row (currently line 19) |

---

## 2. F2 - `Documentation/Prospectus/09-unit-cost-model.md` (NEW FILE)

### 2.1 File-level rules (binding)

- Write the file exactly as the fenced content in §2.2: headers verbatim, tables verbatim, cell text verbatim, relative links only. Do not add, remove, or reword any section, row, cell, or marker.
- All owners are **roles** (per `03-registers.md` rules: "All owners are roles; named persons are `[INFORMATION NEEDED: ...]`"). No person's name, no organization name beyond the delivery-map role labels ("budget owner", "program lead", "executive owner", "technical owner", "evidence reviewer", "named evaluator (TBD - W-10)"), and no SF location may be invented.
- Zero dollar figures: the string `$` must not appear in the file (V1). The only cost rule quoted is the indirect-cost cap (≤29% of direct project/activity costs, E1, rules §7), named as a line rule, not an amount; the competition's award limit is never written with a dollar figure.
- No prohibited words (instructions.md §6): revolutionary, world-class, unique, cutting-edge, empower, unlock, transform, scalable, sustainable, "partners include", "data shows" - 0 hits. In particular, "scalable" never appears: the framework contains no unit-cost figures, so no scalable claim can exist (instructions.md §6: "scalable - only with a unit cost"). "sustainable" never appears (the adoption-timing driver says "post-grant").
- Quote fidelity: before writing, re-read `Documentation/Prospectus/03-registers.md` §1 (DR-04 row) and §2 (F-04, F-07, F-09), `04-delivery-and-budget.md` §2.1-§2.3 (four layers, line categories, three scenarios, proportionality rules), and `08-first-year-operating-plan.md` §1 (FY-01-FY-11) and §2 (Q1-Q4). If the recorded wording drifted from what §2.2 quotes, **stop and report - do not paraphrase or patch blind** (mirrors plans 008/009/011's quote-fidelity rule).
- Cross-links to planned files (`10-narrative.md`) are plain backticked text, NOT markdown links - they do not exist yet, and dangling links fail V8.
- The `\\|` escapes inside the §7 revision-record cell of the §2.2 fence render as `\|` in the target file (mirrors 08 §7 and 011 §2.2; the double backslash is the plan-file escaping of the literal pipe).

### 2.2 Complete file content (write exactly this)

```
# Unit-Cost Model and Funding Scenario - FTSArcade / Boundless San Francisco

**Version:** S0 (framework only) · **Date:** 2026-10-14
**Status:** **FRAMEWORK ONLY - NOT DRAFTABLE.** As of 2026-10-14, DR-04 (funding scenario) is **unselected** (`03-registers.md` §1) and no cost figure exists anywhere: every amount in `04-delivery-and-budget.md` is `[INFORMATION NEEDED: <owner>; cost source]` and changes 008-011 recorded zero dollar figures. Every unit-cost cell, sensitivity estimate, and request amount below is a structural cell or an `[INFORMATION NEEDED: ...]` marker; **no unit cost, volume, or total is invented.** The unit-cost model becomes draftable only when DR-04 is chosen and cost sources are supplied (Section 6).
**Purpose:** Define the unit-cost model and funding-scenario framework - unit definitions per year-1 output, cost drivers, the three funding scenarios with covered/lost structure, graded assumptions, and the request-amount rule - as the **framework** the concrete budget attaches to once DR-04 is selected (delivery-map W-11). This file is the T09 deliverable of plan 001 (bucket CONTENT), is fed by the T08 first-year operating plan, and feeds T10 (narrative).
**Sources:** `04-delivery-and-budget.md` (four-layer cost model §2.1; line categories §2.2; three scenarios §2.3; budget-narrative formula §2.4; year-1 boundary §3), `08-first-year-operating-plan.md` (year-1 objectives FY-01-FY-11 §1; quarter plan Q1-Q4 §2), `03-registers.md` (DR-04 funding-scenario row §1; DR-10 durability row §1; data dictionary F-04 unit cost, F-07 indirect-cost cap, F-09 award request §2), `02-claim-ledger.md` (C23 - no SF delivery capacity or confirmed partner exists as of 2026-10-14), `Logs/instructions.md` (proportionality test §7.7; prohibited words §6).
**Cross-links:** `08-first-year-operating-plan.md` §2 names this file's inputs (Q4: "Unit-cost model inputs handed to T09 (`09-unit-cost-model.md`): quantities and cost sources per line"); `04-delivery-and-budget.md` §2.1-§2.3 is the cost-model spec this framework instantiates. Planned file `10-narrative.md` (T10) - backticked text, not a link (does not exist yet). All owners are roles (per `03-registers.md` rules); named persons are `[INFORMATION NEEDED: program lead; required to name the person for each role (owner test); blocks the whole document - DR-01]`.

## 1. Unit definition and unit cost per output

**Reading note:** units attach to the year-1 outputs of `08-first-year-operating-plan.md` §1 (FY-01-FY-11) and the Q3 staffing-plan output. A unit is the quantity a cost attaches to (data dictionary F-04: "Eligible costs ÷ completers"; `04-delivery-and-budget.md` §2.1 L1: cost per session, participant, site, license, staff role). **No unit cost exists as of 2026-10-14**: every Figure cell carries `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation. The budget test (instructions.md §7.5) is satisfied by construction: every year-1 output has a unit row below.

| Unit ID | Unit | Definition | Output ref (08 §1/§2) | Cost line (04 §2.2) | Figure |
|---|---|---|---|---|---|
| UC-01 | Cabinet-month | One live cabinet kept playable for one month | FY-01 | Technology development, accessibility, security, maintenance | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-02 | Site-month | One platform site kept accessible for one month (hosting, domain, accessibility settings) | FY-02 | Technology development, accessibility, security, maintenance | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-03 | WIP build-year | One workbench build kept labeled "COMING SOON"/"WIP BUILD" with the warning dialog for one year | FY-03 | Technology development, accessibility, security, maintenance | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-04 | Evidence-review pass | One evidence-register review pass (`03-registers.md` §3 rows) | FY-04 | Independent evaluation and data collection | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-05 | Beneficiary-definition package | One decision package: population, inclusion/exclusion rules, geography (DR-01 decision rule) | FY-05 | Participant support or compensation (where appropriate) | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-06 | Pathway-design package | One approved pathway: first contact → completion (delivery-map W-03) | FY-06 | Community delivery and local partner costs | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-07 | Legal-compliance package | One entity-eligibility and funds-control review (DR-02) | FY-07 | Legal, safeguarding, insurance, financial administration | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-08 | Frame-test package | One charitable-frame test including incidental-private-benefit controls design (DR-06) | FY-08 | Legal, safeguarding, insurance, financial administration | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-09 | Pre-registered instrument | One pre-registered evaluation instrument (baseline, target, instrument, collection timing; DR-07 decision rule) | FY-09 | Independent evaluation and data collection | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-10 | SF-establishment sequence | One documented SF-establishment sequence: presence, locations, partner statuses (delivery-map W-08) | FY-10 | Community delivery and local partner costs | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| UC-11 | Decision-gate resolution | The scope-lock gate closed with written rationale (`08-first-year-operating-plan.md` §6) | FY-11 | None (decision; zero cost) | Zero-cost explanation - no cost attaches |
| UC-12 | Staff role-month | One delivery-map role filled for one month (`08-first-year-operating-plan.md` §3.1 staffing plan) | Q3 | Program staff and management | `[INFORMATION NEEDED: budget owner; cost source - DR-04]` |
| - | Indirect-cost allocation | Allocation of overhead to direct lines; **cap: 29% of direct project/activity costs, within the competition's award limit** (E1, rules §7 - quoted as a line rule, not an amount) | All direct lines | Indirect costs | `[INFORMATION NEEDED: budget owner; allocation method - DR-04]` |

**Unit-cost rule (binding):** every unit's Figure cell stays `[INFORMATION NEEDED: budget owner; cost source - DR-04]` until the budget owner supplies a verified figure from a named source (`08-first-year-operating-plan.md` §2 Q2: "Cost sources supplied for every named line category"); a unit without a cost source is a marker, never a number (`04-delivery-and-budget.md` §2.1 L1: "not started"). Per instructions.md §6, statements about how the model can grow in scale require a unit cost; the framework contains no unit-cost figures, so it makes no such statement.

## 2. Cost drivers

**Reading note:** drivers are carried from `04-delivery-and-budget.md` §2.4 (name the operating assumption; show quantity and unit cost; state what happens if the assumption changes) and §2.1 L4 (costs affected by enrollment, facilities, staffing, delayed adoption) and from `08-first-year-operating-plan.md` §5 risk triggers. The Effect cell states the direction of effect structurally; every sensitivity estimate is a marker - no sensitivity number is invented.

| Driver | Effect | Sensitivity marker |
|---|---|---|
| Enrollment volume | Changes participant-support and delivery quantities (L2 operating volume; 08 §5 Demand) | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Session / cohort count | Changes facilitator, facility, and session quantities | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Platform maintenance incidents | Changes the technology line (UC-01-UC-03 quantities; 08 §5 Technical) | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Staffing levels | Changes the program-staff line (UC-12 quantity; 08 §5 Delivery) | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Site / facility count | Changes the community-delivery line (UC-06/UC-10 quantities) | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Evaluation scope | Changes the independent-evaluation line (UC-04/UC-09 quantities) | `[INFORMATION NEEDED: budget owner; sensitivity estimate - DR-04]` |
| Adoption timing | Changes which costs continue after the grant (DR-10; 04 §2.4 step 5) | `[INFORMATION NEEDED: executive owner; post-grant operating-cost model - DR-10]` |

**Sensitivity rule (binding):** the sensitivity cells are the L4 contingency inputs (`04-delivery-and-budget.md` §2.1 L4: "costs affected by enrollment, facilities, staffing, delayed adoption"); when DR-04 is chosen the budget owner supplies the L4 range per driver, never a point figure without a source.

## 3. Funding scenarios (request level | covered outputs | lost outputs | basis)

**Reading note:** the three scenarios are defined in `04-delivery-and-budget.md` §2.3 and the DR-04 register row; no amounts exist as of 2026-10-14 - every cell below is structural or a marker. "Lost outputs" answers the proportionality test (instructions.md §7.7: reduce the request by half, state exactly which outputs disappear).

| Scenario | Request level | Covered outputs | Lost outputs | Basis |
|---|---|---|---|---|
| **Constrained** | Essential pilot and evidence-building only | FY-01-FY-04 sustainment (E1 platform + compliance), FY-09 evaluation instrument, FY-11 gate resolution (UC-01-UC-04, UC-09, UC-11) | All scale outputs (UC-05-UC-08, UC-10: beneficiary package, pathway, legal-compliance, frame test, SF-establishment sequence) - exact loss list `[INFORMATION NEEDED: budget owner; lost-output enumeration - DR-04]` | Pilot cohorts, minimum platform work, independent evaluation, legal/compliance (`04-delivery-and-budget.md` §2.3) |
| **Proposed** | Scale justified by delivery capacity | Full delivery-plan volumes (delivery-map W-03-W-08; `04-delivery-and-budget.md` §2.3) - UC-01-UC-12 at planned volumes | Outputs that disappear if the request drops to the constrained level (the scale set above) - exact loss list `[INFORMATION NEEDED: budget owner; lost-output enumeration - DR-04]` | Request = supported costs; never start at the maximum (`04-delivery-and-budget.md` §2.3); delivery-capacity statement `[INFORMATION NEEDED: budget owner + program lead; delivery-capacity statement - DR-04]` |
| **Maximum** | Scale requiring additional CONFIRMED capacity, not merely more money | Outputs that depend on confirmed partners, staff, sites, and adoption commitments (W-05/W-06/W-08/W-09) | Outputs that cannot yet be executed responsibly - assessment `[INFORMATION NEEDED: program lead; responsible-execution assessment - DR-01/DR-04]` | Additional confirmed capacity (none as of 2026-10-14, `02-claim-ledger.md` C23) - capacity `[INFORMATION NEEDED: program lead; confirmed capacity - DR-01/DR-04]` |

**Proportionality rule (binding):** halving the request removes exactly the stated lost outputs. When DR-04 is chosen, the budget owner enumerates the selected scenario's loss list (which outputs disappear at half the request, and why the original request is consequently justified - instructions.md §7.7, `04-delivery-and-budget.md` §2.3); the enumeration is recorded in `03-registers.md` with the DR-04 entry - never invented, never left blank. The selected scenario's basis explains why cheaper options fail (their lost outputs) and why larger ones cannot yet be executed responsibly (unconfirmed capacity).

## 4. Assumptions with grades

**Reading note:** every material assumption carries a grade E1-E5 and a test (instructions.md §5); an E4 assumption is labeled an assumption and includes a test - no ungraded assumption appears.

| Assumption | Grade | Source | Test |
|---|---|---|---|
| A1 - No cost figure exists anywhere as of 2026-10-14 (DR-04 unselected; every figure is a marker) | E1 | `04-delivery-and-budget.md` rules line; changes 008-011 (zero dollar figures) | Re-verify at execution: dollar-figure scan → 0 hits |
| A2 - Unit costs can be sourced per line category from named sources | E4 | `04-delivery-and-budget.md` §2.1 L1 ("not started") | Budget owner supplies one verified figure per line (`08-first-year-operating-plan.md` §2 Q2); failure → the unit stays a marker |
| A3 - Year-1 volumes match named capacity only | E1 | `04-delivery-and-budget.md` §3.1 | Named-capacity inventory (`08-first-year-operating-plan.md` §2 Q1); no volume exceeds named capacity |
| A4 - Indirect costs are capped at 29% of direct project/activity costs, within the award limit | E1 | rules §7 (`03-registers.md` §2 F-07) | Re-verify the rules page before submission |
| A5 - The proportionality test's lost outputs are enumerable per scenario | E4 | instructions.md §7.7; `04-delivery-and-budget.md` §2.3 | Halved-request simulation when DR-04 is chosen; failure → scenario re-selected |
| A6 - Cost totals equal quantity × unit cost per line (F-09 = sum of supported costs across the four layers) | E4 | `03-registers.md` §2 F-09; `04-delivery-and-budget.md` §2.1 | Reconciliation pass when figures arrive |
| A7 - Post-grant operating costs are modelable once units are priced | E4 | `03-registers.md` §1 DR-10 (undecided) | Executive owner supplies the operating-cost model (`08-first-year-operating-plan.md` §2 Q4); failure → durability row stays a marker |

## 5. Request-amount rule (the request is never invented)

The request amount is **never invented**: DR-04 records it when chosen (`03-registers.md` §1 DR-04: "Request = supported costs from the 4-layer cost model; proportionality test (halve request → state lost outputs)"). Until that record exists, the request cell is `[INFORMATION NEEDED: budget owner; request amount - DR-04]` (data dictionary F-09: "Must equal supported costs"). The request never starts at the maximum: `04-delivery-and-budget.md` §2.3 - "do not start from the award maximum and reverse-engineer activities"; indirect costs are included within the award limit, not added on top. Selecting the scenario and recording the amount is a **successor change** that edits `03-registers.md` - this change does not choose it.

## 6. Decision gate - when the unit-cost model becomes draftable

The unit-cost model **cannot be drafted while DR-04 is unselected** (recorded unselected as of 2026-10-14, `03-registers.md` §1; consequence of delay: the request amount stays unsupported and the rubric's proportionality criterion fails). This document is the framework the concrete budget attaches to.

**Gate:** (1) DR-04 selected in `03-registers.md` with scenario, request amount, and the proportionality loss list (budget owner, delivery-map W-11); (2) cost sources supplied for every line category (`08-first-year-operating-plan.md` §2 Q2); (3) for the maximum scenario only, confirmed capacity (none as of 2026-10-14, C23).

**Once the gate opens:** a follow-on plan (successor to this plan, still T09 content) replaces every marker and `[INFORMATION NEEDED]` cell in Sections 1-3 with verified figures, under the DR-04 record; the assumptions A2/A5/A6/A7 are re-run against the figures; this file is re-verified with the full editing-test set (instructions.md §7).

**Until then:** no draftable budget exists; this framework stands on its own - the deletion test passes (the framework does not depend on the FTSArcade name) and the substitution test passes (all non-marker cells are structural rules that hold under substitution; no invented SF facts).

## 7. Revision record (per methodology)

| Date | Proposed change | Class | Reason | Evidence affected | Budget affected | Decision | Updated documents |
|---|---|---|---|---|---|---|---|
| 2026-10-14 | Unit-cost model and funding-scenario framework created (framework-only: unit definitions UC-01-UC-12 plus the indirect-cost allocation rule, every Figure cell `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation; cost-driver table with 7 drivers and all sensitivity cells as markers; funding-scenario table with the three scenarios (constrained/proposed/maximum) in the request level \| covered outputs \| lost outputs \| basis format, every cell structural or a marker, proportionality rule stated - halving the request removes the stated lost outputs; assumptions table A1-A7 graded E1-E5 with sources and tests; request-amount rule (never invented; DR-04 records it when chosen; request = supported costs; never start at the maximum); decision-gate note (unit-cost model draftable only after DR-04 chosen, cost sources supplied, and - for maximum - capacity confirmed); DR-04/DR-10 states propagated) | Clarifying | Plan 001 T09 (CONTENT) requires the unit-cost model; DR-04 unselected and no cost figures exist as of 2026-10-14, so the change records the framework - no invented unit costs, volumes, or totals | DR-04/DR-10 decision states propagated (E1, source: `03-registers.md` §1; ungraded - unselected/undecided); E1 platform claims (C01-C05, C27) carried; no new figures | None - zero dollar figures; every figure cell carries `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation | No decision closed; unit-cost model stays not draftable until DR-04 chosen | 09-unit-cost-model.md (new), Logs/changes.md, Plan/000-index.md |
```

### 2.3 INFORMATION NEEDED markers list (must appear in the file)

The UC-01…UC-10 table below is the consolidated unknowns list; the complete inline marker texts appear in the file exactly as written in §2.2. Count: **30 inline `[INFORMATION NEEDED: ...]` markers** (1 in the preamble cross-links line, 2 in the Section 1 reading note and unit-cost rule line, 12 in the Section 1 unit table - UC-01-UC-10 and UC-12 Figure cells plus the indirect-cost allocation cell - 7 in the Section 2 driver table, 5 in the Section 3 scenario table, 1 in Section 5, 2 in the Section 7 revision record), each with owner + why + decision-blocked fields per instructions.md §5, each grouped into exactly one of the UC rows below. (The two generic format descriptions in the Status line - "`[INFORMATION NEEDED: <owner>; cost source]`" and "`[INFORMATION NEEDED: ...]`" - are format quotes, not markers; `grep -c` on the file reads **32** hits including them - V9 accounts for this.)

| ID | Owner | Decision blocked | Unblocks | Markers covered |
|---|---|---|---|---|
| UC-01 | Budget owner | DR-04 | Section 1 (Figure cells UC-01-UC-10, UC-12, indirect-cost allocation: 12 cells) | 12 |
| UC-02 | Budget owner | DR-04 | Section 1 (unit-cost rule quotes: reading note + rule line: 2) | 2 |
| UC-03 | Budget owner | DR-04 | Section 2 (sensitivity estimates for 6 drivers: enrollment, session/cohort, maintenance, staffing, sites, evaluation scope) | 6 |
| UC-04 | Executive owner | DR-10 | Section 2 (adoption-timing sensitivity; post-grant operating-cost model) | 1 |
| UC-05 | Budget owner | DR-04 | Section 3 (lost-output enumerations for the constrained and proposed scenarios: 2) | 2 |
| UC-06 | Budget owner + program lead | DR-04 | Section 3 (proposed-scenario delivery-capacity statement) | 1 |
| UC-07 | Program lead | DR-01/DR-04 | Section 3 (maximum scenario: responsible-execution assessment + confirmed capacity: 2) | 2 |
| UC-08 | Budget owner | DR-04 | Section 5 (request amount; F-09) | 1 |
| UC-09 | Program lead | DR-01 | Preamble (named persons per role, owner test) | 1 |
| UC-10 | Budget owner | DR-04 | Section 7 (revision-record budget-affected quotes: 2) | 2 |

---

## 3. F3 - `Documentation/Logs/changes.md`

**Append one row after the plan-011 row (currently line 19), same column format (8 columns; pipes inside cells escaped as `\|` where table formats are named):**

```
| 2026-10-14 | Clarifying | Create unit-cost model and funding-scenario framework (`Prospectus/09-unit-cost-model.md`, new): framework-only - unit definitions table (unit \| definition \| output ref \| cost line in 04 \| figure; rows UC-01-UC-12 plus the indirect-cost allocation rule - every Figure cell `[INFORMATION NEEDED: budget owner; cost source - DR-04]` or an explicit zero-cost explanation; FY-11 gate resolution is zero-cost); cost-driver table (driver \| effect \| sensitivity marker - 7 drivers carried from 04 §2.4/08 §5, all sensitivity cells markers); funding-scenario framework table (request level \| covered outputs \| lost outputs \| basis - constrained/proposed/maximum per 04 §2.3 and the DR-04 row, every cell structural or a marker, proportionality rule stated: halving the request removes the stated lost outputs); assumptions table (assumption \| grade E1-E5 \| source \| test - 7 rows A1-A7); request-amount rule (never invented; DR-04 records it when chosen; request = supported costs; never start at the maximum); decision-gate note (unit-cost model draftable only after DR-04 selected, cost sources supplied, and - for maximum - capacity confirmed); DR-04/DR-10 states propagated | Plan 001 T09 (CONTENT) requires the unit-cost model; DR-04 unselected and no cost figures exist as of 2026-10-14, so the change records the framework - no invented unit costs, volumes, or totals | **INFORMATION NEEDED marker count: 30 (32 `grep -c` hits incl. 2 generic format descriptions in the Status line)** - executor-verified; DR-04/DR-10 decision states propagated (E1, source: 03-registers.md §1; ungraded - unselected/undecided); E1 platform claims (C01-C05, C27) carried; no new figures; no budget affected | No decision closed - unit-cost model stays not draftable until DR-04 chosen | Prospectus/09-unit-cost-model.md (new), Logs/changes.md, Plan/000-index.md | 012 |
```

---

## 4. F4 - `Documentation/Plan/000-index.md`

**Append one row after the plan-011 row (currently line 19):**

```
| 012 | `Documentation/Plan/012-unit-cost-model.md` | Unit-cost model and funding-scenario framework: unit definitions, cost drivers, three scenarios with covered/lost, graded assumptions (plan 001 T09) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 5. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T09: proportionality test; every "scalable" claim has a unit cost; numbers trace to budget lines in 04 - plus the honesty checks below. Per instructions.md §11.6, the orchestrator starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T09; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No invented figures | Read `Documentation/Prospectus/09-unit-cost-model.md` against §2.2 of this plan; `grep -n '\$' Documentation/Prospectus/09-unit-cost-model.md` | The file matches §2.2 verbatim: 0 `$` hits (zero dollar figures); every Figure cell is the `[INFORMATION NEEDED: budget owner; cost source - DR-04]` marker or an explicit zero-cost explanation; 0 numeric unit costs, volumes, or totals |
| V2 | Unit definitions cover every output | Parse the Section 1 unit table | 13 rows (UC-01-UC-12 + the indirect-cost allocation row); every FY-01-FY-11 output ref from `08-first-year-operating-plan.md` §1 appears in the Output ref column (FY-01-FY-10 → UC-01-UC-10, FY-11 → UC-11) and the Q3 staffing output appears (UC-12); UC-11 carries the explicit zero-cost explanation; every Figure cell is the marker or a zero-cost explanation; the indirect-cost row quotes the 29% cap as a line rule, not an amount |
| V3 | Three scenarios with covered/lost structure | Inspect the Section 3 table | Exactly 3 scenario rows (constrained / proposed / maximum) with the request level \| covered outputs \| lost outputs \| basis columns; constrained = essential pilot and evidence-building only; proposed = scale justified by delivery capacity; maximum = scale requiring additional CONFIRMED capacity; every non-structural cell is a marker; "lost outputs" cells are present in all three rows (constrained: the scale set; proposed: the constrained-drop set; maximum: the not-yet-responsible set) |
| V4 | Proportionality rule stated | `grep -niE 'halv|proportionality' Documentation/Prospectus/09-unit-cost-model.md` | The rule appears (Section 3 proportionality paragraph and Section 5): "halving the request removes exactly the stated lost outputs"; ≥ 2 hits |
| V5 | Assumptions graded | Inspect the Section 4 table | 7 rows A1-A7; every row has a grade E1-E5 (A1/A3/A4 = E1; A2/A5/A6/A7 = E4) and a test; no ungraded assumption; no E5 assumption present |
| V6 | No scalable without a unit cost / no prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/09-unit-cost-model.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits in the three executed files ("scalable" must not appear - the framework contains no unit-cost figures, so no scalable claim can exist; "sustainable" must not appear - "post-grant" is used); grep "unique" likewise - 0 hits (the plan file and instructions.md §6's own list are exempt by construction) |
| V7 | Numbers trace to budget lines in 04 | For every unit row and scenario cell, check the Cost line / Basis column against `04-delivery-and-budget.md` §2.2 line categories and §2.3 scenario definitions | Every cost line is a verbatim §2.2 line category name (Technology development, accessibility, security, maintenance; Independent evaluation and data collection; Participant support or compensation (where appropriate); Community delivery and local partner costs; Legal, safeguarding, insurance, financial administration; Program staff and management; Indirect costs); every scenario basis matches the §2.3 wording or is a marker |
| V8 | Tables render | For every table in the new file (Sections 1, 2, 3, 4, 7): header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each; the `\|` escapes inside the §7 revision-record cell render as a literal pipe without breaking the row |
| V9 | INFORMATION NEEDED markers complete | `grep -c "\[INFORMATION NEEDED:" Documentation/Prospectus/09-unit-cost-model.md` + inspect each marker | Count **32** (30 markers + 2 generic format descriptions in the Status line, which are not markers); every marker has the format `[INFORMATION NEEDED: <owner>; <why>; ... <decision blocked>]` with a named role owner and a blocked decision; the §2.3 table contains exactly rows UC-01…UC-10 and every inline marker maps to one of them (sum of the Markers covered column = 30). **Record the verified count in the changes.md row.** |
| V10 | Decision states propagated | `grep -nE 'DR-04|DR-10|unselected as of 2026-10-14' Documentation/Prospectus/09-unit-cost-model.md` | The wording "unselected as of 2026-10-14" appears for DR-04 (03 §1); DR-10 markers present; no decision is closed anywhere in the file; the DR-04 selection is explicitly deferred to a successor change (Section 5) |
| V11 | No drafting boundary | `grep -niE 'dear|subject:|sincerely' Documentation/Prospectus/09-unit-cost-model.md` | 0 hits (protocol R1; no email or promotional text introduced) |
| V12 | changes.md row | Inspect `Documentation/Logs/changes.md` | One new row: class **Clarifying**, plan ref 012, date 2026-10-14, documents updated listing the new file + `Logs/changes.md` + `Plan/000-index.md`; appended after the plan-011 row; existing rows unchanged |
| V13 | Index self-consistency | `grep -c '| 012 |' Documentation/Plan/000-index.md` | Output **1**; the row's status is `planned` (orchestrator flips it through the lifecycle after review); existing rows 001-011 unchanged |
| V14 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | Exactly 1 new file (`Documentation/Prospectus/09-unit-cost-model.md`) + exactly 2 modified files (`Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md`); `Documentation/Plan/012-unit-cost-model.md` appears as the pre-plan artifact (untracked); no other file touched; no deletions |

---

## 6. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| DR-04 / DR-10 decision states and data-dictionary rows F-04/F-07/F-09, verbatim | `Documentation/Prospectus/03-registers.md` §1 (DR-04, DR-10 rows) and §2 (F-04, F-07, F-09) | Preamble and Sections 3, 4, 5 carry the states and definitions; quote-fidelity rule (stop if drifted, do not patch blind) |
| Budget workbook wording (§2.1 layers, §2.2 line categories, §2.3 scenarios + proportionality rules, §2.4 formula, §3.1 year-1 boundary) | `Documentation/Prospectus/04-delivery-and-budget.md` | Sections 1-3 quote line-category names and scenario definitions verbatim; V7 traces every cost line to §2.2 |
| Year-1 outputs FY-01-FY-11 and quarter outputs Q1-Q4 | `Documentation/Prospectus/08-first-year-operating-plan.md` §1-§2 | Section 1 unit table maps output refs (FY-01-FY-10 → UC-01-UC-10, FY-11 → UC-11, Q3 staffing → UC-12); V2 |
| C23 (no SF delivery capacity or confirmed partner as of 2026-10-14) | `Documentation/Prospectus/02-claim-ledger.md` | Section 3 maximum-scenario basis and Section 6 gate condition |
| Marker syntax, evidence grades, proportionality test, change-class definitions | `Documentation/Logs/instructions.md` §5, §7.7, §9.2 | `[INFORMATION NEEDED: <owner>; why; decision blocked]` format; E1-E5 grades; class Clarifying |
| Current row positions in F3/F4 | `Documentation/Logs/changes.md` (plan-011 row at line 19), `Documentation/Plan/000-index.md` (plan-011 row at line 19) | Append after the plan-011 rows; re-check at execution |

**Explicitly out of scope for the executor:** choosing or recommending any DR-04 scenario or request amount (any such action violates this plan; the selection is a successor change that records the decision in `03-registers.md`); inventing any unit cost, volume, or total; editing `03-registers.md`, `08-first-year-operating-plan.md`, `04-delivery-and-budget.md`, `02-claim-ledger.md`, `01-source-case.md`, `00-prospectus.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, root `README.md`, `Documentation/Research/*`, or `Documentation/Refinement/*` (their records already exist and are referenced, not duplicated); drafting any email or promotional copy (protocol R1); committing (orchestrator-only, rule R2).

---

## 7. Revision note (plan amendments)

| Date | Amendment | Class | Reason |
|---|---|---|---|
| (none at plan time) | - | - | - |