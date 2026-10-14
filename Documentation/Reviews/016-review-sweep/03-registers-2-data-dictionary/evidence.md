# Evidence Review - 03-registers.md §2 (Data dictionary)

- **Reviewer role:** Evidence reviewer
- **Review run:** 016-review-sweep · **Unit:** 03-registers-2-data-dictionary
- **Round:** 1 · **Date:** 2026-10-15
- **Scope:** Section 2 (Data dictionary), `Documentation/Prospectus/03-registers.md` lines 84-101 (table F-01..F-11 + rule line)
- **Constitution:** `Documentation/Logs/instructions.md` §5-§6, §11.2 (evidence facet), §11.4 (pass rules)
- **Sources checked:** `08-first-year-operating-plan.md`, `09-unit-cost-model.md` (figure citations); packet-wide `F-\d+` scan (all Prospectus files) for cross-file figure references
- **Context:** unit predates the review model (S0 state); every finding below is a pre-existing state defect, recorded per the record-every-defect instruction

## Check table

| Check | Result | Detail | Location |
|:--|:--|:--|:--|
| 1. Six columns (Definition, Population, Period, Source, Calculation, Limitation) filled or marked on every figure row | PASS | All 11 rows (F-01..F-11) carry all six cells. F-09 marks Population and Period with "-" (not applicable - explicit mark, not a blank); F-11 marks Source as "TBD local source"; F-01 marks Population "population TBD - DR-01". No empty cell anywhere. | §2 table, lines 90-100 |
| 2. One definition per figure; no interchangeable terms without dictionary note | FAIL | The rule line (line 86) prohibits users/participants/young people/beneficiaries interchange unless declared identical, and F-01's limitation correctly separates participants from website users (F-02). But the dictionary's own measurement spine uses population terms outside the rule's scope that are never defined or declared identical: F-03's calculation "Completers ÷ starters" introduces **"starters" with no definition and no identity statement to its own Population cell ("Enrolled cohort")**; F-05's Population is disjunctive ("Completers or enrolled cohort") with no applicability rule; F-01 Definition ("People completing enrollment") vs Calculation ("accepted participants") are not declared identical ("accepted" ≠ "enrolled"). See findings D1-D4. | §2 rule line 86; F-01, F-03, F-05 rows |
| 3. Figures cited by 08/09 exist in the dictionary | PASS | `09-unit-cost-model.md` cites F-04 (lines 11, 70), F-07 (lines 68), F-09 (lines 70, 75) - all present, and quoted definitions match the dictionary verbatim ("Eligible costs ÷ completers"; "29% of direct project/activity costs"; "Sum of supported costs, 4 layers"). `08-first-year-operating-plan.md` cites **no** F-IDs (its F-* references are objectives FY-01..FY-11). The set named in the sweep brief (F-01, F-03, F-05, F-08, F-11) is cited by `06-participant-pathway.md`, `10-narrative.md`, and `01-source-case.md`, not by 08/09; all exist (F-01..F-11 complete, 11/11). Packet-wide scan: no cited F-ID is missing from the dictionary. | 09 lines 6, 11, 68, 70, 75; 08 (no F-IDs); dictionary rows F-01..F-11 |
| 4. No prohibited words (§6) | PASS | Scan of section 2 for revolutionary / world-class / unique / cutting-edge / empower / unlock / transform / scalable / sustainable / "partners include" / "data shows": zero hits. | §2 lines 84-101 |
| 5. Tables render | PASS | Header 8 columns, separator 8 groups, all 11 data rows exactly 8 cells (no stray pipes, no broken rows). Nested `[INFORMATION NEEDED]` markers inside cells (F-02 source, F-09 limitation, F-11 limitation) render as inline text. | §2 table lines 88-100 |

## Findings (all defects recorded)

| # | Paragraph / element | Finding | Rule violated | Severity |
|:--|:--|:--|:--|:--|
| D1 | F-03 row (line 92) | Calculation "Completers ÷ starters" uses **"starters"**, which is defined nowhere in the dictionary and never declared identical to the row's own Population ("Enrolled cohort"). The formula is not executable from the dictionary alone. | §2 rule: one definition per figure; no interchangeable terms without identity statement (line 86) | Moderate |
| D2 | F-05 row (line 94) | Population "Completers or enrolled cohort" is disjunctive - two alternative populations with no rule for when each applies, contradicting the one-definition-per-figure rule. | §2 rule (line 86) | Minor |
| D3 | F-01 row (line 90) | Definition "People completing enrollment" vs Calculation "Count of accepted participants" - "accepted" and "enrolled" are not declared identical, so the reach count's population is ambiguous within the row. | §2 rule (line 86) | Minor |
| D4 | Rule line (line 86) | The interchangeability prohibition names only 4 terms (users/participants/young people/beneficiaries); the population terms the dictionary's own calculations actually chain (starters, completers, enrolled cohort, accepted participants) fall outside the rule's scope, leaving the F-01→F-03→F-04→F-05 measurement spine on undeclared population identity. | §2 rule (line 86) - incomplete coverage | Minor |
| D5 | F-09 row (line 98) | Population and Period marked "-" - acceptable as explicit not-applicable marks; recorded for completeness, not a defect. | none | Info |
| D6 | F-08 row (line 97) | Limitation self-declares that "benefiting" must be defined per activity - the limitation cell is doing its job; the pending definition is a recorded open item, not a silent gap. | none | Info |

## Verdict

**FAIL** - highest-priority defect: **D1** - F-03's calculation "Completers ÷ starters" uses the undefined term "starters", never equated to its own population "Enrolled cohort"; the dictionary's one-definition rule (line 86) is therefore not satisfied within the dictionary's own rows, and the reach→completion→unit-cost→outcome measurement spine (F-01/F-03/F-04/F-05) rests on undeclared population identity. Per §11.4, a single FAIL sends the section back to revision; the unit passes only when D1-D3 are resolved (define "starters" or replace it, resolve the F-05 disjunction, declare F-01's definition/calculation terms identical) and the rule line's term coverage is extended (D4).

- Checks passed: 1, 3, 4, 5 (all figure rows complete; all cited figures exist and quoted definitions match; no prohibited words; tables render).
- Cross-file verification: packet-wide `F-\d+` scan found no figure cited anywhere that is absent from the dictionary (11/11 present); 09's three citations (F-04, F-07, F-09) match the dictionary verbatim.
- No E5 claims, no silent inference, and no failed editing test were found in the unit; the defects are dictionary-internal definitional gaps, not source-contradiction defects.