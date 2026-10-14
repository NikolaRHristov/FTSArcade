# 006 - Charitable Frame Scope Lock: Record DR-06 Decision State and Options (T03)

> **For Hermes:** Execute this plan with an execute agent. Orchestrator reviews and commits once (`docs(grant): <change>`). This change records the DR-06 (charitable frame) decision **state** - undecided as of 2026-10-14 - and the candidate frames with the six-question commercial-benefit test applied, **without choosing a frame** (no frame is adopted anywhere in the packet; picking one is forbidden by this plan).

**Goal:** Satisfy plan 001 task T03 (bucket SCOPE-LOCK): record the DR-06 charitable-frame decision honestly in `Documentation/Prospectus/03-registers.md` §1.1 (decision state, options table with commercial-benefit-test results, decision rule, needed evidence, owner, deadline, consequence), and apply the record where the decision bites in `01-source-case.md` (intervention, platform-role, theory-of-change, eligibility rows; ten-statement #7; revision record) and `00-prospectus.md` (Decision summary intervention line, §3.1, §4.2, §8, §10.1, §11), plus the `changes.md` row and `000-index.md` row.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2, instructions.md §9.2, and the T03 task detail): no scope change occurs - no charitable frame is defined or redefined; the change adds missing information (the decision state) and records a decision-register entry, exactly mirroring changes 004 (DR-11) and 005 (DR-01). Foundational would apply only if the decision were made and changed scope (the §9.2 example "Scope-lock decision (DR-01/06/07)" presumes a decision); it is not - the frame stays undecided.

**Scope - in:** the 6 files listed in Section 1 (1 new plan file exists already; 5 documents edited).
**Scope - out:** choosing or recommending a charitable frame (any such action violates this plan); any edit to `00-alignment-matrix.md` (its Table B charitable-use row already states the decision needed: "ONE public-benefit frame; businesses separated from the charitable program; commercial-benefit test applied to each feature" with owner program lead + counsel), root `README.md` (no status field changes - gate stays Blocked per DR-11, packet stays Not ready), `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/006-charitable-frame.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/03-registers.md` | Modify: DR-06 live row; append DR-06 §1.1 entry + options-detail block |
| F3 | `Documentation/Prospectus/01-source-case.md` | Modify: rows 3, 4, 5, 10 status cells; ten-statement #7; append revision-record row |
| F4 | `Documentation/Prospectus/00-prospectus.md` | Modify: §1 Intervention line; §3.1 candidate-directions line; §4.2 section; §8 claim; §10.1 governance bullet; §11 row 5 |
| F5 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 006) |
| F6 | `Documentation/Plan/000-index.md` | Modify: append row 006, status `planned` |

---

## 2. F2 - `Documentation/Prospectus/03-registers.md`

### 2.1 Replace the live DR-06 row (Section 1 table, currently line 17)

**Current text (quote):**
```
| DR-06 | **Charitable frame** | (a) Public cultural-installation program supported by commerce; (b) Commercial arcade business with civic branding (likely ineligible as a grant case); (c) none approved | Only (a)-type frames fit this competition, and only with defined beneficiary, site plan, access rules, and evidence | Defined public benefit; permission from landmark/business owners; advertising-standard control plan | Decision owner | Before scope lock | Project identity undefined; Ambition criterion unscorable |
```

**Replacement:**
```
| DR-06 | **Charitable frame** | (a) Public cultural-installation program supported by commercial activity (the export's hypothesized frame: free public cultural/recreational game installations documenting specific SF places, funded by advertising/commerce); (b) Commercial arcade business with civic branding (rejected-type option - likely ineligible as a grant case); (c) none approved - **all recorded, not chosen** (see §1.1) | Public benefit must be primary and defined; private benefit no more than incidental (rules §3/§8); every commercial feature passes the six-question commercial-benefit test incl. the revenue-zero question; only (a)-type frames fit this competition, and only with defined beneficiary, site plan, access rules, and evidence | Defined public benefit; site plan; access rules; business-selection rules; advertising-standard control plan; permission from landmark/business owners; evidence connecting gameplay to public benefit; charity-law review | Program lead + counsel | Before scope lock (not achieved) | Project identity undefined; Ambition criterion unscorable; commercial roster cannot be separated from any charitable program |
```

