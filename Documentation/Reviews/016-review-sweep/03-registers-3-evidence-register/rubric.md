# Rubric Review - `03-registers.md` §3 (Evidence register)

**Change:** 016 (review sweep) · **Sweep batch:** 1 · **Unit:** 03-registers-3-evidence-register
**Reviewer:** rubric (subagent; never commits) · **Date:** 2026-10-15 · **Round:** 1
**Method:** §3 reviewed in reading order (heading, fields line, status line, 7 table rows) against the constitution (instructions.md §5 grades E1-E5), the claim ledger (`02-claim-ledger.md`, C01..C28), and change 010 (E5 relocation). Note: the file predates the review model (S0, 2026-10-14); defects are recorded as found.

## Scope

Section 3 = lines 104-117 of `Documentation/Prospectus/03-registers.md`: the "Evidence register (template + pre-filled rows)" heading, fields line, status line, and the 7-row claim table (C01-C04, C06, C19, C20, C12-C18, C21-C22, C07/C08/C23/C24).

## Score table

| Dimension | Score (1-5) | Defect |
|---|---|---|
| 1. Clarity | 4 | Each present row is readable and self-consistent (claim set · evidence · source · population · finding · limitation · grade · test plan). Minor: bundled rows (C01-C04, C12-C18, C07/C08/C23/C24) require the ledger to resolve individual IDs; "Export" appears as a source without the full reference path used in the ledger; the C07/C08/C23/C24 row's dual-grade cell "E1 (absence) / E5 (positive claim)" is compact but understandable. |
| 2. Consistency | 3 | Present causal rows (C19, C20) are E4 with concrete test plans; E5 records C21-C22 carry a "Removed" row consistent with change 010. But C28 - which the ledger and changes.md row 010 identify as the third causal E4 claim **with a test** - has no register row, so the register's claim-to-test mapping is incomplete; C24 (relocated to "Removed claims (E5)" by change 010) still sits inside the E1-absence row C07/C08/C23/C24 (dual grade mitigates, but the row's primary reading is E1); status line "only E1 rows are complete; E4 rows need test plans" sits at odds with C19/C20 rows that already carry test plans. |
| 3. Enforceability | 3 | Every present row carries grade, source, and limitation, and no ungraded causal verb appears anywhere in §3 (finding cells state absence/assertion/prohibition, not causation). But the register cannot enforce discipline on claims that have no row: C05, C09-C11, C25-C28 have no grade/source/limitation/test here (they are graded only in the ledger), so the register fails as an enforcement instrument for ~29% of the ledger's claims. |
| 4. Completeness | 2 | 8 of 28 ledger claim IDs have no register entry and no explicit exclusion in §3: **C05** (E1 documented absence), **C09, C10, C11** (E4 operational), **C25, C26, C27** (E1 factual, added by change 010), **C28** (E4 causal with test). The C25-C28 gap is acknowledged in the ledger's "Evidence-register linkage" as a follow-up ("added when that file is next touched") that never ran; C05 and C09-C11 are excluded nowhere. |

**Verdict: FAIL.**

Highest-priority defect: **completeness** - the evidence register omits 8 of the 28 ledger claim IDs (C05, C09, C10, C11, C25, C26, C27, C28) with no row and no explicit exclusion, including C28, one of the three causal E4 claims declared to carry test plans (ledger linkage; changes.md row 010), and the three E1 competition/workbench facts C25-C27 added by change 010. The register therefore cannot serve its stated function - making every packet claim traceable to a source, grade, limitation, and next verification step - for a material share of the claim set. Rows for C25-C28 must be added (or the register must record the exclusion and its owner), and C05/C09-C11 must either gain rows or be explicitly excluded.

## Findings table

