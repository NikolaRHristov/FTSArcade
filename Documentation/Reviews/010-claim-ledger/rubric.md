# Rubric review - change 010 (claim ledger build-out)

**Reviewer facet:** Rubric (threefold review)
**Artifact reviewed:** `Documentation/Prospectus/02-claim-ledger.md` (25 live claims, 11 columns, E5 records relocated)
**Design authority:** `Documentation/Plan/010-claim-ledger.md` (file matches it on every checked edit)
**Constitution:** `Documentation/Logs/instructions.md` (§5 evidence grades, §6 prohibited words, §7 editing tests, §11 review model)
**Date:** 2026-10-14
**Verdict: PASS**

## Score table

| Dimension | Score (1-5) | What would raise it one point | Defect |
|---|---|---|---|
| Clarity | 4 | Reconcile C02's claim text (and its permitted wording) with the entry-list count - 9 WIP entries, per C27's rule - so a reader need not hop C3 → C27 to reconcile "15 live + 8 labeled = 23" with the "24 cabinets" opener. | Minor (pre-existing, now flagged): C02's sentence asserts "lists 24 cabinets; 15 are live playable and 8 are labeled work-in-progress" - arithmetically 23 of 24, the label-vs-list tension of conflict C3. The design flags it (Conflict ref C3 on C02; detail in C27, which states counts must come from the entry list), and the tension predates 010 (identical wording in plan §0.1; also in data dictionary F-06), so it is a designed, cross-referenced preservation, not a regression. Every other claim reads unambiguously; the 11-column structure is uniform and the header rules paragraph explains count semantics. |
| Consistency | 5 | - (at ceiling) | None material. All 21 preserved rows (C01-C20, C23) keep verbatim cell text with exactly the three planned cells inserted after Evidence status (plan §1.3 table); C25-C27 trace to facts-pack (#15/#16/#18/#19; #4 + timeline table; §(d) facts 4/6/7/8) and C28 to `03-registers.md` §1.1 option detail (DR-01 a-d, DR-06 a, DR-07 a-f; capability/progression/system levels; engagement-not-outcome rule); grades match evidence - E1 for facts (incl. the documented-absence rows C05/C07/C08/C23, consistent with registers §3's "E1 (absence)" row) and E4 for every option/assertion row; no 07-boundary §5 non-claim appears as a claim (C28's "community connection" is a register option label; "engagement metrics are never outcomes" is the DR-07 rule); conflicts C1-C6 are all cross-referenced in the Conflict ref column per plan §0.3 (C1+C4 on C06; C2 on C25; C3 on C02+C27; C5 on C26; C6 on C23). |
| Enforceability | 5 | - (at ceiling) | None. All 25 rows carry an E1-E5 Evidence status, a non-empty Source URL cell, an owner role, and a permitted-wording cell; 0 ungraded causal verbs (C18 Forward E4; C19/C20/C28 Causal E4 - V4-equivalent check returns nothing); 0 prohibited words used as claims (the sole V7 hit is the pre-existing C18 "sustainable" meta-quotation, flagged benign); 0 drafting text (no dear/subject/sincerely); `[INFORMATION NEEDED: ...]` markers follow instructions.md §5 format and the header restates the named-person rule. |
| Completeness | 5 | - (at ceiling) | None material. 25 live claim rows in [15,25] (top of band: `grep -c '^| C[0-9][0-9] '` = 25; single pipe-table, 27 lines × 12 pipes = 11 columns, contiguous); E5 records C21/C22/C24 relocated verbatim to "Removed claims (E5)" and explicitly excluded from the count; header count sentence, 11-column unification, Removed-claims section, quick list, and Evidence-register linkage match plan §1.1-§1.6; changes.md row 010 and 000-index row 010 match plan §2-§3; git status shows exactly the planned file set. The two flagged deviations are benign: plan V3's awk reads $7 (Source status, off-by-one from the leading empty field) instead of $8 (Conflict ref) - the file itself cross-references all six conflicts correctly; V7's grep catches the pre-existing "sustainable" meta-quotation in C18's permitted wording ("Not: 'the project will be sustainable through commerce.'"), which quotes the prohibited phrase rather than using it. |

## Verification evidence (checked against sources)

| Check | Source | Result |
|---|---|---|
| Claim count in [15,25] | plan V1 | `grep -c '^| C[0-9][0-9] '` = 25; 27 pipe lines, all 12 pipes (11 columns), one pipe-table, rows C01-C20, C23, C25-C28 contiguous |
| Every claim graded + sourced | plan V2 | 0 NO-GRADE / NO-SOURCE lines (25/25 rows have E1-E5 Evidence status and non-empty Source URL) |
| Conflicts cross-referenced | plan V3 (corrected column) | All six present in Conflict ref: C1+C4 on C06; C2 on C25; C3 on C02+C27; C5 on C26; C6 on C23 |
| Plan V3 as written | plan V3 (literal) | Reports C1/C4 missing - awk reads $7 (Source status) because the leading pipe makes Conflict ref $8. Flagged deviation; the file is correct under the intended column |
| No ungraded causal verbs | plan V4 | 0 UNGRADED (C18 Forward E4; C19/C20/C28 Causal E4; C12-C17 Operational, all graded) |
| No prohibited words used | plan V7 | 1 line hit: C18 permitted wording (pre-existing "sustainable" meta-quotation inside "Not: ..."; flagged benign). All other words 0 |
| No drafting boundary | plan V8 / R1 | 0 hits (dear / subject: / sincerely) |
| No non-claim leak | plan V5 / 07-boundary §5 | 0 hits in C25-C28 for the §5 non-claim terms |
| Preserved rows verbatim | plan §0.1 vs live file | C01-C20, C23 cells identical to the pre-change rows; three cells inserted per plan §1.3 (spot-checked C01, C03, C05, C06, C07, C08, C10, C19, C20, C23) |
| New rows trace to sources | facts-pack #4/#15/#16/#18/#19, §(d) facts 4/6/7/8, timeline, registers §1.1 | C25 matches facts 15/16/18/19 + C2; C26 matches fact 4 + timeline ("by June 2027", "up to $500,000", "$1-3.5M pool", prospectus Aug 2027) + C5; C27 matches facts 4/6/7/8 + C3; C28 matches DR-01/06/07 option detail and the DR-07 decision rule |
| E5 relocation verbatim | plan §0.1 rows C21/C22/C24 vs §1.4 bullets | C21/C22 verbatim; C24 verbatim plus one trailing period (cosmetic) |
| Header / quick list / linkage | plan §1.1/§1.4/§1.6 | Count sentence "25 (within the 15-25 band)" with E5-exclusion note; Removed-claims section before the unchanged quick list; linkage updated (C19/C20/C28 causal E4 with tests; C25-C28 register rows recorded as follow-up) |
| changes.md / 000-index.md | plan §2/§3; git status | Row 010 present in both files matching the planned text; `git status --porcelain` = exactly 3 modified + untracked plan file, no deletions |

## Verdict

**PASS** - all four dimensions ≥ 3 (Clarity 4, Consistency 5, Enforceability 5, Completeness 5). The ledger is an enforceable, fully sourced claim control: 25 live claims at the top of the [15,25] band, E5 records preserved as prohibition records outside the count, every claim graded/owned/sourced with permitted wording, no non-claim promoted, and all six conflicts cross-referenced. The two flagged deviations (plan V3 column typo; pre-existing C18 "sustainable" meta-quotation) are confirmed benign - the file is correct where the plan's check is off-by-one, and the word hit is a quoted prohibition, not a usage. Highest-priority (non-blocking) follow-up: when C02 is next touched, state the WIP count from the entry list (9) per C27's rule so the row's arithmetic (15 + 9 = 24) matches its "24 cabinets" opener without requiring the C3 hop.