The Options cell drops the bare label and adds the export's frame wording; the Decision rule cell adds the public-benefit-primary / incidental-private-benefit rule and the commercial-benefit-test (revenue-zero) requirement; the Needed-information and Owner cells align with the Table B charitable-use row (owner: program lead + counsel).

### 2.2 §1.1 intro sentence - NO change

Already updated by change 005 ("Entries are appended as decisions are made **or decision states are recorded**..."). Do not touch it. The DR-11 and DR-01 §1.1 rows and the DR-01 options-detail block stay untouched.

### 2.3 Append the DR-06 recorded entry to the §1.1 table

**Insert** one new row as the last row of the §1.1 table (immediately after the DR-01 row - the row beginning `| DR-01 | Beneficiary | **Undecided as of 2026-10-14**` - i.e., between that row and the blank line preceding the `**DR-01 option detail (recorded 2026-10-14, not chosen).**` paragraph).

**New row (quote to insert, DR-11/DR-01 column format):**
```
| DR-06 | Charitable frame | **Undecided as of 2026-10-14** - as of 2026-10-14, no packet document adopts a charitable frame: the export's hypothesized frame ("Provide publicly accessible cultural and recreational game installations that document and increase engagement with specific San Francisco places, while any advertising or commerce funds free public access." - `Documentation/Reference/we're looking to prepare a grant application for h.md`, §"Choose a charitable frame") is an E4 hypothesis with no defined beneficiary, site plan, access rules, or evidence connecting gameplay to a public benefit; the commercial arcade business with civic branding is recorded as the rejected-type option (export §"it's both": only the first identity is likely to fit this competition); none approved is the base case. The candidate options below are recorded from the export; they are **options, not chosen**. The unresolved state is consistent with `01-source-case.md` rows 3-5 and 10, `00-prospectus.md` §4.2 and §8, evidence-register rows C19-C20, and `00-alignment-matrix.md` Table B (charitable-use row), all of which carry the E4/unresolved state. No positive claim is made about a frame; the status is recorded as undecided. | Program lead + counsel `[INFORMATION NEEDED: named persons; required to own the frame decision and the charity-law review of incidental-private-benefit controls; blocks Mechanism, Ambition - DR-06]` | 2026-10-14 | E1 (frame text, commercial-benefit test, and identity contrast sourced from the export and the DR-06 register row, verified 2026-10-14; the undecided status itself is ungraded - no positive claim, mirroring DR-11) | **Open** (scope not locked; downstream work paused) | Program lead + counsel: (1) apply the six-question commercial-benefit test to every roster item (export §"Commercial-benefit test": what charitable result it produces; who pays and who benefits; would the feature still belong if it generated no revenue; could it advantage the company or advertisers more than the public; what rule prevents excessive private benefit; what happens to public access if advertising disappears); (2) for the (a)-type frame, define the public benefit, site plan, access rules, business-selection rules, and advertising standards; (3) obtain charity-law review that private benefit stays no-more-than-incidental (rules §3/§8); (4) choose ONE option by the decision rule below; record the decision as a new DR-06 addendum. |
```

### 2.4 Append the DR-06 options-detail block

**Insert** immediately after the DR-01 options-detail block's final line `**Consequence of delay:** all downstream work pauses; packet stays Not ready.` (currently line 46) and before the `---` separator that precedes `## 2. Data dictionary`.

**Insert (quote):**
```
**DR-06 option detail (recorded 2026-10-14, not chosen).** Sources: export `Documentation/Reference/we're looking to prepare a grant application for h.md` §"Separate the businesses" (roster separation), §"Choose a charitable frame" (frame text), §"Commercial-benefit test" (six questions), and §"it's both" (identity contrast - "Only the first is likely to fit this competition"); option (c) is the base case. The commercial-benefit-test column applies the export's six questions; question 3 is decisive per the export ("If the honest answer to the third question is no, the feature probably belongs in the business plan rather than the grant narrative"). Weakest-assumption column is the adversarial test (instructions.md §7.8) applied per option.

