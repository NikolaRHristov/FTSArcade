# Rubric review - `03-registers.md` §1 Decision register + §1.1 Recorded decisions

- **Reviewer:** rubric reviewer (sweep batch 1, change 016)
- **Date:** 2026-10-15 · **Round:** 1
- **Scope:** `Documentation/Prospectus/03-registers.md` §1 + §1.1 (lines 8-80): register table DR-01..DR-10, recorded-decision table (DR-11, DR-01, DR-06, DR-07), and the DR-01/DR-06/DR-07 option-detail blocks
- **Constitution:** `Documentation/Logs/instructions.md` - §5 (evidence grades, `[INFORMATION NEEDED: <owner>; why; decision blocked]`), §11 (review model, artifact format)
- **Evidence checked:** `Documentation/Research/facts-pack.md` (facts #9, #10, #17, #19, #21-23, #25; conflicts C2/C3), `Documentation/Prospectus/02-claim-ledger.md` (C07, C10, C17-C20, C24, C25, C28), `Documentation/Prospectus/04-delivery-and-budget.md` (W-01, §2.3 scenarios). NOTE: this file predates the review model; defects are recorded honestly as pre-existing.

## Score table

| Dimension | Score (1-5) | Defect |
|---|---|---|
| 1. Clarity | 4 | Every DR row is structurally self-contained (decision, lettered options, decision rule, needed information, owner, deadline, consequence), and the option-detail blocks for DR-01/06/07 are exemplary adversarial tables. Defects: **DR-01 §1.1 next action cites "the decision rule in §2.1", which does not exist in this file** (headings are §1, §1.1, §2, §3, §4; the rule lives in the DR-01 option-detail block); **DR-08's "Options" cell contains a required assignment** ("Named person to complete 4 (up to 6) peer reviews…"), not a set of alternatives; the DR-01/06/07 decided-value cells are paragraph-length single-cell prose that mixes state, evidence rationale, and option lists (scannable, but heavy). |
| 2. Consistency | 4 | All recorded decision states match the facts pack and claim ledger, verified per row: **DR-11** Unknown/Blocked matches facts #9/#10/#25 and ledger C07/C25 (E1 documented absence); **DR-01/06/07** Undecided/Open match ledger C10/C19/C20/C28 and F-11; **DR-04** unselected matches 04-delivery-and-budget §2.3 (no scenario chosen; all amounts `[INFORMATION NEEDED]`) and ledger C17/C18 ("under consideration"/"being investigated"); DR-02 foreign-entity flag matches facts #18/#19 + conflict C2; DR-03/DR-11 go/no-go chain matches W-01; DR-05 matches C21 (E5 removal); DR-08 matches facts #22/#23; DR-09 matches C24; DR-10 matches C18. Evidence grades (E1) on all four §1.1 entries match the ledger's E1 usage. Defects: **DR-04's unselected state is not recorded in the register itself** - its row carries no "none approved / not chosen" marker (DR-01/06/07 all carry one) and it has no §1.1 entry, so the state is only inferable from another file; the §2.1 dangling reference above is also a cross-reference inconsistency. |
| 3. Enforceability | 4 | Structurally enforceable: all 10 open rows fill all eight columns; every row names the decision, options, rule, needed information, a role owner (named persons correctly deferred as `[INFORMATION NEEDED]`), a deadline (DR-03 "Oct 14-15 (immediate go/no-go)" is the sharpest), and a consequence of delay; all four §1.1 entries carry owner, date, evidence grade, gate effect, and a concrete next action, and their owner markers follow the §5 canonical form (e.g. DR-11: "named person; … blocks the gate - DR-03"). Defects: **DR-08 has no real options to decide** (the options cell is a spec, so the decision-rule cell governs assignment rather than choice); **DR-04 has no expressible "recorded, not chosen" state** because its options list lacks a base case, making its enforcement asymmetric with DR-01/06/07; DR-01/06/07 deadlines are conditional ("before scope lock (not achieved)") rather than dated - acceptable since the trigger is explicit, but weaker than dated deadlines. |
| 4. Completeness | 3 | All 11 refs are present: DR-01..DR-10 in the register table (header "10 open decisions" is accurate - DR-11 is a recorded entry, not an open row), DR-11 in §1.1; recorded-decision blocks exist for DR-11 (Unknown/Blocked), DR-01/06/07 (Undecided, with full option-detail blocks and decision-rule/needed-evidence/owner/deadline/consequence sections). One material gap: **DR-04 has no recorded-decision block and no "not chosen" marker** - §1.1's own convention ("entries are appended as decisions are made or decision states are recorded") plus the DR-01/06/07 precedent mean the funding-scenario state (unselected as of 2026-10-14) should be recorded, and it is not; DR-02/03/05/08/09/10 correctly have no entries (genuinely open, carried by row-level markers). |

## Findings

| Row | Finding | Rule violated | Severity |
|---|---|---|---|
| DR-04 | Funding-scenario state is unrecorded: the row lists options (a)-(c) with no "none approved / not chosen" base case (DR-01/06/07 all carry one), and §1.1 has no DR-04 entry; the unselected state is only inferable from `04-delivery-and-budget.md` §2.3 and ledger C17/C18. The register fails its own §1.1 audit-trail convention for a decision whose state is effectively recorded everywhere else. | §1.1 convention ("entries are appended as … decision states are recorded"); state-recording parity with DR-01/06/07 | Medium |
| DR-01 | §1.1 next action: "choose ONE option by the decision rule in §2.1" - no §2.1 exists in this file (headings: §1, §1.1, §2, §3, §4); the DR-01 decision rule is in the "DR-01 option detail" block | Cross-reference integrity (instructions §11.5 Q2: can the claim be traced) | Medium |
| DR-08 | "Options" cell holds a required assignment ("Named person to complete 4 (up to 6) peer reviews (~2.5 h), Nov-Dec 2026, after submission"), not a set of alternatives; the row prescribes rather than offers options | Options-column semantics (row structure) | Low |
| DR-01/06/07 | §1.1 decided-value cells are paragraph-length single-cell prose mixing state, evidence rationale, cross-references, and option lists; a reader must parse long run-ons to extract the four facts (state, grade, gate effect, next action) that the table's columns should carry | None - clarity note, not a rule violation | Info |
| DR-11 | Gate effect "Blocked" alongside DR-03's "Oct 14-15 (immediate go/no-go)" reads as a tension at first glance; it is resolved by the next-action email (exception request to boundless-sf@submittable.com, facts #25) and the W-01 failure response (gap report, not draft). No correction needed. | None - verified consistent | Info |

## What would raise each score

| Dimension | Rises to 5 when |
|---|---|
| Clarity | §2.1 reference corrected to the option-detail block; DR-08 options cell replaced with real alternatives or relabeled; decided-value cells split into scannable sub-fields |
| Consistency | DR-04 row gains the "none approved - recorded, not chosen" marker and/or a §1.1 entry matching its actual (unselected) state |
| Enforceability | DR-04 options gain an expressible base case; DR-08 row restructured so the decision cell contains a genuine choice |
| Completeness | DR-04 recorded-decision block appended (state: unselected as of 2026-10-14; owner: budget owner; gate effect: Open) |

## Verdict

**PASS** - all four dimensions ≥ 3 (4, 4, 4, 3).

**Highest-priority defect:** DR-04's funding-scenario state is unrecorded. Every other open decision's state is either marked in its register row ("all recorded, not chosen" for DR-01/06/07) or recorded in §1.1 (DR-11 unknown/Blocked), but DR-04 carries neither: its options list has no base case and §1.1 has no entry, so "no scenario selected as of 2026-10-14" is only inferable from `04-delivery-and-budget.md` §2.3. The state itself is consistent with the packet (nothing selects a scenario), so this does not block the round's pass; DR-04 should be brought in line with the DR-01/06/07 convention at the next edit of this file (add a "none approved - recorded, not chosen" marker and/or a §1.1 entry).