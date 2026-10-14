# Evidence review - 03-registers.md section 1 (Decision register incl. §1.1 Recorded decisions)

**Review run:** 016-review-sweep · **Unit:** 03-registers-1-decision-register
**Reviewer:** Evidence reviewer (subagent) · **Date:** 2026-10-15 · **Round:** 1
**Scope:** `Documentation/Prospectus/03-registers.md` section 1 (lines 8-81): §1 Decision register (rows DR-01…DR-10) and §1.1 Recorded decisions (rows DR-11, DR-01, DR-06, DR-07 + option-detail blocks).
**Sources checked:** `Documentation/Research/facts-pack.md` (facts #9/#10/#25, conflicts C1/C2, §(e) sources), `Documentation/Prospectus/02-claim-ledger.md`, `Documentation/Logs/instructions.md` (§5-§7), `Documentation/Logs/changes.md` (changes 004-007), `Documentation/Refinement/00-alignment-matrix.md`, `Documentation/Prospectus/01-source-case.md`, `Documentation/Prospectus/00-prospectus.md`, Reference export `Documentation/Reference/we're looking to prepare a grant application for h.md`.

---

## Check table

| # | Check | Result | Detail | Location |
|---|---|---|---|---|
| 1 | Every DR row has all 7 content columns (decision, options, rule, needed info, owner, deadline, consequence) filled or marked | PASS | §1 table: header + 10 rows (DR-01…DR-10), every row 8 cells (Ref + 7 content columns), all cells populated; base-case options explicitly marked "none approved - **all recorded, not chosen** (see §1.1)" (DR-01 e, DR-06 c, DR-07 g). §1.1 table: 4 rows (DR-11, DR-01, DR-06, DR-07), every row 8 cells (Ref, Decision, Decided value, Deciding owner, Date, Evidence grade, Gate effect, Next action), all populated | 03-registers.md lines 10-21; 27-32 |
| 2 | Recorded decisions DR-11/DR-01/DR-06/DR-07 use correct states (unknown/undecided as of 2026-10-14, ungraded, no invented outcomes) and match changes 004-007 | PASS | DR-11: "Unknown as of 2026-10-14", gate **Blocked**, E1 gate facts + "status itself is ungraded", next action = 3-part email to boundless-sf@submittable.com - matches change 004. DR-01/DR-06/DR-07: "Undecided as of 2026-10-14", gate **Open** (scope not locked), "E1 (…); the undecided status itself is ungraded - no positive claim, mirroring DR-11)" - match changes 005/006/007. All rows state "No positive claim is made…"; options recorded as "options, not chosen"; no invented outcomes; all dated 2026-10-14 | 03-registers.md lines 29-32; changes.md rows 13-16 |
| 3 | Owner test: named owners or INFORMATION NEEDED markers | PASS | §1 owners are roles only (Program lead, Authorized officer, Budget owner, Evidence reviewer, Program lead + counsel, Rights owner, Executive owner); no bare personal names. §1.1 deciding owners are roles, each carrying `[INFORMATION NEEDED: named person(s); <required action>; blocks <decisions> - DR-xx]`. Every next-action cell names its owner (instructions.md §7.3 owner test satisfied) | 03-registers.md lines 12-21 (owner col.), 29-32 (deciding-owner col., next-action col.) |
| 4 | Uncertainty language where status is unknown | PASS | Verbatim phrases per instructions.md §5: "Unknown as of 2026-10-14", "Undecided as of 2026-10-14", "As of 2026-10-14, the facts pack (`Documentation/Research/facts-pack.md`, facts #9, #10, #25) shows…" (DR-11); all option-detail rows graded "E4, untested"; E1/E4 grades on every recorded entry; no unknown silently resolved | 03-registers.md lines 29-32; 34-80 |
| 5 | No prohibited words (instructions.md §6) | PASS | Zero hits for revolutionary / world-class / unique / cutting-edge / empower / unlock / transform / scalable / sustainable / "partners include" / "data shows" in section 1 and in the whole file (regex scan, case-insensitive) | 03-registers.md whole file |
| 6 | Tables render (equal pipe counts per row) | PASS | §1 register table: 9 pipes / 8 cells on all 11 rows (header + 10 DR rows). §1.1 table: 9 pipes / 8 cells on all 5 rows. Option-detail tables: 5 pipes / 4 cells on all rows (7 + 5 + 9). §2/§3 tables uniform. No non-uniform row in any table | 03-registers.md lines 10-21, 27-32, 36-42, 52-56, 66-74 |
| 7 | Cross-links resolve (`../Refinement/00-alignment-matrix.md` form) | FAIL | All referenced files exist and cited content verified - with 2 Low-severity reference defects (F1, F2 below). See findings table | F1: line 30; F2: line 32 |

---

## Findings

| Paragraph/row | Finding | Rule violated | Severity |
|---|---|---|---|
| DR-01 §1.1 row, Next action (line 30) | Cites "the decision rule in §2.1" - no §2.1 exists in 03-registers.md (sections: 1, 1.1, 2, 3, 4) nor in any companion document; the DR-01 decision rule is stated in this file's own §1.1 option-detail block (line 44). Dangling/unresolvable section reference; the rule text quoted in the cell is correct, only the pointer is wrong | instructions.md §11.2 evidence facet: cross-references must resolve; §7 editing tests (traceability) | Low |
| DR-07 §1.1 row, Decided value (line 32) | Cites "`00-prospectus.md` §7 (Measurement) carry `[INFORMATION NEEDED: decision owner / evaluation lead; … DR-06/DR-07]` markers" - the actual §7 marker (00-prospectus.md line 176) is `[INFORMATION NEEDED: evaluation lead; required once beneficiary and outcome are chosen; blocks Section 7 - DR-05]`: the owner word matches ("evaluation lead") but the blocked-decision suffix is DR-05, not DR-06/DR-07. The §1 (line 24) and §4.3 (line 110) markers do carry "decision owner … DR-06/DR-07", so the composite citation is partly imprecise | instructions.md §11.2 evidence facet: claims about sources must be accurate | Low |

**Observations (informational, not defects):**
- Export citations use "§1" / §"heading"" style for an unnumbered-heading document; each quoted phrase ("Choose one primary purpose", "Choose a charitable frame", "it's both", "Run a mock review", "Commercial-benefit test", "Separate the businesses", "Define the public benefit", "Build around the rubric", "Measurement design") was verified verbatim in the export (lines 54/60/79/721/1439/2403/2428/2460/2482).
- 02-claim-ledger.md rows C25-C28 have no rows in 03-registers.md §3 evidence register; documented as a follow-up in the ledger ("Evidence-register linkage"). Outside this unit's scope (section 1 only).

---

## Verdict: **PASS**

Highest-priority defect: **F1 - Low** - DR-01 §1.1 next action cites "the decision rule in §2.1", a section that does not exist (03-registers.md has no §2.1; the rule lives in the §1.1 option-detail block). Both findings are Low-severity reference-precision issues: no factual claim, decision state, evidence grade, owner, or table rendering is wrong, and the substance of every cited cross-file claim was verified in source. Section 1 meets the evidence-facet pass rules of instructions.md §11.4 (every material claim carries a grade and source; no E5 claims; figures match the data dictionary; no prohibited words; no failed editing test).

**Evidence basis (key verifications):** facts-pack #9 (registration closed Sep 11 2026 5:00 p.m. PT, "Only registrants can submit"), #10 (application deadline Oct 15), #25 (boundless-sf@submittable.com), C1/C2 (deadline widget; foreign-entity FAQ/Rules contradiction) - all quoted accurately in DR-11; alignment matrix Table A criterion 1 names "SF Arts Commission, Cultural Districts, OEWD, Rec & Park - … not partners" (DR-01 next action resolves) and Table B has the charitable-use row (DR-06 resolves); 01-source-case.md rows 1/3-5/10 and ten-statement #7 carry the cited markers/states; 00-prospectus.md §1/§2/§4.2/§4.3/§7/§8 markers verified (F2 excepted); changes.md 004-007 match the recorded entries row-for-row.