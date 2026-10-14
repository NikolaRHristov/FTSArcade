# Narrative - FTSArcade / Boundless San Francisco

**Version:** S0 (framework only) · **Date:** 2026-10-14
**Status:** **FRAMEWORK ONLY - NOT DRAFTABLE - NARRATIVE PROSE BLOCKED.** As of 2026-10-14, DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided** (`03-registers.md` §1.1), DR-04 (funding scenario) is **unselected**, and the registration gate (DR-11) is **Blocked**. Per `Logs/instructions.md` §8, the narrative is drafted only after the other artifacts exist and agree; per the stop conditions (`Refinement/02-refinement-checklist.md` §(a)), where no beneficiary or intervention is approved the correct product is a gap report, not more prose. Narrative prose is therefore **BLOCKED until the packet reaches Draftable - DR-01/DR-06/DR-07 closed in the register** (`03-registers.md` §1.1). This document is the narrative's **framework**: the section skeleton, binding drafting rules, per-section source mapping, paragraph-trace formats, and hold markers (NF-01-NF-11) where prose attaches once decisions close. It contains framework headings, rules, tables, and markers only - **no prose sentence, zero invented claims, zero dollar figures**.
**Purpose:** Define the T10 deliverable of plan 001 (bucket CONTENT, LAST) as the framework the narrative prose attaches to once the scope-lock gate closes. The framework fixes: the eight-section skeleton (Decision summary held last; Problem and beneficiaries; Intervention; Change mechanism; San Francisco execution; Evidence and measurement; Financial plan; Durability and governance), the binding drafting rules (paragraph method, drafting formula, uncertainty language, evidence grades, paragraph-trace format, prohibited words, editing tests), the per-section source map, and the prose-block gate. Fed by all seven evidence artifacts; feeds the draftable packet (D1) once DR-01/DR-06/DR-07 close.
**Sources:** `01-source-case.md` (problem), `06-participant-pathway.md` and `07-platform-boundary.md` (intervention), `02-claim-ledger.md` (claims C01-C28; evidence-register linkage; E5 prohibition records C21/C22/C24), `08-first-year-operating-plan.md` (plan), `09-unit-cost-model.md` (budget), `05-durability-risks-rights.md` (durability), `03-registers.md` (decision states DR-01-DR-11; data dictionary F-01-F-11; evidence register §3), `Logs/instructions.md` (§5 evidence and uncertainty language, §6 prohibited words, §7 editing tests, §8 build order), `Refinement/02-refinement-checklist.md` (§(a) stop conditions), Reference export (paragraph method, drafting formula, prospectus architecture, page budgets).
**Cross-links:** every source file above is linked; `00-prospectus.md` §1 holds the placeholder decision summary that the narrative's Section 1 supersedes when drafted; `04-delivery-and-budget.md` §2 is the cost-model spec Section 7 quotes. All owners are roles (per `03-registers.md` rules); named persons are marked (NF-02).

## Framework rules (binding)

**FR-01 - Prose-block rule (binding).** No prose sentence is drafted in this file, and none may be added by any successor content while the gate in the Decision gate section is open. The file contains only: framework headings, binding rules (FR-01-FR-10), the section skeleton and source map, framework placeholders, hold markers (NF-01-NF-11), and the revision record. Narrative prose is BLOCKED until the packet reaches Draftable - DR-01/DR-06/DR-07 closed in `03-registers.md` §1.1 (scope-lock gate; `Logs/instructions.md` §8: "The narrative is drafted only after the other artifacts exist and agree"; stop conditions: where no beneficiary or intervention is approved, "the correct product then is this gap report, not more prose"). When the gate closes, a successor plan (still T10 content) replaces the hold markers with prose under FR-02-FR-06 and re-runs FR-08.