| Option | Proposed role for FTSArcade | Commercial-benefit test (six questions, export §"Commercial-benefit test") | Weakest assumption (adversarial test) |
|---|---|---|---|
| (a) Public cultural-installation program supported by commerce | Free public cultural/recreational installations documenting specific SF places, funded by advertising/commerce (export's hypothesized frame) | Q1 charitable result: free public access + documented engagement with specific SF places (E4, untested). Q2 payer/beneficiary: commerce pays; SF residents/visitors benefit by design. Q3 revenue-zero: **passes by design** - free public access is the frame's core and must survive zero revenue (free-access rule not yet written). Q4 private-benefit risk: businesses/landmarks could gain more than the public - controlled by business-selection rules + advertising standards (none designed). Q5 rule: rules §3/§8 - funds for tax-exempt purposes; private benefit incidental only (E1). Q6 access if advertising disappears: must be answered by a written free-access rule - not yet designed | Commerce can fund free public access while private benefit stays incidental - no site plan, access rules, business-selection rules, or advertising controls exist (E4, untested) |
| (b) Commercial arcade business with civic branding | Commercial business whose city promotion is the project identity (rejected-type option) | Q1 charitable result: city popularity/notoriety - not a measurable outcome; business promotion cannot itself be the public benefit (export). Q2 payer/beneficiary: customers and advertisers pay; the company and advertisers benefit; public benefit undefined. Q3 revenue-zero: **fails** - the roster items (cabinet sales, custom development, ad space, referrals) belong in the business plan, not the grant narrative (export's own rule). Q4 private-benefit risk: advantage to the company/advertisers is the purpose, not incidental. Q5 rule: no rule can make promotion incidental while promotion is the purpose. Q6 access: no free-access rule; no charitable access defined | City exposure through business upselling constitutes a charitable public benefit - export: commercial and promotional effects do not by themselves establish the charitable project (E4, untested) |
| (c) None approved | No charitable frame adopted | Not applicable - no frame, so no commercial-benefit questions are answered | No frame leaves the commercial roster inseparable from any charitable program, rubric criterion 1 (Ambition) unscorable (score 1-2), and the packet Not ready - the recorded base case, not a plan |

**Decision rule:** public benefit must be primary and defined (beneficiary, site plan, access rules, business-selection rules, advertising standards); private benefit must be no more than incidental (rules §3/§8, E1); every commercial feature must pass the six-question commercial-benefit test, including the revenue-zero question (export §"Commercial-benefit test"); only (a)-type frames fit this competition (export §"it's both").
**Needed evidence:** defined public benefit with free-access rules; site plan; permission from landmark/business owners; business-selection rules; advertising-standard control plan; evidence connecting gameplay to the stated public benefit; charity-law review of incidental-private-benefit controls.
**Owner:** program lead + counsel (named persons `[INFORMATION NEEDED]`).
**Deadline:** before scope lock (not achieved).
**Consequence of delay:** project identity undefined; the commercial roster cannot be separated from any charitable program; Ambition criterion unscorable (score 1-2); packet stays Not ready.
```

---

## 3. F3 - `Documentation/Prospectus/01-source-case.md`

### 3.1 Replace row 3 (Intervention) status cell (currently line 11)

**Current text (quote):** `**NOT DEFINED.** No participant pathway. Candidate directions (creative workforce pathways; accessible community learning; community connection) are options only. \`[INFORMATION NEEDED: program lead; required to specify pathway, dose, setting, staffing, completion rule; blocks Sections 3-4 - DR-05]\``

**Replacement:** `**NOT DEFINED.** No participant pathway. Candidate directions (creative workforce pathways; accessible community learning; community connection; public cultural-installation program - charitable frame decision state recorded 2026-10-14 as undecided, \`03-registers.md\` §1.1 DR-06) are options only. \`[INFORMATION NEEDED: program lead; required to specify pathway, dose, setting, staffing, completion rule; blocks Sections 3-4 - DR-05]\``

### 3.2 Replace row 4 (Platform role) status cell (currently line 12)

**Current text (quote):** `**PROVISIONAL ONLY.** Known product facts (E1): browser-based, publicly accessible, free play, 24 cabinets listed, 15 live, 8 WIP, settings incl. reduced-motion accessibility. Essential-function list is empty until intervention is chosen. Platform boundary: see \`00-prospectus.md\` §3.2. \`[INFORMATION NEEDED: program lead; required to name the unique contribution; blocks Solution - DR-01/DR-05]\``

**Replacement:** `**PROVISIONAL ONLY.** Known product facts (E1): browser-based, publicly accessible, free play, 24 cabinets listed, 15 live, 8 WIP, settings incl. reduced-motion accessibility. Essential-function list is empty until intervention is chosen. The charitable frame that would define the platform's public role (free public access vs commercial service) is **undecided** as of 2026-10-14 (\`03-registers.md\` §1.1, DR-06). Platform boundary: see \`00-prospectus.md\` §3.2. \`[INFORMATION NEEDED: program lead; required to name the unique contribution; blocks Solution - DR-01/DR-05]\``

### 3.3 Replace row 5 (Theory of change) status cell (currently line 13)

**Current text (quote):** `**NOT DEFINED.** All four causal links blocked. Candidate charitable frame is an E4 hypothesis, not adopted. \`[INFORMATION NEEDED: decision owner; required for Mechanism section; blocks rubric criterion 1 - DR-06/DR-07]\``

**Replacement:** `**NOT DEFINED.** All four causal links blocked. Charitable frame decision state recorded 2026-10-14 (\`03-registers.md\` §1.1, DR-06): **undecided** - frame options (a) public cultural-installation program supported by commerce, (b) commercial arcade business with civic branding (rejected-type), (c) none approved are recorded, **not chosen**; the export's hypothesized frame remains an E4 hypothesis. \`[INFORMATION NEEDED: program lead + counsel; required for Mechanism section; blocks rubric criterion 1 - DR-06/DR-07]\``

### 3.4 Replace row 10 (Eligibility) status cell (currently line 18)

**Current text (quote):** `**UNRESOLVED.** Registration status unknown (Sept 11 deadline passed); legal entity, jurisdiction, tax status unknown; non-U.S. entity requires written confirmation; for-profit leads face expenditure responsibility (IRC §4945(h)); funds must serve charitable purposes with only incidental private benefit; rights/ownership of platform assets undocumented. \`[INFORMATION NEEDED: authorized officer; required to confirm a valid route to submit; blocks the application itself - DR-02/DR-03/DR-09]\``

**Replacement:** `**UNRESOLVED.** Registration status unknown (Sept 11 deadline passed); legal entity, jurisdiction, tax status unknown; non-U.S. entity requires written confirmation; for-profit leads face expenditure responsibility (IRC §4945(h)); funds must serve charitable purposes with only incidental private benefit (the charitable frame defining that purpose is **undecided** as of 2026-10-14 - \`03-registers.md\` §1.1, DR-06); rights/ownership of platform assets undocumented. \`[INFORMATION NEEDED: authorized officer; required to confirm a valid route to submit; blocks the application itself - DR-02/DR-03/DR-09]\``

### 3.5 Ten-statement #7 (currently line 30)

**Current text (quote):** `7. "The evidence for the mechanism is [grade and source], limited by [difference]." → **UNKNOWN** - no mechanism chosen; no analogous evidence identified`

**Replacement:** `7. "The evidence for the mechanism is [grade and source], limited by [difference]." → **UNKNOWN** - no mechanism chosen; charitable frame undecided as of 2026-10-14 (\`03-registers.md\` §1.1, DR-06); no analogous evidence identified`

### 3.6 Append one row to the Revision record table (after line 44)

**New row (quote):**
```
| 2026-10-14 | DR-06 charitable frame decision state recorded (undecided; frame options with six-question commercial-benefit test applied, not chosen) | Clarifying | Plan 001 T03 requires the scope-lock record; no frame is adopted anywhere, so the state - not a frame - is recorded | Export frame text + commercial-benefit test (E1, source); no new figures; E4 assumptions unchanged | Undecided as of 2026-10-14; owner program lead + counsel; deadline before scope lock | 03-registers.md, 01-source-case.md, 00-prospectus.md |
```

---

## 4. F4 - `Documentation/Prospectus/00-prospectus.md`

### 4.1 §1 Decision summary - Intervention line (currently line 20)

**Current text (quote):** `**Intervention:** Not yet chosen. The team's commercial roster (cabinet sales, custom game development, city-promotion ecosystem, internal game economy, stickers/QR/Uber referrals) is a set of businesses, not a charitable intervention. A single admissible framing has been hypothesized but not adopted: *"Provide publicly accessible cultural and recreational game installations that document and increase engagement with specific San Francisco places, while any advertising or commerce funds free public access."* This is an **E4 assumption** pending a beneficiary, site plan, access rules, and evidence (\`[DR-06]\`).`

**Replacement:** `**Intervention:** Not yet chosen. The team's commercial roster (cabinet sales, custom game development, city-promotion ecosystem, internal game economy, stickers/QR/Uber referrals) is a set of businesses, not a charitable intervention. A single admissible framing has been hypothesized but not adopted: *"Provide publicly accessible cultural and recreational game installations that document and increase engagement with specific San Francisco places, while any advertising or commerce funds free public access."* This is an **E4 assumption** pending a beneficiary, site plan, access rules, and evidence. Decision state recorded 2026-10-14 (\`03-registers.md\` §1.1, DR-06): **undecided** - frame options recorded, none chosen (\`[DR-06]\`).`

### 4.2 §3.1 candidate-directions line (currently line 67)

**Current text (quote):** `Candidate directions from the export (options, **not chosen**, recorded 2026-10-14 in \`03-registers.md\` §1.1 with roles, evidence needs, and weakest assumptions): creative workforce pathways; accessible community learning; community connection; public cultural-installation program (DR-06 frame hypothesis); none approved. Each would give FTSArcade a different function (entry point into structured game-development training; platform for facilitated digital-literacy programs; tool for recurring facilitated neighborhood activities). Choosing one is \`[DR-01]\`.`

**Replacement:** `Candidate directions from the export (options, **not chosen**, recorded 2026-10-14 in \`03-registers.md\` §1.1 with roles, evidence needs, and weakest assumptions): creative workforce pathways; accessible community learning; community connection; public cultural-installation program (DR-06 frame - decision state recorded 2026-10-14 as undecided, \`03-registers.md\` §1.1); none approved. Each would give FTSArcade a different function (entry point into structured game-development training; platform for facilitated digital-literacy programs; tool for recurring facilitated neighborhood activities). Choosing one is \`[DR-01]\`; the frame for the public cultural-installation direction is \`[DR-06]\`.`

### 4.3 §4.2 Candidate charitable frame (currently lines 95-99)

**Current text (quote):**
```
### 4.2 Candidate charitable frame (E4 hypothesis, not adopted)

> Participating businesses fund or host public arcade installations. The installations feature approved San Francisco places and businesses. Public use creates measurable cultural, educational, recreational, or economic benefits for San Francisco residents. Advertising and upselling remain subordinate to that public purpose.

Every arrow in this chain is currently unproven and must be labeled an assumption until defined: public beneficiary; public result (free cultural access, documented local history, youth activity, verified spending - not "popularity"/"notoriety", which are not measurable outcomes as stated); business benefit that is incidental; selection rules for businesses/landmarks; free-access rules; and evidence connecting gameplay to the stated city benefit. Decision: \`[DR-06]\`.
```

**Replacement:**
```
### 4.2 Candidate charitable frame (decision state undecided as of 2026-10-14; E4 hypothesis, not adopted)

**Decision state recorded 2026-10-14 (\`03-registers.md\` §1.1, DR-06): undecided** - the frame options are recorded, not chosen: (a) public cultural-installation program supported by commerce (the export's hypothesized frame below), (b) commercial arcade business with civic branding (rejected-type option - export: only the first is likely to fit this competition), (c) none approved. Every roster item remains a business, not a charitable intervention, until a frame is chosen.

> Participating businesses fund or host public arcade installations. The installations feature approved San Francisco places and businesses. Public use creates measurable cultural, educational, recreational, or economic benefits for San Francisco residents. Advertising and upselling remain subordinate to that public purpose.

Every arrow in this chain is currently unproven and must be labeled an assumption until defined: public beneficiary; public result (free cultural access, documented local history, youth activity, verified spending - not "popularity"/"notoriety", which are not measurable outcomes as stated); business benefit that is incidental; selection rules for businesses/landmarks; free-access rules; and evidence connecting gameplay to the stated city benefit. Decision: \`[DR-06]\` (undecided as of 2026-10-14 - \`03-registers.md\` §1.1).
```

### 4.4 §8 Financial plan - claim (currently line 184)

**Current text (quote):** `**Claim (E1, rule):** Award funds may not be used entirely for general operating support; for-profit leads face expenditure responsibility under IRC §4945(h); spending must serve tax-exempt purposes with only incidental private benefit.`

**Replacement:** `**Claim (E1, rule):** Award funds may not be used entirely for general operating support; for-profit leads face expenditure responsibility under IRC §4945(h); spending must serve tax-exempt purposes with only incidental private benefit (rules §3/§8; the charitable frame defining the tax-exempt purpose is **undecided** as of 2026-10-14 - \`03-registers.md\` §1.1, DR-06).`

### 4.5 §10.1 Governance - award-spending bullet (currently line 218)

**Current text (quote):** `- Award-spending controls for a for-profit lead: documented charitable purpose and permitted-use budget; project-specific accounting; financial/outcome reporting; policies for owner compensation, related-party transactions, and IP licensing; procedures to identify and prevent prohibited spending (recommend U.S. nonprofit-tax counsel and accountant).`

**Replacement:** `- Award-spending controls for a for-profit lead: documented charitable purpose and permitted-use budget; project-specific accounting; financial/outcome reporting; policies for owner compensation, related-party transactions, and IP licensing; procedures to identify and prevent prohibited spending (recommend U.S. nonprofit-tax counsel and accountant). The documented charitable purpose depends on the charitable frame - **undecided** as of 2026-10-14 (\`03-registers.md\` §1.1, DR-06).`

### 4.6 §11 Blocking unknowns - row 5 (currently line 238)

**Current text (quote):** `| 5 | Charitable frame + single public outcome | Mechanism, Ambition | Decision owner | DR-06, DR-07 |`

**Replacement:** `| 5 | Charitable frame + single public outcome | Mechanism, Ambition | Decision owner | DR-06 (undecided as of 2026-10-14 - recorded \`03-registers.md\` §1.1), DR-07 |`

---

## 5. F5 - `Documentation/Logs/changes.md`

**Append one row after the plan-005 row (currently line 14), same column format:**

```
| 2026-10-14 | Clarifying | Record DR-06 charitable frame decision state (undecided as of 2026-10-14): candidate frames (a) public cultural-installation program supported by commerce, (b) commercial arcade business with civic branding (rejected-type option), (c) none approved - recorded, not chosen; six-question commercial-benefit test applied per option; decision rule (public benefit primary; private benefit incidental; revenue-zero test), owner (program lead + counsel), deadline (before scope lock), consequence (identity undefined; Ambition unscorable) | Plan 001 T03 (SCOPE-LOCK) requires the frame record; no frame is adopted anywhere, so the record states the undecided state - no frame chosen | Export frame text + commercial-benefit test (E1, source); status itself ungraded (undecided); no budget affected | Recorded: undecided as of 2026-10-14; deciding owner = program lead + counsel; gate effect Open (scope not locked) | Prospectus/03-registers.md, Prospectus/01-source-case.md, Prospectus/00-prospectus.md, Plan/000-index.md | 006 |
```

---

## 6. F6 - `Documentation/Plan/000-index.md`

**Append one row after the plan-005 row (currently line 13):**

```
| 006 | `Documentation/Plan/006-charitable-frame.md` | Charitable frame scope lock: record DR-06 decision state and options (plan 001 T03) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 7. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T03: owner test; adversarial test (weakest assumption of the chosen frame acknowledged in writing - here, of each recorded option); affected files updated and cross-linked; changes.md row. Per instructions.md §11.6, the orchestrator also starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T03; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No frame chosen | Read the changed cells (03-registers §1.1 entry + option table, source-case rows 3/4/5/10, prospectus §1/§3.1/§4.2/§8/§10.1/§11) | 0 positive claims of an adopted frame; the only frame wording is inside the recorded option descriptions (a)-(b) and the export's quoted hypothesis; "undecided"/"recorded, not chosen"/"options" language present in all changed locations; the §4.2 heading carries the undecided state |
| V2 | Uncertainty language | `grep -n "Undecided as of 2026-10-14" Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md` | ≥1 hit in 03-registers.md §1.1; the status carries no evidence grade of its own (graded only as "ungraded - no positive claim", mirroring DR-11); phrase "as of 2026-10-14" present |
| V3 | Owner test | Inspect the §1.1 DR-06 entry | Deciding owner named = Program lead + counsel (roles); named-person `[INFORMATION NEEDED: ...]` markers preserved; every next-action verb has the program lead + counsel as party |
| V4 | Adversarial test | Inspect the §1.1 options-detail table | Every option (a)-(c) has a weakest-assumption cell acknowledging the untested assumption (E4) |
| V5 | Cross-links | `test -f Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md Documentation/Logs/changes.md Documentation/Plan/000-index.md; echo "EXIT:$?"` + inspect `[DR-06]`/`[INFORMATION NEEDED]` references | All files exist (EXIT:0); §1.1 entry ↔ source-case rows 3/4/5/10 ↔ prospectus §1/§3.1/§4.2/§8/§10.1/§11 references resolve; `00-alignment-matrix.md` Table B charitable-use row consistent with the recorded owner (program lead + counsel) and decision-needed state; evidence-register rows C19-C20 remain consistent (E4, untested); no dangling relative link |
| V6 | Tables render | For each edited table (03-registers §1 table, §1.1 table, §1.1 option table; changes.md; 000-index): header row, separator row, body rows have equal pipe counts | Equal pipe counts per table; separator row present in each |
| V7 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md Documentation/Logs/changes.md Documentation/Plan/000-index.md Documentation/Plan/006-charitable-frame.md` | 0 hits (this plan file included). "unique" is checked separately per plan 001 V3's caveat: allowed only inside instructions.md §6's own list; the prospectus's pre-existing "uniquely" (line 22) is not in scope of this change |
| V8 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | Exactly 1 added file (`Documentation/Plan/006-charitable-frame.md` - written by the pre-plan agent) + exactly 5 modified files (F2-F6); no other file touched, no deletions |
| V9 | changes.md row | Inspect changes.md | One new row with class **Clarifying**, plan ref 006, date 2026-10-14, documents updated listing F2-F4 + F6 |
| V10 | Index self-consistency | Inspect 000-index.md | Row 006 present, status `planned`; existing rows 001-005 unchanged |

---

## 8. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| Exact current rows to replace | F2-F4 as quoted in Sections 2-4 (re-read at execution; if any quoted text drifted, stop and report - do not patch blind) | Precision requirement; quote fidelity |
| Export frame text + identity contrast | `Documentation/Reference/we're looking to prepare a grant application for h.md` §"Separate the businesses" (~lines 2403-2413), §"Choose a charitable frame" (~lines 2428-2444), §"Build the source claims" (~lines 2447-2458), §"Commercial-benefit test" (~lines 2460-2471), §"it's both" (~lines 2482-2496) | Canonical source of the frame hypothesis, the roster-separation requirement, the six questions, and the "only the first is likely to fit this competition" identity contrast |
| §1.1 entry format | 03-registers.md DR-11 and DR-01 rows | Column format and the "unknown/undecided state" precedent (change 004/005) |
| Rules §3/§8 constraint | `00-alignment-matrix.md` Table B charitable-use row; `00-prospectus.md` §8 | "Award funds exclusively for tax-exempt purposes; private benefit no more than incidental" is the binding legal constraint behind DR-06 |
| Change-class definition | `Documentation/Logs/instructions.md` §9.2; plan 001 §0.2 | Class Clarifying (no scope change - no frame adopted) |

**Explicitly out of scope for the executor:** choosing or recommending a charitable frame (any such action violates this plan); editing `00-alignment-matrix.md` (its Table B charitable-use row already states the decision needed and the owner program lead + counsel); editing root `README.md` (no status field changes - gate stays Blocked per DR-11, packet stays Not ready); drafting any email or promotional copy (protocol R1).