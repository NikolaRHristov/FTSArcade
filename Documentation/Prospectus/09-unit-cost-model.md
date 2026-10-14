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