**FR-02 - Paragraph method (binding, Reference export "Use a fixed paragraph method").** Every substantive paragraph, in order: (1) state the claim; (2) give the most relevant fact or mechanism; (3) explain why it matters to San Francisco; (4) identify the evidence, limitation, or implementation condition; (5) connect it to the next action or outcome. Additionally, each paragraph must pass the five acceptance questions (`Logs/instructions.md` §11.5): the first sentence states its claim; the claim can be traced; its certainty is correctly labeled; it adds exactly one new idea; deleting it removes useful information rather than tone. Retain a paragraph only if all five answers are yes.

**FR-03 - Drafting formula (binding, Reference export).** Prose follows the internal drafting formula, with every clause supported or assigned: "For [defined beneficiaries], [named barrier] limits [specific opportunity]. The project will [specific activity], delivered by [responsible party], so that [measurable result] occurs. This is expected to contribute to [broader change] because [evidence or reasoned mechanism]. [Named party] will sustain [specific element] after the grant through [mechanism]." Delete any clause that cannot be supported or assigned to someone.

**FR-04 - Uncertainty-language requirements (binding, `Logs/instructions.md` §5).** Use the phrases verbatim:
- "As of [date], [source] shows…"
- "Comparable evidence suggests…"
- "The project will test whether…"
- "The planning target is…"

**Confidence rule (binding):** a sentence may move down in confidence, never up; an E3 finding cannot be rewritten as proven. **Uncertainty phrases are mandatory wherever evidence is below E3** (T10 verification, plan 001 §2). Unknowns are never silently resolved: a hold marker names its owner, the missing information, and the blocked decision (format per the hold-marker section).

**FR-05 - Evidence grades (binding, `Logs/instructions.md` §5).** Every material claim carries a grade; E5 claims are removed, not rewritten.

| Grade | Meaning | Permitted treatment |
| :-- | :-- | :-- |
| E1 | Direct evidence from this project and population | State as demonstrated, with metric and limitation |
| E2 | Direct evidence from a closely comparable program | State similarity and relevant differences |
| E3 | Relevant analogous evidence | Use to support the mechanism, not identical outcomes |
| E4 | Plausible but untested assumption | Label as an assumption and include a test |
| E5 | Insufficient support | Remove from the prospectus |

**FR-06 - Paragraph-trace format (binding).** Every substantive paragraph carries a trace line: `**Trace:** source: <artifact file> §<section>; claims: <claim IDs from 02-claim-ledger.md>; figures: <F-IDs from 03-registers.md §2>; evidence grade: E<n>; limitation: <stated limitation or marker>.` Example (format only): `**Trace:** source: 08-first-year-operating-plan.md §1; claims: C01-C05, C27; figures: F-06; grade: E1; limitation: site labels change; counts may drift.` The trace satisfies checklist test 9 (traceability - at least 95% of factual sentences map to the claim ledger) and `Logs/instructions.md` §11.5 question 2.

