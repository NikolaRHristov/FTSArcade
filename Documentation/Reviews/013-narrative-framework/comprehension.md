# Comprehension Review - Change 013 (Narrative Framework)

**Reviewer role:** Comprehension · **Target:** `Documentation/Prospectus/10-narrative.md` (new, 2026-10-14, S0)
**Method:** file read once, answered from memory · **Verdict: PASS**

## Restatement

Change 013 creates `Documentation/Prospectus/10-narrative.md` as a framework-only (S0) document for the prospectus narrative: an eight-section skeleton with verbatim headings, ten binding drafting rules (FR-01..FR-10), a per-section source-mapping table with page budgets, eleven hold markers (NF-01..NF-11), and a decision gate. All narrative prose is blocked until the scope-lock gate closes (DR-01/DR-06/DR-07 decided in `03-registers.md` §1.1), with Section 7 additionally requiring DR-04 and Section 8 additionally DR-10/DR-09. The file deliberately contains zero prose sentences, zero invented claims, and zero dollar figures; a successor plan (still T10) replaces the hold markers with prose under FR-02-FR-06 once the gate opens.

## Answers to the adapted six questions

| # | Question | Answer |
|---|---|---|
| 1 | What is this artifact? | A framework-only (S0) document, not the narrative itself: section skeleton, binding rules, source map, hold markers, decision gate. It is the T10 deliverable of plan 001 (bucket CONTENT, LAST), written before the narrative can be drafted. |
| 2 | What problem does it address? | The narrative cannot be drafted: DR-01/DR-06/DR-07 are undecided, DR-04 unselected, DR-11 registration blocked. Rather than invent a beneficiary, intervention, or outcome, the change records the structure the prose attaches to once decisions close - a gap-report-style hold instead of fabricated content. |
| 3 | What are the key binding commitments? | FR-01 prose block while gate open; FR-02 fixed paragraph method (claim → fact/mechanism → SF relevance → evidence/limitation → next step, plus five acceptance questions); FR-03 drafting formula with every clause supported or assigned; FR-04 verbatim uncertainty phrases, confidence never moves up, phrases mandatory below E3; FR-05 evidence grades E1-E5 (E5 removed, not rewritten); FR-06 mandatory trace line per substantive paragraph; FR-07 zero hits for the prohibited-words blacklist; FR-08 editing tests incl. deletion/substitution at T10; FR-09 decision summary written last from accepted claims only; FR-10 each section independently understandable with page budgets. |
| 4 | What grounds the framework? | Seven evidence artifacts (`01-source-case`, `06-participant-pathway`, `07-platform-boundary`, `02-claim-ledger`, `08-first-year-operating-plan`, `09-unit-cost-model`, `05-durability-risks-rights`), decision states in `03-registers.md` (DR-01-DR-11), `Logs/instructions.md` §5-§8 (evidence/uncertainty language, prohibited words, editing tests, build order), `Refinement/02-refinement-checklist.md` §(a) stop conditions, and the Reference export (paragraph method, drafting formula, prospectus architecture, page budgets). |
| 5 | What are its boundaries? | Zero prose sentences, zero dollar figures, zero invented claims; SF-specific wording limited to the verbatim architecture heading, rule text, and markers. Section 8's page budget is carried in other sections' budgets. The DR-11 registration gate does not block drafting, but a blocked registration outcome converts the deliverable to a gap report. |
| 6 | What would change the artifact? | The gate opening: DR-01/DR-06/DR-07 closed with written rationale in the register (packet reaches Draftable D1); then a successor plan replaces every marker with prose under FR-02/FR-03/FR-04/FR-06 and re-runs FR-08. Section 7 additionally requires DR-04 selected (deadline "Before narrative drafting"); Section 8 additionally DR-10/DR-09. |

## Acceptance check - prose-block rule (FR-01)

| # | Question | Result | Note |
|---|---|---|---|
| 1 | Does the rule explicitly forbid drafting prose while the gate is open? | ✅ Yes | FR-01: "No prose sentence is drafted in this file, and none may be added by any successor content while the gate… is open." |
| 2 | Does the file actually contain zero prose sentences? | ✅ Yes | Content limited to framework headings, rules FR-01..FR-10, tables, placeholders, markers NF-01..NF-11, revision record; no narrative prose sentences present. |
| 3 | Is the unblock condition precisely defined? | ✅ Yes | Scope-lock gate: DR-01/DR-06/DR-07 closed with written rationale in `03-registers.md` §1.1 (Draftable D1); Section 7 adds DR-04; Section 8 adds DR-10/DR-09. |
| 4 | Does the block bind successors, not just this file? | ✅ Yes | Explicitly "none may be added by any successor content"; unblock requires a successor plan. |
| 5 | Is the path from blocked → drafted specified? | ✅ Yes | On gate close, successor replaces hold markers with prose under FR-02-FR-06, then runs FR-08 (full §7 editing-test set + T10 verification). |

## Acceptance check - source-mapping table

| # | Question | Result | Note |
|---|---|---|---|
| 1 | Does the table cover all eight sections with the verbatim headings? | ✅ Yes | 8 rows; headings match the skeleton exactly (Decision summary … Durability and governance). |
| 2 | Does every row identify its source artifact(s)? | ✅ Yes | Each row names artifact file(s) with section ranges, e.g. row 3: `06-participant-pathway.md` §1-§4, `07-platform-boundary.md` §1-§3. |
| 3 | Does every row carry a page budget? | ✅ Yes | 1 / 2 / 2 / 3 / 2 / 1 / 2+workbook / carried-in-other-budgets (the carry is itself explicit). |
| 4 | Does every row carry a hold marker? | ✅ Yes | NF-03 (row 1) through NF-10 (row 8), all present and consolidated in the hold-marker section. |
| 5 | Does the table map to all six T10 outline feeds? | ✅ Yes | Feeds column covers problem (01), intervention (06/07), evidence (02), plan (08), budget (09), durability (05). |

## Acceptance check - decision-summary hold (Section 1 / FR-09)

| # | Question | Result | Note |
|---|---|---|---|
| 1 | Is Section 1 explicitly written last? | ✅ Yes | FR-09 binds it; quote from `00-prospectus.md` drafting note: "the summary should be written last, using only claims already accepted in the other sections." |
| 2 | Does it draw only on claims accepted elsewhere? | ✅ Yes | "using only claims already accepted in Sections 2-8"; source-map row 1: "Sections 2-8, accepted claims only." |
| 3 | Is a placeholder/marker in place instead of prose? | ✅ Yes | Framework placeholder (prose blocked - NF-03); no summary prose drafted. |
| 4 | Does it stay held until other sections are drafted and verified? | ✅ Yes | "Prose attaches only after every other section is drafted and verified; until then this section carries its hold marker." |
| 5 | Is the content spec for what attaches recorded? | ✅ Yes | Source-map row 1 spec (beneficiary, intervention, change sought, request, result) and NF-03 (beneficiary, intervention, single public outcome, request amount, result - DR-01/DR-06/DR-07/DR-04). |

## Verdict

**PASS.**

- Restatement: faithful - captures artifact type (framework, not prose), the eight-section skeleton, FR-01..FR-10, source map, NF-01..NF-11, the decision gate, and the zero-prose constraint.
- Six answers: all present and grounded in the file's content.
- Acceptance units: prose-block rule, source-mapping table, and decision-summary hold each pass all five questions - no unit fails any question, hence no unit fails more than one.