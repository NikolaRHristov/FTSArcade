# Evidence Review - Change 011 (First-Year Operating Plan Framework)

**Reviewer facet:** Evidence · **Date:** 2026-10-14 · **Verdict:** **PASS**

**Scope reviewed:** `Documentation/Prospectus/08-first-year-operating-plan.md` (new), `Documentation/Logs/changes.md` (row 011), `Documentation/Plan/000-index.md` (row 011), against design authority `Documentation/Plan/011-first-year-plan.md` (amended) and sources `02-claim-ledger.md`, `03-registers.md`, `04-delivery-and-budget.md`, `05-durability-risks-rights.md`.

## Check table

| # | Check | Result | Detail | Location |
|---|---|---|---|---|
| 1 | File byte-identical to the amended plan fence | **PASS** | sha256 of plan §2.2 fence (lines 41-165 + trailing newline) = sha256 of the new file = `7742a6023ae7bbff4611dd4033947720dadba3b8e11e2d683ff274c6c3c1bcc9`; identical line-by-line (125 lines) | Plan §2.2 ↔ `Prospectus/08-first-year-operating-plan.md` |
| 2 | Zero invented content | **PASS** | 0 dollar figures (`$` count = 0; `$[0-9]` = 0) in all three executed files; 0 named persons; orgs named only where recorded (Community Initiatives, Intersection for the Arts - `03-registers.md` §1 DR-02 candidates; SF Arts Commission, Cultural Districts Program, OEWD, Rec & Park - §1.1 DR-01 next action, evidence sources not partners); no invented locations, commitments, or partners beyond the fence; the only dollar-adjacent rule quoted is the indirect-cost cap named as a line rule (≤29% of direct costs, E1 rules §7), no amount | File preamble/Sections 1-6; `04-delivery-and-budget.md` §2.2 |
| 3 | Cost lines use recorded §2.2 category names | **PASS** | Every named cost line is verbatim one of the 6 recorded categories: Community delivery and local partner costs; Participant support or compensation (where appropriate); Program staff and management; Technology development, accessibility, security, maintenance; Independent evaluation and data collection; Legal, safeguarding, insurance, financial administration. Two rows name "All lines" (Q2/Q4 cost-source rows) - shorthand for the full §2.2 category set per the L1-L4 build order (§2.1), each carrying the DR-04 marker | Sections 1 and 2 cost lines ↔ `04-delivery-and-budget.md` §2.2 |
| 4 | Budget test under amended rule (13 quarter rows) | **PASS** | 13/13 rows pass: 9 rows named category + `[INFORMATION NEEDED: budget owner; cost source - DR-04]`; 2 rows explicit zero-cost explanation (`None (decision; zero cost)` - Q1 decision-gate check, Q4 year-1 review); 2 rows pure `[INFORMATION NEEDED]` cells (Q1 named-capacity inventory - DR-01; Q4 survivor-plan-update - DR-10), valid under the amended V2 rule; 0 empty cost lines; 0 dollar figures | Section 2 quarter table |
| 5 | Durability survivors = 3 named retained assets with owner + continuity condition | **PASS** | Exactly 3 retained-asset survivors named: (1) Live platform: 15 playable cabinets, free browser access, no account gate - owner Technical owner (+ payer marker DR-10), continuity: hosting/domain continuity, rights schedule (DR-09), post-grant payer; (2) Workbench: 9 WIP builds honestly labeled - owner Technical owner, continuity: completion is a funded decision, not an automatic survivor; (3) Accessibility settings - owner Technical owner, continuity: built-in, no maintenance cost documented. Adopted activities / funded operations / retained-access rule / continuity-if-exit are markers, never defaults; no-default-continuation rule quoted from §3.3 | Section 4 survivor table ↔ `04-delivery-and-budget.md` §3.3, `05-durability-risks-rights.md` §1 |
| 6 | 38 markers (39 grep hits), each with owner + blocked decision | **PASS** | `grep -c '[INFORMATION NEEDED:'` = 39; 38 real markers + 1 format description (Status-line phrase "`[INFORMATION NEEDED: ...]`", not a marker), exactly as plan §2.3/V5 predicts. Every marker has a role owner + a blocked DR ref (17 unique texts; the sole exception is the format description). Per-section counts match §2.3: preamble cross-links 1, Section 1 table 7, Section 2 13 (11 Q rows + reading note + expansion rule), Section 3 10 (7 staffing + 3 partners), Section 4 5, Section 5 1, Section 7 1 = 38 | Whole file; plan §2.3 |
| 7 | Undecided states propagated; DR-04 unselected; DR-08/09/10 markers present | **PASS** | "undecided as of 2026-10-14" appears for DR-01/06/07 jointly (2×: Section 1 reading note, Section 6); DR-04 "unselected" 4× (preamble, Section 2 reading note, Financial risk, revision record); DR-08 6 hits, DR-09 6 hits, DR-10 10 hits; "No decision closed" present (revision record Decision cell); no decision is closed anywhere | Preamble, Sections 1/5/6/7 ↔ `03-registers.md` §1.1/§1 |
| 8 | No prohibited words | **PASS** | 0 hits for revolutionary, world-class, unique, cutting-edge, empower, unlock, transform, scalable, sustainable, "partners include", "data shows" in all three executed files (new file, changes.md, 000-index.md) | V7 scan on 3 files |
| 9 | Tables render | **PASS** | All 7 tables (Sections 1, 2, 3.1, 3.2, 4, 5, 7): header, separator, and body rows have equal unescaped-pipe counts (8/5/6/5/6/5/9); the `\|` escapes in the §7 revision-record cell render as literal pipes without breaking the row | Sections 1-7 |
| 10 | changes.md row 011 and 000-index row 011 | **PASS** | changes.md: one new row appended after the plan-010 row - class **Clarifying**, plan ref **011**, date 2026-10-14, documents updated list new file + Logs/changes.md + Plan/000-index.md, marker count recorded: "**INFORMATION NEEDED marker count: 38 (39 `grep -c` hits incl. the Status-line format description)** - executor-verified" (matches my count); existing rows unchanged. 000-index.md: row 011 present, content verbatim per plan §4, status `planned`; `grep -c '| 011 |'` = 1 | `Logs/changes.md` line 20; `Plan/000-index.md` line 26 |
| 11 | Git status: exactly 2 modified + 2 untracked (plan + new file) | **PASS** | `git status --porcelain`: M `Logs/changes.md`, M `Plan/000-index.md`; ?? `Plan/011-first-year-plan.md`, ?? `Prospectus/08-first-year-operating-plan.md` (+ this review dir); no other files touched, no deletions | Repo root |

