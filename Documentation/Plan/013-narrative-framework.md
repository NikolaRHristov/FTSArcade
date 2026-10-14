# 013 - Narrative Framework: Section Skeleton, Binding Rules, Source Map (T10)

> **For Hermes:** Execute this plan with one execute agent. The executor writes `Documentation/Prospectus/10-narrative.md` as a **narrative framework - not narrative prose** - because DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided as of 2026-10-14** (`03-registers.md` §1.1), DR-04 (funding scenario) is unselected, and the registration gate (DR-11) is Blocked. Per the methodology's stop conditions, the correct product while no beneficiary or intervention is approved is a gap report, not more prose - so this change produces the framework the narrative attaches to. The executor edits exactly three files (F2-F4), never commits, and reports the verified marker count. The orchestrator reviews, commits once (`docs(grant): narrative framework (T10)`), and flips the 000-index row through the lifecycle.

**Goal:** Satisfy plan 001 task T10 (bucket CONTENT, LAST) by creating `Documentation/Prospectus/10-narrative.md` - a NARRATIVE FRAMEWORK: (1) prose-block statement (narrative prose BLOCKED until the packet reaches Draftable - DR-01/DR-06/DR-07 closed in the register); (2) binding drafting rules FR-01-FR-10 (paragraph method; drafting formula; uncertainty-language requirements; evidence grades; paragraph-trace format; prohibited words; editing tests; decision summary written last; independent sections); (3) section skeleton with per-section source mapping (8 sections: 1 Decision summary (written last - held), 2 Problem and beneficiaries, 3 Intervention, 4 Change mechanism, 5 San Francisco execution, 6 Evidence and measurement, 7 Financial plan, 8 Durability and governance); (4) hold markers NF-01-NF-11 where prose attaches once decisions close; (5) decision-gate section - and appending the changes.md row and the 000-index.md row. No prose sentence is drafted: the file contains framework headings, rules, tables, and markers only - zero invented claims, zero dollar figures.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and the T10 task detail): no scope change occurs - no option of DR-01/DR-06/DR-07 is chosen or redefined, and no budget number changes; the change adds missing information (the narrative framework, the propagated decision states, and the prose-block gate) and creates one new packet document. This mirrors the Clarifying precedent of changes 004-012 (recorded undecided/unselected decision states; pathway, boundary, claim-ledger, first-year-plan, and unit-cost-model frameworks). Foundational would apply only if the decisions were made and changed scope; they are not. Operational would apply to delivery/budget numbers; the document adds none (zero dollar figures).

**Scope - in:** the 3 files listed in Section 1 (F2-F4) plus this plan file (F1, already written by the pre-plan agent).
**Scope - out:** drafting any narrative prose sentence (any invented beneficiary, intervention, outcome, partner, cost, or figure violates this plan); choosing or recommending any option of DR-01/DR-06/DR-07 or any DR-04 scenario or request amount; edits to `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `02-claim-ledger.md`, `04-delivery-and-budget.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, `08-first-year-operating-plan.md`, `09-unit-cost-model.md`, root `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/013-narrative-framework.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/10-narrative.md` | **New file** (verified absent at plan time): the narrative framework - write the Section 2.2 content verbatim |
| F3 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 013) after the plan-012 row (currently line 20) |
| F4 | `Documentation/Plan/000-index.md` | Modify: insert row 013, status `planned`, INSIDE the Index table directly after the plan-012 row (currently line 20) - NOT at end of file (see Section 4 placement rule) |

---

## 2. F2 - `Documentation/Prospectus/10-narrative.md` (NEW FILE)

### 2.1 File-level rules (binding)

