# Rubric review - `03-registers.md` §2 Data dictionary

- **Reviewer:** rubric reviewer (sweep batch 1, change 016)
- **Date:** 2026-10-15 · **Round:** 1
- **Scope:** `Documentation/Prospectus/03-registers.md` §2 (lines 84-100): rule line + dictionary table F-01..F-11
- **Constitution:** `Documentation/Logs/instructions.md` - §5 (uncertainty/`[INFORMATION NEEDED: owner; why; decision blocked]` format), §11 (review model), data-dictionary rule (one definition per figure; figures carry definition, population, period, source, calculation, limitation). NOTE: this file predates the review model; defects are recorded honestly as pre-existing.

## Score table

| Dimension | Score (1-5) | Defect |
|---|---|---|
| 1. Clarity | 4 | Most rows are crisp, self-contained one-liners - a reader can extract meaning, population, period, source, formula, and limitation without hopping documents. Defects: **F-06** definition is a numeric inventory that does not reconcile - "24 cabinets listed; 15 live; 8 WIP" (15+8=23≠24) - and silently uses the "8 ON THE BENCH" label count rather than the entry list; **F-10** calculation cell carries rule values ("4 required, up to 6 if necessary, ~2.5 h") rather than a calculation; **F-05** definition is terse ("Pre-specified result"). |
| 2. Consistency | 4 | All uses match the dictionary: Reach = enrollments, never website users (06 §1/§4, DR-07 (d)); Website use distinct (06 §1); Completion = completers ÷ starters with acceptable-absence precondition (06 steps 4/§4, IN-06/IN-08); Unit cost per completer (09 reading note); Outcome pre-registered (06 step 5, DR-07); 29% indirect cap (09 A4, 04 rules line); ≤25% compliance (06 §1, DR-01 rule); request = supported costs (DR-04, 09 A6); peer-review load 4/up to 6/~2.5 h (DR-08); F-11 estimate with source + method (DR-01, 06 §1, 08 OY-02, 10 NF-04). One material defect: **F-06 contradicts the ledger's own resolution** - C27 (E1) holds cabinet counts must be stated from the entry list (9 WIP entries) and flags "8 ON THE BENCH" as internally inconsistent (conflict C3), yet F-06 repeats the label-based 24/15/8 numbers, unreconciled, with no conflict reference. |
| 3. Enforceability | 4 | Structurally fully enforceable: all 11 rows fill or mark all six required columns; zero blank cells; unknowns carried as markers, never silently resolved. Minor: three markers (**F-02, F-09, F-11**) deviate from the §5 canonical form `[INFORMATION NEEDED: <owner>; why; decision blocked]` - owner and why present, blocked-decision/DR reference omitted; **F-09** marks population/period "-" where "Award budget"/"Award period" would match F-07/F-08. |
| 4. Completeness | 5 | All 11 dictionary rows are referenced elsewhere in the packet (F-01/02/03/05/08: 06 pathway; F-04/07/09: 09 cost model + DR-04; F-06: claim ledger C02/C27 + 10-narrative FR-06 example; F-10: DR-08; F-11: DR-01, 06 §1, 08 OY-02, 10 NF-04, 01 source-case). Conversely, every figure used across the packet is F-01..F-11 - no used-but-undefined figure exists (UC-01..UC-12 are cost-model units anchored to F-04; C06/C26 dollar amounts are competition rules, not project figures; run 014 verification independently confirmed zero invented figures). |

## Findings

| Row | Finding | Rule violated | Severity |
|---|---|---|---|
| F-06 | "24 cabinets listed; 15 live; 8 WIP" - 15+8=23≠24; repeats the label count ("8 ON THE BENCH") that C27 (E1, conflict C3) proves inconsistent with the 9 WIP entry-list entries; no conflict reference in the row; the row's own calculation cell ("count of cabinet entries") contradicts its definition cell's label-based numbers | "One definition per figure" (03 §2 header); numerical consistency (refinement checklist item 13); figures-vs-dictionary cross-check (instructions §11.2) | Medium |
| F-10 | Calculation cell holds rule values (4 required, up to 6, ~2.5 h), not a calculation; matches DR-08 verbatim but is mislabeled as a calculation | 6-column figure format (calculation column) | Low |
| F-02 / F-09 / F-11 | Markers carry owner + why but omit the blocked-decision element of the canonical form | instructions.md §5 `[INFORMATION NEEDED: <owner>; why; decision blocked]` | Low |
| F-09 | Population/period cells "-" instead of naming the award scope; acceptable as marked, inconsistent with F-07/F-08 "Award period" | 6-column format (marked, not blank) | Low |
| F-05 | Definition "Pre-specified result" is terse; comprehensible only with the pre-registered-method context (DR-07 decision rule) | None - clarity note, not a rule violation | Info |

## What would raise each score

| Dimension | Rises to 5 when |
|---|---|
| Clarity | F-06 restated from the entry list with reconciled counts; F-10 calculation cell replaced by a formula or relabeled as rule values; F-05 definition expanded |
| Consistency | F-06 aligned to C27 (entry-list counts, conflict C3 referenced) |
| Enforceability | All markers carry the full §5 owner/why/blocked-decision format; F-09 dashes replaced by award-scope values |
| Completeness | - (at ceiling; no further content needed) |

## Verdict

**PASS** - all four dimensions ≥ 3 (4, 4, 4, 5).

**Highest-priority defect:** F-06 cabinet-count conflict - the dictionary's definition repeats the unreconciled label-based inventory (24/15/8; 15+8=23) that the claim ledger itself flags as conflict C3, and C27's resolution (counts from the entry list = 9 WIP) has not been propagated into the dictionary. The defect is pre-existing and already flagged elsewhere in the packet (C02/C27), so it does not block this round's pass; F-06 should be reconciled with C27 at the next edit of this file.