## Supporting detail

**Budget test rows (Section 2, 13 rows):**

| Q | Cost-line cell | Pass class |
|---|---|---|
| Q1 Platform continuity | Technology development, accessibility, security, maintenance + DR-04 marker | Named category |
| Q1 Evidence-register rows | Independent evaluation and data collection + DR-04 marker | Named category |
| Q1 Named-capacity inventory | `[INFORMATION NEEDED: program lead; named capacity - DR-01]` | Pure marker (amended rule) |
| Q1 Decision-gate check | None (decision; zero cost) | Zero-cost explanation |
| Q2 Cost sources (L1-L4) | All lines + DR-04 marker | Named categories (all §2.2) |
| Q2 Platform maintenance | Technology development, accessibility, security, maintenance + DR-04 marker | Named category |
| Q2 If gate closed | Community delivery and local partner costs; participant support or compensation (where appropriate) + DR-04 marker | Named categories |
| Q3 Staffing plan | Program staff and management + DR-04 marker | Named category |
| Q3 Partner statuses | Community delivery and local partner costs + DR-04 marker | Named category |
| Q3 Evaluation instrument | Independent evaluation and data collection + DR-04 marker | Named category |
| Q4 Year-1 review | None (decision; zero cost) | Zero-cost explanation |
| Q4 Unit-cost model inputs | All lines + DR-04 marker | Named categories (all §2.2) |
| Q4 Survivor plan updated | `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]` | Pure marker (amended rule) |

**Marker count reconciliation (plan §2.3 enumeration):** preamble cross-links 1 · Section 1 7 · Section 2 13 · Section 3.1 7 · Section 3.2 3 · Section 4 5 · Section 5 1 · Section 7 1 = **38**; + 1 Status-line format description = **39 grep hits**. Verified programmatically.

**Source-fidelity spot checks (all PASS):** risk register Section 5 matches `05-durability-risks-rights.md` §2 for all 8 rows (7 categories + eligibility: trigger → action → owner → status); post-grant owner markers match 05 §1 (`executive owner; operating-cost model - DR-10`, `program lead; free-access rules - DR-06`, `rights owner; license continuity - DR-09`); claim refs match `02-claim-ledger.md` (C01-C05/C27 E1 platform facts; C06 peer-review 4-6 × ~2.5 h Nov-Dec 2026; C09/C10/C11/C15/C19/C20/C23/C28 E4 rows; E5 records C21/C22/C24); year-1 boundary quote "capacity that named people and partners can deliver" verbatim from 04 §3.1; C23 absence quote verbatim.

## Verdict

**PASS** - all 11 checks pass; no defect blocks the change. The threefold review's evidence facet finds the file byte-identical to the amended plan fence, zero invented content, all budget-test rows valid under the amended rule, correct survivor/marker/decision-state propagation, clean tables, recorded marker count in changes.md, and the exact expected git file set.

**Non-blocking observation:** plan §4 instructed the 000-index row be appended directly after the plan-010 row (line 18); the executor appended it at end-of-file (line 26, after the Status Lifecycle section). Row content is verbatim-correct and status `planned` (V12 count = 1), but it renders outside the Index table. Cosmetic only; no evidence impact. Recommend the orchestrator note the placement when flipping the row status.