**FR-07 - Prohibited words (binding, `Logs/instructions.md` §6).** The final prose and this framework file carry zero hits for every term in the instructions.md §6 blacklist; the blacklist is not repeated here by name - `Logs/instructions.md` §6 is the authoritative list and the verification grep (plan V5) names the terms. In particular: no scale claim without a unit-cost figure (Section 7 draws figures from `09-unit-cost-model.md`), and no post-grant claim without a named payer (Section 8 follows `08-first-year-operating-plan.md` §4 survivors' plan, which uses "post-grant").

**FR-08 - Editing tests (binding, `Logs/instructions.md` §7; plan 001 §2 T10 verification).** At prose time (successor change), the full §7 test set runs: deletion, substitution, owner, evidence, budget, durability, proportionality, adversarial. The T10 verification (plan 001 §2) is binding: deletion + substitution tests; prohibited-words scan, 0 hits (FR-07); uncertainty phrases used wherever evidence is below E3 (FR-04). This framework passes deletion and substitution by construction: its content is structural rules, source references, and markers, none of which depends on the project name or on an invented SF fact.

**FR-09 - Decision summary written last (binding).** Section 1 is written last, using only claims already accepted in Sections 2-8: "the summary should be written last, using only claims already accepted in the other sections" (`00-prospectus.md` drafting note; Reference export). Until every other section is drafted and verified, Section 1 stays a framework placeholder (NF-03).

**FR-10 - Each section independently understandable (binding, Reference export "Prospectus architecture").** "Each section should enable a reviewer to make one judgment." Sections carry the export's page budgets (source-map table); no section depends on another section's prose to be understood; cross-references name the section.

## Section skeleton and source map

**Reading note:** the eight headings below are the narrative's permanent structure (T10 outline - problem, intervention, evidence, plan, budget, durability - plan 001 §2). The Content that attaches column is the export's spec for what each section must contain once the gate closes - not drafted content. Hold markers NF-03-NF-10 are consolidated in the hold-marker section.

| # | Section heading (verbatim) | Feeds (T10 outline) | Source artifact(s) | Content that attaches once unblocked | Page budget | Hold marker |
|---|---|---|---|---|---|---|
| 1 | Decision summary | - (written last, FR-09) | Sections 2-8, accepted claims only | Beneficiary, intervention, change sought, request, and result (export Prospectus architecture) | 1 page | NF-03 |
| 2 | Problem and beneficiaries | problem (01) | `01-source-case.md` (ten-statement packet, problem rows; SF problem analysis and F-11 reachable-population estimate are markers) | Condition, scale, cause, and consequence (export Need); baseline with source limitation | 2 pages | NF-04 |
| 3 | Intervention | intervention (06/07) | `06-participant-pathway.md` §1-§4; `07-platform-boundary.md` §1-§3 | Who participates, what they receive, how often and for how long, where it happens, who delivers it, what the platform does, success after one year (export "Define the intervention") | 2 pages | NF-05 |
| 4 | Change mechanism | evidence (02) | `02-claim-ledger.md` (claims C01-C28; evidence-register linkage); `03-registers.md` §3 | Why outputs become outcomes and broader change; causal table problem to activity to output to outcome to system change with evidence grades (export "Build the theory of change") | 3 pages (Mechanism and evidence) | NF-06 |
| 5 | San Francisco execution | plan (08) | `08-first-year-operating-plan.md` §1-§5 | Sequence, partners with statuses (confirmed / in discussion / proposed), capacity, SF-establishment sequence (delivery-map W-08); responsibility and dependency table | 2 pages (Delivery) | NF-07 |
| 6 | Evidence and measurement | (02/ledger) | `02-claim-ledger.md` (claims, evidence-register linkage, E5 prohibition records C21/C22/C24); `03-registers.md` §3 (evidence register) and §2 (data dictionary F-01-F-11) | What is known, analogous, assumed, and untested (export Evidence); indicator table with a pre-registered indicator - baseline, target, instrument, collection timing (DR-07 decision rule) | 1 page (Measurement) | NF-08 |
| 7 | Financial plan | budget (09) | `09-unit-cost-model.md` §1-§5; `04-delivery-and-budget.md` §2 | Scenario comparison; why the request is justified; proportionality - halving the request removes the stated lost outputs; request = supported costs (DR-04) | 2 pages plus workbook | NF-09 |
| 8 | Durability and governance | durability (05) | `05-durability-risks-rights.md` §1-§4 | Post-grant owner, funding, access, and maintenance; rights schedule; governance controls (DR-10/DR-09) | Carried in Delivery and Financial plan budgets | NF-10 |

## 1. Decision summary

**Framework placeholder (prose blocked - NF-03).** Held per FR-09: written last, using only claims already accepted in Sections 2-8. Prose attaches only after every other section is drafted and verified; until then this section carries its hold marker (NF-03) and the source-map row 1 spec (beneficiary, intervention, change sought, request, and result).

## 2. Problem and beneficiaries

**Framework placeholder (prose blocked - NF-04).** Source: `01-source-case.md`; the SF problem analysis (city sources) and the reachable-population estimate (F-11) are program-lead inputs recorded in `03-registers.md` §1.1 DR-01. Content attaches per source-map row 2; paragraph trace per FR-06; uncertainty per FR-04 (baseline source and limitation required); hold marker NF-04.

## 3. Intervention

**Framework placeholder (prose blocked - NF-05).** Source: `06-participant-pathway.md` §1-§4 and `07-platform-boundary.md` §1-§3. Content attaches per source-map row 3 (export "Define the intervention" list); paragraph trace per FR-06; uncertainty per FR-04 (partner and provider references carry statuses, never bare names); hold marker NF-05.

## 4. Change mechanism

**Framework placeholder (prose blocked - NF-06).** Source: `02-claim-ledger.md` claims and evidence-register linkage, `03-registers.md` §3. Content attaches per source-map row 4 (causal table with grades; engagement metrics never relabeled as outcomes - DR-07 decision rule; E5 prohibition records honored); paragraph trace per FR-06; uncertainty per FR-04; hold marker NF-06.

## 5. San Francisco execution

**Framework placeholder (prose blocked - NF-07).** Source: `08-first-year-operating-plan.md` §1-§5. Content attaches per source-map row 5 (sequence, partner statuses, named capacity only - `04-delivery-and-budget.md` §3.1 year-1 boundary); paragraph trace per FR-06; uncertainty per FR-04; hold marker NF-07.

## 6. Evidence and measurement

**Framework placeholder (prose blocked - NF-08).** Source: `02-claim-ledger.md` and `03-registers.md` §3 and §2. Content attaches per source-map row 6 (known / analogous / assumed / untested; pre-registered indicator - baseline, target, instrument, collection timing, decision affected); paragraph trace per FR-06; uncertainty per FR-04; hold marker NF-08.

## 7. Financial plan

**Framework placeholder (prose blocked - NF-09).** Source: `09-unit-cost-model.md` §1-§5 and `04-delivery-and-budget.md` §2. Content attaches per source-map row 7 (scenario comparison, proportionality, request = supported costs); DR-04 must be selected before prose attaches (the DR-04 register-row deadline is "Before narrative drafting"); zero dollar figures until the budget owner supplies sourced figures; paragraph trace per FR-06; hold marker NF-09.

## 8. Durability and governance

**Framework placeholder (prose blocked - NF-10).** Source: `05-durability-risks-rights.md` §1-§4. Content attaches per source-map row 8 (post-grant owner, funding, access, maintenance; rights schedule; governance controls); the durability test (`Logs/instructions.md` §7.6) requires named survivors with owners; paragraph trace per FR-06; hold marker NF-10.

## Hold markers (NF-01-NF-11)

**Reading note:** every marker carries the format `[INFORMATION NEEDED: <owner>; why; decision blocked]` (owner = role, per `03-registers.md` rules); markers are resolved only by recording the decision in `03-registers.md` - never silently.

- **NF-01** (whole document): `[INFORMATION NEEDED: program lead; beneficiary, charitable frame, and single public outcome approved in the register; blocks all narrative prose - DR-01/DR-06/DR-07]`
- **NF-02** (preamble): `[INFORMATION NEEDED: program lead; named person for each role (owner test); blocks the whole document - DR-01]`
- **NF-03** (Section 1): `[INFORMATION NEEDED: program lead; beneficiary, intervention, single public outcome, request amount, and result - DR-01/DR-06/DR-07/DR-04]`
- **NF-04** (Section 2): `[INFORMATION NEEDED: program lead; SF problem analysis from city sources and reachable-population estimate (F-11) - DR-01]`
- **NF-05** (Section 3): `[INFORMATION NEEDED: program lead; intervention with defined participant pathway (delivery-map W-03) - DR-01/DR-06]`
- **NF-06** (Section 4): `[INFORMATION NEEDED: program lead + evidence reviewer; theory-of-change causal links with evidence grades - DR-05/DR-07]`
- **NF-07** (Section 5): `[INFORMATION NEEDED: program lead; SF-establishment sequence, named capacity, and partner statuses - DR-01]`
- **NF-08** (Section 6): `[INFORMATION NEEDED: evidence reviewer + named evaluator (TBD - W-10); pre-registered indicator (baseline, target, instrument, collection timing) - DR-07]`
- **NF-09** (Section 7): `[INFORMATION NEEDED: budget owner; selected funding scenario and request amount - DR-04]`
- **NF-10** (Section 8): `[INFORMATION NEEDED: executive owner + rights owner; post-grant operating-cost model and rights schedule - DR-10/DR-09]`
- **NF-11** (gate): `[INFORMATION NEEDED: authorized officer; registration confirmation or written exception - DR-11/DR-03]`

## Decision gate - when narrative prose unblocks

**Gate (binding, FR-01).** Narrative prose is BLOCKED until: (1) the **scope-lock gate closes** - DR-01/DR-06/DR-07 closed with written rationale in `03-registers.md` §1.1 (the packet then reaches Draftable, D1); (2) **Section 7 additionally** requires DR-04 selected with the request amount and the proportionality loss list (`09-unit-cost-model.md` §6 gate; DR-04 deadline "Before narrative drafting"); (3) **Section 8 additionally** requires DR-10 (post-grant operating-cost model) and DR-09 (rights schedule). The registration gate (DR-11/DR-03, deadline Oct 14-15) is a submission gate: it does not block drafting, but a blocked registration outcome converts the deliverable to a gap report (stop conditions, `Refinement/02-refinement-checklist.md` §(a)).

**Once the gate opens:** a successor plan (still T10 content) replaces every hold marker and framework placeholder with prose written under FR-02/FR-03/FR-04/FR-06, then runs FR-08's tests; this file is re-verified with the full editing-test set (`Logs/instructions.md` §7) and the T10 verification (deletion + substitution + prohibited-words 0 hits + uncertainty phrases below E3).

**Until then:** this framework stands on its own - it passes the deletion test (rules, source references, and markers do not depend on the project name) and the substitution test (no invented SF facts; the only SF wording is the verbatim architecture heading, rule wording, and marker text).

## Revision record (per methodology)

| Date | Proposed change | Class | Reason | Evidence affected | Budget affected | Decision | Updated documents |
|---|---|---|---|---|---|---|---|
| 2026-10-14 | Narrative framework created (prose blocked): section skeleton with the 8 verbatim headings (Decision summary held - written last; Problem and beneficiaries; Intervention; Change mechanism; San Francisco execution; Evidence and measurement; Financial plan; Durability and governance); binding rules FR-01-FR-10 (prose block; paragraph method; drafting formula; uncertainty language; evidence grades E1-E5; paragraph-trace format; prohibited words; editing tests; decision summary written last; independent sections with page budgets); per-section source mapping table (8 rows); framework placeholders with hold markers NF-01-NF-11; decision-gate section (prose unblocks when DR-01/DR-06/DR-07 close; Section 7 additionally DR-04; Section 8 additionally DR-10/DR-09); zero prose sentences beyond framework headings, rules, and markers; DR-01/DR-04/DR-06/DR-07/DR-09/DR-10/DR-11 states propagated | Clarifying | Plan 001 T10 (CONTENT, LAST) requires the narrative written only after all evidence artifacts exist; DR-01/DR-06/DR-07 undecided and DR-04 unselected as of 2026-10-14, so the change records the framework the prose attaches to - no beneficiary, intervention, outcome, or figure invented | DR-01/DR-04/DR-06/DR-07/DR-09/DR-10/DR-11 decision states propagated (E1, source: 03-registers.md §1/§1.1; ungraded - undecided/unselected/blocked); E1 platform claims (C01-C05, C27) available as prose sources; no new figures | None - zero dollar figures | No decision closed - narrative stays not draftable until scope lock | 10-narrative.md (new), Logs/changes.md, Plan/000-index.md |