- Write the file exactly as the fenced content in §2.2: headers verbatim, tables verbatim, cell text verbatim, relative links only. Do not add, remove, or reword any section, row, cell, or marker.
- All owners are **roles** (per `03-registers.md` rules: "All owners are roles; named persons are `[INFORMATION NEEDED: ...]`"). No person's name and no organization name may appear; the only role labels used are program lead, budget owner, evidence reviewer, named evaluator (TBD - W-10), executive owner, rights owner, authorized officer. The recorded fiscal-sponsor candidates are not named here (they belong to Section 5 prose once unblocked).
- **Zero prose sentences:** the file contains framework headings, binding rules, tables, markers, and placeholders only. A "prose sentence" is any sentence asserting a fact about the project, a beneficiary, an intervention, an outcome, a partner, a cost, or an SF condition. The paragraph-scan check (V1) enforces this mechanically.
- Zero dollar figures: the string `$` must not appear in the file (V7).
- No causal claims: the only causal wording is inside quoted decision-state references and claim refs; no gameplay-to-outcome statement.
- No prohibited words (instructions.md §6) - 0 hits (V5). In particular, the §6 blacklist is never written into the file by name; FR-07 references `Logs/instructions.md` §6 as the authoritative list.
- Quote fidelity: before writing, re-read `Documentation/Prospectus/03-registers.md` §1.1 (DR-01/DR-06/DR-07 undecided wording) and §1 rows (DR-04/DR-05/DR-09/DR-10/DR-11), `Logs/instructions.md` §5-§8, `Refinement/02-refinement-checklist.md` §(a) (stop conditions), and the Reference export (paragraph method, drafting formula, prospectus architecture, page budgets). If the recorded wording drifted from what §2.2 quotes, **stop and report - do not paraphrase or patch blind** (mirrors plans 008/009/011/012's quote-fidelity rule).
- Marker count (binding): exactly **11** `[INFORMATION NEEDED: ...]` markers (NF-01-NF-11), each on its own bullet line in the hold-marker section, plus **1** generic format description in the hold-marker reading note - `grep -c` reads **12** (V8 accounts for this).
- Cross-links reference only existing files (`01-source-case.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, `02-claim-ledger.md`, `08-first-year-operating-plan.md`, `09-unit-cost-model.md`, `05-durability-risks-rights.md`, `03-registers.md`, `04-delivery-and-budget.md`, `00-prospectus.md`, `Logs/instructions.md`, `Refinement/02-refinement-checklist.md`); the successor prose plan (still T10 content) is not a file yet and is never linked.

### 2.2 Complete file content (write exactly this)

```
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
```

### 2.3 INFORMATION NEEDED markers list (must appear in the file)

**11 markers** (NF-01-NF-11), each with owner + why + decision-blocked fields per instructions.md §5. `grep -c` on the file reads **12** hits including the 1 generic format description in the hold-marker reading note (V8 accounts for this). The consolidated list below is the unknowns register for the narrative; the complete inline marker texts appear in the file exactly as written in §2.2.

| ID | Owner | Decision blocked | Unblocks | Markers covered |
|---|---|---|---|---|
| NF-01 | Program lead | DR-01/DR-06/DR-07 | Whole document (prose block) | 1 |
| NF-02 | Program lead | DR-01 | Preamble (named persons per role, owner test) | 1 |
| NF-03 | Program lead | DR-01/DR-06/DR-07/DR-04 | Section 1 (decision-summary values) | 1 |
| NF-04 | Program lead | DR-01 | Section 2 (SF problem analysis; F-11) | 1 |
| NF-05 | Program lead | DR-01/DR-06 | Section 3 (intervention and pathway) | 1 |
| NF-06 | Program lead + evidence reviewer | DR-05/DR-07 | Section 4 (theory-of-change links) | 1 |
| NF-07 | Program lead | DR-01 | Section 5 (SF-establishment sequence, named capacity, partner statuses) | 1 |
| NF-08 | Evidence reviewer + named evaluator (TBD - W-10) | DR-07 | Section 6 (pre-registered indicator) | 1 |
| NF-09 | Budget owner | DR-04 | Section 7 (selected scenario and request amount) | 1 |
| NF-10 | Executive owner + rights owner | DR-10/DR-09 | Section 8 (post-grant model, rights schedule) | 1 |
| NF-11 | Authorized officer | DR-11/DR-03 | Decision gate (registration confirmation or written exception) | 1 |

Sum of the Markers covered column = **11**.

---

## 3. F3 - `Documentation/Logs/changes.md`

**Append one row after the plan-012 row (currently line 20), same column format (8 columns):**

```
| 2026-10-14 | Clarifying | Create narrative framework (`Prospectus/10-narrative.md`, new): framework-only - prose-block statement (narrative prose BLOCKED until the packet reaches Draftable - DR-01/DR-06/DR-07 closed in `03-registers.md` §1.1; stop conditions quoted from `Refinement/02-refinement-checklist.md` §(a); build order from `Logs/instructions.md` §8); binding rules FR-01-FR-10 (prose block; paragraph method - state claim, fact or mechanism, why it matters to San Francisco, evidence or limitation, connect, plus the five acceptance questions; drafting formula verbatim from the Reference export - "For [defined beneficiaries], [named barrier] limits [specific opportunity]. The project will [specific activity], delivered by [responsible party], so that [measurable result] occurs..."; uncertainty-language table - four verbatim phrases, mandatory wherever evidence is below E3; evidence grades E1-E5; paragraph-trace format - source, claim IDs, figures, evidence grade, limitation; prohibited words - 0 hits; editing tests - T10 verification: deletion + substitution + prohibited words + uncertainty phrases; decision summary written last using only accepted claims; each section independently understandable with page budgets); section skeleton with per-section source mapping table (8 rows: 1 Decision summary (held - all sections, written last), 2 Problem and beneficiaries (01), 3 Intervention (06/07), 4 Change mechanism (02), 5 San Francisco execution (08), 6 Evidence and measurement (02/ledger), 7 Financial plan (09), 8 Durability and governance (05)); the 8 verbatim section headings each carrying a framework placeholder; hold markers NF-01-NF-11 (whole-document, named persons, one per section, registration gate); decision-gate section (prose unblocks when DR-01/DR-06/DR-07 close; Section 7 additionally requires DR-04; Section 8 additionally DR-10/DR-09); zero prose sentences beyond framework headings, rules, and markers - zero invented claims; DR-01/DR-04/DR-06/DR-07/DR-09/DR-10/DR-11 states propagated | Plan 001 T10 (CONTENT, LAST) requires the narrative written only after all evidence artifacts exist; DR-01/DR-06/DR-07 undecided and DR-04 unselected as of 2026-10-14, so the change records the framework the prose attaches to - no beneficiary, intervention, outcome, or figure invented | **INFORMATION NEEDED marker count: 11 (12 `grep -c` hits incl. 1 generic format description in the hold-marker reading note)** - executor-verified; DR-01/DR-04/DR-06/DR-07/DR-09/DR-10/DR-11 decision states propagated (E1, source: 03-registers.md §1/§1.1; ungraded - undecided/unselected/blocked); E1 platform claims (C01-C05, C27) available as prose sources; no new figures; no budget affected | No decision closed - narrative stays not draftable until scope lock | Prospectus/10-narrative.md (new), Logs/changes.md, Plan/000-index.md | 013 |
```

---

## 4. F4 - `Documentation/Plan/000-index.md`

**Placement rule (binding - the 011/012 placement defect must not recur):** insert row 013 **inside the Index table**, directly after the plan-012 row (currently line 20) - i.e., between the `| 012 |` row and the blank line that precedes `## Status Lifecycle`. **Do not append at the end of the file:** plan 011's executor appended the 011 row at end-of-file (after `## Status Lifecycle`), rendering it outside the Index table (recorded as a non-blocking observation in `Documentation/Reviews/011-first-year-plan/evidence.md`). V13 verifies the row sits before the `## Status Lifecycle` heading.

```
| 013 | `Documentation/Plan/013-narrative-framework.md` | Narrative framework: section skeleton, binding rules (paragraph method, drafting formula, uncertainty language), per-section source map, prose-block gate (plan 001 T10) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 5. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T10: deletion + substitution tests; prohibited-words scan, 0 hits (Section 6 of instructions.md); uncertainty phrases used wherever evidence is below E3 - recorded here as binding rules (FR-04/FR-08) because the framework contains no prose yet; the prose-level T10 checks run at the successor drafting change. Per instructions.md §11.6, the orchestrator starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T10; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | Zero prose sentences (defined check) | Paragraph scan (below): split the file into blank-line-separated paragraphs; a paragraph is a prose sentence unless it matches an allowed framework form | Output "non-framework: 0" - every paragraph is a heading (`^#{1,3} `), table (`^\|`), list (`^[-*+>] `, `^\d+\. `), blockquote (`^> `), bold-labeled framework line (`^\*\*`), code fence, or marker line (`^\[INFORMATION NEEDED`) |
| V2 | Deletion test (framework level) | `grep -n 'FTSArcade' Documentation/Prospectus/10-narrative.md` | Occurrences only in the H1 title (≤ 2 hits); deleting the name leaves every paragraph a valid framework paragraph - rules, source references, and markers name files, not the project |
| V3 | Substitution test (framework level) | `grep -niE 'san francisco|\bSF\b' Documentation/Prospectus/10-narrative.md` | Every SF mention is a verbatim heading, rule wording (FR-02 step 3), source reference, or marker text; the file asserts no SF-specific fact (zero prose), so replacing SF with another city cannot invalidate any paragraph |
| V4 | Uncertainty-phrase rule present | `grep -nF 'As of [date], [source] shows' Documentation/Prospectus/10-narrative.md; grep -nF 'Comparable evidence suggests' ...; grep -nF 'The project will test whether' ...; grep -nF 'The planning target is' ...` | All four verbatim phrases appear in FR-04; the sentence "Uncertainty phrases are mandatory wherever evidence is below E3" appears |
| V5 | No prohibited words | `grep -rniE 'revolutionary|world-class|unique|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/10-narrative.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits in the three executed files (the blacklist is not written into the file by name; `Logs/instructions.md` §6 is authoritative) |
| V6 | Eight-section skeleton | `grep -n '^## [1-8]\. ' Documentation/Prospectus/10-narrative.md` | Exactly the 8 verbatim headings in order: Decision summary; Problem and beneficiaries; Intervention; Change mechanism; San Francisco execution; Evidence and measurement; Financial plan; Durability and governance |
| V7 | No invented figures / zero dollar figures | `grep -n '\$' Documentation/Prospectus/10-narrative.md`; inspect all figure references | 0 `$` hits; no numeric cost, volume, or total anywhere; the only figure references are data-dictionary IDs (F-11, F-01-F-11) and claim IDs (C01-C28, C21/C22/C24) |
| V8 | INFORMATION NEEDED markers complete | `grep -c '\[INFORMATION NEEDED:' Documentation/Prospectus/10-narrative.md` + inspect each marker | Count **12** (11 markers NF-01-NF-11 + 1 generic format description in the hold-marker reading note); every marker has a role owner, a why, and a blocked decision (DR refs); the §2.3 table contains exactly rows NF-01-NF-11 and the Markers covered column sums to 11. **Record the verified count in the changes.md row.** |
| V9 | Prose-block statement present | `grep -niE 'blocked|draftable|stop condition' Documentation/Prospectus/10-narrative.md` | The Status line and FR-01 state that narrative prose is BLOCKED until the packet reaches Draftable - DR-01/DR-06/DR-07 closed in `03-registers.md` §1.1; the Decision gate section states the unblock conditions (incl. Section 7 needing DR-04, Section 8 needing DR-10/DR-09) |
| V10 | Decision summary held | Inspect `## 1. Decision summary` | Section 1 carries its framework placeholder with the written-last rule (FR-09 quote) and hold marker NF-03; no summary content drafted |
| V11 | No drafting boundary | `grep -niE 'dear|subject:|sincerely' Documentation/Prospectus/10-narrative.md` | 0 hits (protocol R1; no email or promotional text introduced) |
| V12 | changes.md row | Inspect `Documentation/Logs/changes.md` | One new row: class **Clarifying**, plan ref 013, date 2026-10-14, documents updated listing the new file + `Logs/changes.md` + `Plan/000-index.md`; appended after the plan-012 row; existing rows unchanged |
| V13 | Index row inside the table | `grep -n '| 013 |' Documentation/Plan/000-index.md; grep -n '## Status Lifecycle' Documentation/Plan/000-index.md` | Output **1** for the 013 row; the row's line number is **less than** the `## Status Lifecycle` line number (inside the Index table, directly after the `| 012 |` row - the 011/012 end-of-file placement defect must not recur); status `planned`; existing rows 001-012 unchanged |
| V14 | Tables render | For every table in the new file (FR-05 evidence grades; section skeleton; revision record): header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each |
| V15 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | Exactly 1 new file (`Documentation/Prospectus/10-narrative.md`) + exactly 2 modified files (`Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md`); `Documentation/Plan/013-narrative-framework.md` appears as the pre-plan artifact (untracked); no other file touched; no deletions |

**V1 command (run as one script; pass = `non-framework: 0`):**

```
python3 - <<'EOF'
import re
text = open('Documentation/Prospectus/10-narrative.md', encoding='utf-8').read()
paras = [p.strip() for p in re.split(r'\n\s*\n', text) if p.strip()]
allowed = re.compile(r'^(#{1,3} |\||[-*+>] |\d+\. |> |\*\*|```|\[INFORMATION NEEDED)')
bad = [p for p in paras if not allowed.match(p)]
print('paragraphs:', len(paras), '| non-framework:', len(bad))
for p in bad[:5]:
    print('---', p[:100])
EOF
```

---

## 6. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| DR-01/DR-04/DR-05/DR-06/DR-07/DR-09/DR-10/DR-11 decision states, verbatim | `Documentation/Prospectus/03-registers.md` §1 (DR rows) and §1.1 (recorded decisions) | Status line, FR-01, gate section, and hold markers carry the states; quote-fidelity rule (stop if drifted, do not patch blind) |
| Evidence grades, uncertainty phrases, prohibited words, editing tests, build order | `Documentation/Logs/instructions.md` §5, §6, §7, §8 | FR-04/FR-05/FR-07/FR-08 quote these; the E1-E5 table is copied verbatim |
| Stop conditions | `Documentation/Refinement/02-refinement-checklist.md` §(a) | FR-01 quotes the gap-report stop condition |
| Paragraph method, drafting formula, prospectus architecture, page budgets | `Documentation/Reference/we're looking to prepare a grant application for h.md` ("Use a fixed paragraph method"; "Prospectus architecture"; page-budget table) | FR-02/FR-03/FR-09/FR-10 and the source-map Page budget column |
| Section headings of the seven evidence artifacts | `Documentation/Prospectus/01-source-case.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, `02-claim-ledger.md`, `08-first-year-operating-plan.md`, `09-unit-cost-model.md`, `05-durability-risks-rights.md` | Source-map table rows 2-8 (artifact and section refs) |
| E1 platform claims and E5 prohibition records | `Documentation/Prospectus/02-claim-ledger.md` | Source-map rows 4/6 name C01-C28 and C21/C22/C24 |
| Current row positions in F3/F4 | `Documentation/Logs/changes.md` (plan-012 row at line 20), `Documentation/Plan/000-index.md` (plan-012 row at line 20; `## Status Lifecycle` at line 22) | Append/insert after the plan-012 rows; re-check at execution |

**Explicitly out of scope for the executor:** drafting any narrative prose sentence (any invented beneficiary, intervention, outcome, partner, cost, or figure violates this plan; prose attaches only in a successor change after DR-01/DR-06/DR-07 close); choosing or recommending any DR-01/DR-06/DR-07 option or any DR-04 scenario or request amount; editing `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `02-claim-ledger.md`, `04-delivery-and-budget.md`, `05-durability-risks-rights.md`, `06-participant-pathway.md`, `07-platform-boundary.md`, `08-first-year-operating-plan.md`, `09-unit-cost-model.md`, root `README.md`, `Documentation/Research/*`, or `Documentation/Refinement/*`; drafting any email or promotional copy (protocol R1); committing (orchestrator-only, rule R2).

---

## 7. Revision note (plan amendments)

| Date | Amendment | Class | Reason |
|---|---|---|---|
| (none at plan time) | - | - | - |