| # | Paragraph / row | Finding | Rule violated | Severity |
|---|---|---|---|---|
| 1 | Status line "only E1 rows are complete; E4 rows need test plans owned by the evidence reviewer once the program is defined" | Incomplete coverage claim: C19/C20 rows already list test plans, and C12-C18's test names the claim owners, not the evidence reviewer; the sentence understates what the register already carries. Also silent on the 8 claims with no row. | instructions.md §5 (certainty labeling); §11.5 Q3 (certainty correctly labeled) | Low |
| 2 | Row C07/C08/C23/C24 ("E1 (absence) / E5 (positive claim)") | C24 was relocated to "Removed claims (E5)" (not a claim, excluded from count) by change 010, but appears inside an E1-anchored row; a reader's primary reading is that C24 is E1. Dual-grade cell prevents a hard contradiction. | change 010 E5 relocation; §5 grade consistency | Low |
| 3 | Rows C19/C20 | Consistent as written: causal claims, E4, with concrete test plans (pilot + pre-registered measures; charity-law review + written controls). No defect. | - | - |
| 4 | Row C21-C22 | Consistent with change 010: E5, "Removed; reintroduce only via DR-05 with real evidence". No defect. | - | - |
| 5 | Entire table | No row for **C28** (Causal E4, "options recorded, not chosen... will test whether the chosen option's intended outcome follows", test = pre-registered indicator per DR-07 rule). The ledger linkage names C28 among "the causal claims graded E4 with tests"; the register's E4 rows are supposed to carry those tests. | ledger "Evidence-register linkage"; changes.md row 010 ("C19/C20/C28 are the causal E4 claims with tests"); §5 (E4 must include a test) | High |
| 6 | Entire table | No row for **C25, C26, C27** (E1 factual: foreign-entity eligibility/fiscal sponsorship; finalist stage + $500k project-development grant; workbench WIP counts + label conflict C3) - material competition and platform facts added by change 010. Ledger linkage defers them ("added when that file is next touched"); 03-registers.md was not touched after change 010, so the follow-up never ran. | ledger "Evidence-register linkage" (unfulfilled); §5 (every material claim graded + sourced) | High |
| 7 | Entire table | No row for **C09, C10, C11** (E4 operational: eligible lead org, beneficiary definition, intervention/pathway) and no explicit exclusion of them anywhere in §3. The C12-C18 row covers only C12-C18, so three E4 operational claims are outside the register. | §5 (every material claim graded + sourced); §11.4 evidence pass rule | Medium |
| 8 | Entire table | No row for **C05** (E1 factual documented absence: site makes no claims about beneficiaries/partners/outcomes) - a gap statement the Evidence section relies on; the C07/C08/C23/C24 absence row covers packet-source absences, not the site-content absence. No exclusion recorded. | §5; ledger coverage | Medium |
| 9 | Source cells ("Export §...", "Export roster section", "Export inference boundaries") | "Export" abbreviates the reference file path the ledger spells out (`../Reference/we're looking to prepare a grant application for h.md`); understandable in packet context but not a retrievable path on its own. | §5 source discipline (plan 016 F2 family) | Low |
| 10 | Row C12-C18 | Test plan "Owners to supply documentation or downgrade to E5" is the weakest test in the register (documentation-or-remove, no method or date), but is a legitimate E4-adjacent treatment; no defect beyond the general E4-test ownership ambiguity in finding 1. | - | - |

## Paragraph acceptance (instructions.md §11.5)

| Paragraph | Q1 claim first | Q2 traceable | Q3 certainty labeled | Q4 one new idea | Q5 deletion loses info | Result |
|---|---|---|---|---|---|---|
| Fields + status line | Yes | Yes | No (finding 1) | Yes | Yes | Fail (Q3) |
| Row C01-C04 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C06 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C19 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C20 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C12-C18 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C21-C22 | Yes | Yes | Yes | Yes | Yes | Pass |
| Row C07/C08/C23/C24 | Yes | Yes | Partial (dual grade; C24 reading) | Yes | Yes | Pass |

## What would raise each score

- **Clarity → 5:** expand "Export" to the reference path; split the C07/C08/C23/C24 row or annotate C24's E5 relocation; add a row-index note that bundles resolve in the ledger.
- **Consistency → 5:** add C28 row with its test plan (DR-07 pre-registered-indicator rule); reconcile the status line with the C19/C20/C12-C18 test plans already present; align C24's row placement with its E5 record status.
- **Enforceability → 5:** every claim row present with grade/source/limitation/test, and a named owner per test plan (status line already defers E4 test ownership to the evidence reviewer once the program is defined).
- **Completeness → 5:** add rows C05, C09-C11, C25-C28 (or record explicit exclusions with owners); the revision change should also remove the ledger's stale "added when that file is next touched" deferral once the rows land.

**Verdict: FAIL** - round 1. Highest-priority defect: completeness (8 of 28 ledger claims - C05, C09, C10, C11, C25, C26, C27, C28 - have no evidence-register row and no explicit exclusion, including causal-E4 C28 with a declared test plan). Revision path: pre-plan designs the register row additions per §11.4; the register is re-reviewed after execution.