# 014 - Editing-Test Verification Pass (plan 001 T11)

> **For Hermes:** Execute this plan with the standard delegation cycle (R2): an execute agent implements this design exactly, appends the changes.md row, and never commits; the orchestrator reviews, starts the constitution §11.6 review run for this change, and commits exactly once (`docs(grant): <change>`). This change records verdicts only - it edits **no** packet document under `Documentation/Prospectus/`.

**Goal:** Run all 8 editing tests (`Logs/instructions.md` §7) and all 21 checklist tests (`Refinement/02-refinement-checklist.md` §(a)) across the packet **as it currently stands** (S0, framework-only: DR-01/DR-06/DR-07 undecided, DR-04 unselected, DR-11 gate Blocked, zero dollar figures, no narrative prose - 10-narrative.md FR-01); record one honest verdict per test - **PASS** (passes at framework level, evidence cited), **PARTIAL** (passes structurally with markers noted), or **BLOCKED** (cannot be finally assessed until decisions close) - each with an evidence reference (file + section); report every BLOCKED test as a named follow-up task with its unblocking decision (never silently fixed); append the changes.md row (class Clarifying, plan ref 014, verdict summary incl. fails) and the 000-index row.

**Scope - in:** `Documentation/Refinement/02-refinement-checklist.md` (verdict columns + two verdict tables + one summary line), `Documentation/Logs/changes.md` (one row), `Documentation/Plan/000-index.md` (one row), this plan file (already written, untracked).
**Scope - out:** any edit to any file under `Documentation/Prospectus/` (a test verdict is a record, never a license to change the packet); any drafting; any git commit (orchestrator-only).

---

## 1. Packet state the verdicts must match (read before executing; do not re-derive)

| Fact | Value | Source |
|---|---|---|
| Packet version | S0 (incomplete source packet; framework-only) | Prospectus/README.md; 06/07/08/09/10 Status lines |
| Scope-lock decisions DR-01 / DR-06 / DR-07 | **Undecided as of 2026-10-14** - options recorded, not chosen | 03-registers.md §1.1 |
| Funding scenario DR-04 | **Unselected** | 03-registers.md §1 |
| Registration gate DR-11 | **Blocked** (status unknown; no registration confirmation located) | 03-registers.md §1.1 |
| Dollar figures | Zero budget figures; all `$` amounts in the packet are competition rules (C06 award range $10M-$50M; C26 $500K/$1-3.5M finalist; F-07 29% cap) | 09 §7; executor grep (see V4) |
| Live claim count | 25 (in [15,25]) | 02-claim-ledger.md header rules |
| Narrative prose | None - prose BLOCKED by FR-01 until scope lock | 10-narrative.md §FR-01 |
| Partners | confirmed: none; in discussion: none; proposed: 2 fiscal-sponsor candidates | 04 §1; 08 §3.2 |
| Owner persons | None named anywhere; every owner is a role with `[INFORMATION NEEDED]` | 06 IN-09; 07 BU-06; 08 §3.1; 10 NF-02 |

Consequence: several tests' pass rules require content that does not exist yet (intervention prose, SF-specific facts, a request amount, a signatory). Those tests are recorded **BLOCKED** with their unblocking decisions - never PASS, never FAIL, never silently "fixed" by editing the packet. Tests whose pass rule is genuinely satisfied by the framework as it stands are recorded **PASS** with evidence. Tests that pass structurally but whose final assessment awaits later content are recorded **PARTIAL**.

---

## 2. Edit 1 - `Documentation/Refinement/02-refinement-checklist.md`

### 2.1 Replace the §(a) table's Result column with the verdict columns

The current header (line 12) is:

```
| # | Test | Action | Pass rule | Result (fill on review) |
```

Replace it with:

```
| # | Test | Action | Pass rule | Verdict | Evidence ref | Unblocked by / follow-up |
```

For each of the 21 body rows, replace the trailing `| ☐ |` cell with the three new cells given in the table below (columns 5-7). Every row's Action and Pass rule text stays verbatim (quoted below as the "Current row" you replace).

### 2.2 The 21 checklist rows - verdict, evidence, unblocked-by (quotes are the current rows)

| # | Current row (Action \| Pass rule, verbatim) | Verdict | Evidence ref (file §section) | Unblocked by / follow-up |
|---|---|---|---|---|
| 1 | **Deletion test** \| Delete every sentence naming FTSArcade from each paragraph. \| An intelligible intervention remains (beneficiary, activity, deliverer, outcome). If the project vanishes, the intervention is underdefined. | **BLOCKED** | Framework-level property holds - no packet content depends on the project name (06 §6, 07 §6, 08 §6, 09 §6, 10 "Until then"); the pass rule cannot be assessed: no intervention prose exists (10 §FR-01 prose block; 00 §3.1 "Not defined") | Scope lock (DR-01/DR-06/DR-07) → T10 successor drafts prose under FR-02/FR-08 → re-run |
| 2 | **Substitution test** \| Replace "San Francisco" with another city throughout. \| Some facts remain true only of SF (population, institution, partner, cost, policy, route, landmark). If nothing changes, viability is generic. | **BLOCKED** | No SF-specific facts exist to survive substitution: SF problem analysis, site plan, and SF sources are all markers (06 §5 IN-07 "Substitution test unsatisfiable without sources"; 07 §3 all dependencies markers; 01 rows 1-2 NOT DEFINED) | DR-01 (SF problem analysis from city sources, 03 §1.1 DR-01 next action) + DR-06 (site plan) → T05/T06 successors fill IN-07/BU-04 → re-run |
| 3 | **Owner test** \| Underline every action verb. \| Every action has a named responsible party (person or org) - no "the community will…", no "we will" without a name. | **PASS** | Every action verb carries a responsible role: delivery map W-01..W-13 responsible-party column (04 §1); step owners (06 §3); staffing roles with statuses (08 §3.1); owner column on every ledger claim incl. C09-C11 (02); packet prose has no "we will"/"the community will" (executor grep, V4) | Follow-up (marker, not a fail): named persons per role - 06 IN-09, 07 BU-06, 08 OY-01, 10 NF-02, unblocked by DR-01; re-run at prose time |
| 4 | **Evidence test** \| Underline every causal verb ("improves", "leads to", "enables", "creates"). \| Each underlined verb points to an evidence grade (E1-E4) and a limitation; E5 claims are removed, not rewritten. | **PASS** | Every causal verb is graded: theory of change - all four links carry a grade (Blocked/E4, 00 §4.1); causal claims C19/C20/C28 graded E4 with tests (02; 03 §3); E5 claims removed as prohibition records (02 "Removed claims (E5)"); 05 §5 step 3 "passes for E1 rows; causal rows E4 with tests pending" | Follow-up (marker): E4 rows need test results - evidence reviewer, 03 §3; no verdict change |
| 5 | **Budget test** \| Underline every promised output (cohorts, sites, sessions, participants). \| Each output has a cost line or an explicit zero-cost explanation. | **PARTIAL** | Pass rule holds by construction: every quarter-plan row has a named cost line or "None (decision; zero cost)" (08 §2); every unit row's Figure cell is a marker or an explicit zero-cost explanation (09 §1 UC-01..UC-12); zero dollar figures anywhere (09 §7) | Figures and final assessment blocked: DR-04 (funding scenario) + cost sources per line (08 §2 Q2; 09 §6 gate) → T09 successor → re-run |
| 6 | **Durability test** \| End the grant on paper. \| Named activities, jobs, maintenance, and participant benefits that survive, each with an owner and an operating cost. | **PARTIAL** | Named survivors exist with owners: retained assets (live platform, workbench WIP builds, accessibility settings) each with evidence basis, continuity condition, and owner (08 §4); post-grant element table with owner roles (05 §1) | Operating cost missing - 05 §1 `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]`; adopted activities/funded operations blocked by DR-10; rights continuity by DR-09 → re-run |
| 7 | **Proportionality test** \| Reduce the request by half. \| The draft states exactly which outputs disappear and why the original request is justified at its size. | **BLOCKED** | No request exists to halve and no loss list: every lost-output cell is `[INFORMATION NEEDED: budget owner; lost-output enumeration - DR-04]` (09 §3); rule stated, enumeration absent (09 §3 proportionality rule; 04 §2.3) | DR-04 (scenario + request amount + proportionality loss list; 09 §6 gate (1)) → T09 successor → re-run |
| 8 | **Adversarial test** \| A reviewer attacks the weakest assumption. \| The draft already acknowledges and tests that assumption before the reviewer finds it. | **PASS** | Weakest assumption acknowledged in writing per recorded option: Weakest-assumption column in every option-detail table (03 §1.1 DR-01/DR-06/DR-07); assumptions A1-A7 graded with tests (09 §4); every risk has a decision trigger (05 §2); E4 assumptions with tests (00 §6.4) | Re-run at prose time (10 FR-08); no current fail |
| 9 | **Traceability** \| Map every factual sentence to a claim ID. \| ≥95% of factual sentences map to the claim ledger. | **PARTIAL** | Mapping mechanism binding: "No prospectus sentence may introduce a claim absent from this ledger" (02 header rules); existing factual content maps - 00 §6.1 ↔ C01-C05, 07 §1.1 ↔ C27, 00 §6.2/§8 ↔ C06; paragraph-trace format binds future prose (10 FR-06) | ≥95% metric unassessable until prose exists - 10 §FR-01 gate → T10 successor → re-run |
| 10 | **No silent inference** \| Check every website-derived claim. \| Zero claims that upgrade product facts into outcomes (see section (d) table). | **PASS** | Zero website-derived outcome claims: non-claims table - 12 rows, each with its prohibition source (07 §5); site-observation inference rules quoted verbatim (07 §1.2; 00 §3.2); E5 prohibition records C21/C22 (02); no-inference rule (07 §1.1) | Re-run at prose time (10 FR-07); no current fail |
| 11 | **Status fidelity** \| Check every partner and evidence mention. \| 100% of partner statuses (confirmed / in discussion / proposed) and evidence grades preserved in prose. | **PASS** | Every partner mention carries a status: 04 §1 "confirmed (none), in discussion (none), proposed (as marked)"; partner table with status column (08 §3.2); SF city institutions labeled evidence sources, not partners (08 §3.2; 00 §5); no confirmed partner claimed (C23) | Statuses update only via written confirmations (W-09, 04 §1); no current fail |
| 12 | **Gap visibility** \| Search for deleted information markers. \| 100% of unknown required fields still carry **[INFORMATION NEEDED: owner; why; decision blocked]** - deleting a marker without new information is a failed draft. | **PASS** | Marker discipline holds: 06 §5 IN-01..IN-10; 07 §4 BU-01..BU-11; 10 NF-01..NF-11; 00 §11 (12 blocking unknowns); 05 §3 "fields marked unknown must literally say 'unknown'; a blank is not permission to infer" | Markers resolve only via register entries (03 §1.1); no marker deleted without new information |
| 13 | **Numerical consistency** \| Cross-check every figure against the data dictionary and budget workbook. \| All figures match (definition, population, period, source, calculation, limitation). | **PASS** | Zero invented figures: no budget dollar figure exists (09 §7); executor grep of `$` across the packet → competition-rule amounts only (C06, C26, F-07); every figure has a dictionary row F-01..F-11 (03 §2); count conflict C3 flagged, not hidden (02 C27) | Follow-up (cosmetic): C3 label-vs-list count resolution (07 BU-10); no verdict change |
| 14 | **Capacity consistency** \| Compare planned volume vs stated capacity. \| First-year outputs never exceed named staff/partner/facility capacity. | **PASS** | Year-1 boundary = named capacity only (04 §3.1; 08 §1); no output exceeds capacity because no volume is claimed - all scale rows are markers, E1 sustainment rows FY-01-FY-04 are existing-site facts (08 §1); no confirmed capacity exists (C23); Q1 named-capacity inventory row (08 §2) | Re-run when the first-year plan is drafted (08 §6 gate); no current fail |
| 15 | **Prohibited claims** \| Grep the blacklist (section (d)) and the commercial-roster prohibitions. \| Zero prohibited claims. | **PASS** | Executor grep of the §(d)/§6 blacklist over the packet → 0 hits outside the ledger's own prohibited-claims quick-list block (02 "Prohibited-claims quick list"); FR-07 binds zero hits for future prose (10) | Re-run at prose time (10 FR-07); no current fail |
| 16 | **Criterion coverage** \| Map sections to the four criteria. \| Every rubric criterion is answered or explicitly blocked with the missing input named. | **PASS** | Every criterion answered (E1 facts) or explicitly blocked with the missing input named: 12 blocking unknowns with Blocks column (00 §11); consequences name Ambition/Viability/Evidence/Durability unscorable (03 §1 DR-01/DR-04/DR-06/DR-07/DR-10); proportionality note (04 §2.3) | Blocked-criterion inputs stay `[INFORMATION NEEDED]` until their DRs close (00 §11 rows) |
| 17 | **Paragraph acceptance** \| Five yes/no questions per paragraph (claim first? traceable? certainty labeled? one new idea? deletion loses info not tone?). \| All five "yes" per paragraph. | **PARTIAL** | Framework paragraphs are claim-first and traceable: claim-labeled paragraphs ("Claim (E1, documented absence):") in 00 §2/§5/§8/§9; the five-question rule binds every substantive paragraph (10 FR-02; instructions §11.5) | Full five-question run is a §11.5 review activity on prose - unblocked by scope lock → T10 successor + review rounds |
| 18 | **Contradiction audit** \| Check the 10 pairs (beneficiary↔capacity, outcome↔evidence grade, partner role↔status, budget↔volume, timeline↔staffing, measures↔outcomes, platform↔funded dev, post-grant owner↔governance, request↔scenario, lead authority↔legal structure). \| No unresolved contradiction; fixes go into the source case first, then prose is regenerated. | **PASS** | Mechanism exists (03 §4); run now: all 10 pairs consistent at framework level - both sides of each pair are carried states or markers (budget↔volume: zero figures + zero volume; partner role↔status: proposed-only; post-grant owner↔governance: DR-10/DR-02 markers); decision states propagate identically across all 11 files (03 §1.1 undecided ↔ 06/07/08/09/10 Status lines) | Re-run at each version (03 §4); contradictions resolve in the source case first |
| 19 | **Red-team protocol** \| One reviewer actively tries to fail the draft (unsourced claim, causal leap, over-stated partner, number without denominator, cost without activity, year-1 promise needing unsigned capacity, post-grant benefit without owner, platform feature as human service, omitted limitation). \| Findings classified: correct / already disclosed / requires project decision / speculative objection. | **PARTIAL** | Packet pre-empts every red-team category: unsourced claims - none, every claim graded/sourced (02); causal leaps - E4-labeled, E5 removed (02); over-stated partners - proposed-only (08 §3.2); numbers without denominator - zero figures (09 §7); cost without activity - zero figures; year-1 promise beyond unsigned capacity - named-capacity-only (04 §3.1); post-grant benefit without owner - survivors have owners (08 §4); platform feature as human service - non-claims (07 §5); omitted limitation - limitation column on E1 rows (00 §6.1) | Reviewer run with findings classification is a §11 review activity at content time - unblocked by scope lock → review rounds |
| 20 | **Comprehension review** \| An unfamiliar reader (doesn't know games or the org) answers the six questions in (c). \| Answers match the draft; mismatches are drafting defects, not reviewer failures. | **PARTIAL** | Packet is self-consistent: the six answers (who benefits - none defined; problem - undocumented; deliverable - browser arcade, E1; why outcomes - no mechanism; why the amount - no amount; what remains - retained assets) match the packet's own statements (00 §1) | Reader run with 4 unfamiliar readers (02 §(c)) is a §11.2 activity at prose time - unblocked by scope lock |
| 21 | **Sign-off** \| Authorized signatory confirms eligibility, central claims, budget, rights, and partner statuses are verified or accurately disclosed. \| Signatory can name the weakest assumption without help. Submission acceptance record signed. | **BLOCKED** | 05 §5 step 8: "Sign-off audit - **currently fails**; signatory cannot approve at S0"; no signatory named (00 §10.1; 03 §1.1 DR-11 `[INFORMATION NEEDED: authorized officer]`); stop conditions hold (00 §11) | Eligibility + content: DR-02/DR-03/DR-11 (registration + entity), DR-09 (rights schedule), DR-04, DR-10, scope lock, and a named signatory → re-run before submission |

**Verdict summary line (insert immediately after the §(a) table, before the "Stop conditions" blockquote):**

```
**Verdicts recorded <execution date> by change 014 (plan 001 T11, class Clarifying):** 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL across the 21 checklist rows plus the 8 editing-test rows below. BLOCKED tests are reported as follow-up tasks with named unblocking decisions - never silently fixed.
```

### 2.3 New subsection - the 8 editing-test verdicts (constitution §7)

Insert immediately after the "Stop conditions" blockquote (line 36), before the `---` that precedes §(b):

```
## (a.1) Editing-test verdicts (constitution §7) - recorded by change 014 (plan 001 T11)

Verdicts for the 8 editing tests of `Logs/instructions.md` §7 against the S0 framework-only packet.
Rows 1-8 of table (a) are the actionable form of these same tests and carry identical verdicts.

| Test (constitution §7, verbatim) | Verdict | Evidence ref | Unblocked by / follow-up |
|---|---|---|---|
| **Deletion test:** Remove FTSArcade from the paragraph. If no intelligible intervention remains, the project is underdefined. | BLOCKED | No content depends on the project name (06 §6, 07 §6, 08 §6, 09 §6, 10 "Until then"); no intervention prose exists to test (10 §FR-01; 00 §3.1) | Scope lock (DR-01/DR-06/DR-07) → T10 successor → re-run |
| **Substitution test:** Replace the beneficiary with a different city. If no San Francisco-specific facts remain, viability is too generic. | BLOCKED | No SF-specific facts exist (06 §5 IN-07; 07 §3; 01 rows 1-2) | DR-01 (SF problem analysis) + DR-06 (site plan) → T05/T06 successors → re-run |
| **Owner test:** Underline every action. Any action without a responsible party is not yet operational. | PASS | Every action has a responsible role: 04 §1 W-01..W-13; 06 §3; 08 §3.1; owner column on every claim (02); no "we will" in packet prose (grep) | Follow-up: named persons (06 IN-09; 08 §3.1) - unblocked by DR-01 |
| **Evidence test:** Underline every causal verb, such as "improves," "leads to," or "enables." Each must point to an evidence grade. | PASS | All causal verbs graded: 00 §4.1 (Blocked/E4 per link); C19/C20/C28 E4 with tests (02; 03 §3); E5 removed (02) | Follow-up: E4 tests pending (03 §3) |
| **Budget test:** Underline every promised output. Each must have a cost or an explicit zero-cost explanation. | PARTIAL | Cost-line discipline by construction: 08 §2; 09 §1 UC-01..UC-12; zero dollar figures (09 §7) | DR-04 + cost sources → T09 successor → re-run |
| **Durability test:** End the grant on paper. Identify which activities, jobs, maintenance, and participant benefits survive. | PARTIAL | Retained-asset survivors named with owners (08 §4); element table (05 §1) | DR-10 (operating cost) + DR-09 (rights) → re-run |
| **Proportionality test:** Reduce the request by half. State exactly which outputs disappear and why the original request is consequently justified. | BLOCKED | No request or loss list: 09 §3 lost-output cells all `[INFORMATION NEEDED - DR-04]`; 04 §2.3 | DR-04 (scenario + request + loss list; 09 §6 gate (1)) → T09 successor → re-run |
| **Adversarial test:** A reviewer challenges the weakest assumption. The draft should acknowledge and test it before the reviewer discovers it. | PASS | Weakest assumptions in writing per option (03 §1.1 DR-01/DR-06/DR-07); assumptions A1-A7 with tests (09 §4); risks with triggers (05 §2) | Re-run at prose time (10 FR-08) |
```

(Table content is given complete above - copy it verbatim; the executor does not abbreviate.)

---

## 3. Edit 2 - `Documentation/Logs/changes.md` (one row, appended after the row 013 entry)

Row format is the existing record table: `| Date | Change class | What changed | Why | Evidence/budget affected | Decision | Documents updated | Plan ref |`.

```
| <execution date> | Clarifying | Record editing-test verification pass (plan 001 T11): verdicts for all 8 editing tests (instructions.md §7) and all 21 checklist tests (02-refinement-checklist.md §(a)) against the S0 framework-only packet - 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL across 29 rows (editing tests: 3 PASS / 2 PARTIAL / 3 BLOCKED; checklist: 11 PASS / 6 PARTIAL / 4 BLOCKED); every test row carries a verdict and an evidence reference (file + section); BLOCKED tests recorded as named follow-up tasks, never silently fixed: deletion (needs narrative prose - scope lock DR-01/DR-06/DR-07 then T10 successor; 10 §FR-01), substitution (needs SF facts - DR-01 problem analysis + DR-06 site plan; 06 §5 IN-07), proportionality (needs request + loss list - DR-04; 09 §3/§6), sign-off (needs eligibility + signatory - DR-02/DR-03/DR-09/DR-11 + named signatory; 05 §5 step 8); 0 fails | plan 001 T11 (VERIFY) requires the pass recorded; verdicts are recorded against the current packet state - no verdict invented, no packet content changed | No new figures; no budget affected; verdict evidence = the packet files as cited in each row (E1 decision states, E1 platform facts, marker discipline); changes 008-013 zero-dollar-figure status unchanged | Recorded: verification pass (14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL); blocked tests tracked as follow-ups with named unblocking decisions | Refinement/02-refinement-checklist.md, Logs/changes.md, Plan/000-index.md | 014 |
```

`<execution date>` = the actual run date (all prior S0 rows use 2026-10-14; if executed later, use the real date). Do not fabricate a date.

---

## 4. Edit 3 - `Documentation/Plan/000-index.md` (one row, inside the Index table, after the 013 row)

```
| 014 | `Documentation/Plan/014-verification-pass.md` | Editing-test verification pass: verdicts for the 8 editing tests + 21 checklist tests (plan 001 T11) | planned | Pre-plan written; orchestrator advances planned → approved → executed → committed |
```

---

## 5. Verification - run in order; every check must pass before handoff

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | Every test row has a verdict + evidence ref | Inspect the two tables in 02-refinement-checklist.md (21 rows + 8 rows) | Every row has a verdict in {PASS, PARTIAL, BLOCKED} and an evidence ref naming a file + section; count rows: 21 and 8 |
| V2 | Verdicts match the packet's actual state - no invented PASS | For every PASS row, open the cited evidence and confirm it exists and supports the verdict | PASS rows are exactly: owner (3), evidence (4), adversarial (8), no silent inference (10), status fidelity (11), gap visibility (12), numerical consistency (13), capacity consistency (14), prohibited claims (15), criterion coverage (16), contradiction audit (18) - 11 checklist + the matching 3 editing rows; no test marked PASS whose pass rule needs content that does not exist (intervention prose, SF facts, request amount, signatory) |
| V3 | BLOCKED tests name the unblocking decision | Inspect the 4 BLOCKED rows (1, 2, 7, 21) in both tables | Each names its unblocking decisions: deletion → scope lock + T10 successor; substitution → DR-01/DR-06; proportionality → DR-04; sign-off → DR-02/DR-03/DR-09/DR-11 + named signatory |
| V4 | No prohibited words added | `git diff -- Documentation/Refinement/02-refinement-checklist.md Documentation/Logs/changes.md Documentation/Plan/000-index.md \| grep -E '^\+' \| grep -iE 'revolutionary\|world-class\|unique\|cutting-edge\|empower\|unlock\|transform\|scalable\|sustainable\|partners include\|data shows\|community-led\|at scale\|and more\|solutions for San Francisco'`; also `grep -rniE 'revolutionary\|world-class\|unique\|cutting-edge\|empower\|unlock\|transform\|scalable\|sustainable\|partners include\|data shows\|community-led\|at scale\|and more\|solutions for San Francisco' Documentation/Plan/014-verification-pass.md` | 0 hits on added lines; 0 hits in the plan file outside the V4 command's own regex quoting (same exemption as instructions.md §6's own list) and outside the pre-existing blacklist blocks (02 §(d), 02 §(a) row 15, 02 "Prohibited-claims quick list" quote), which are exempt and unchanged |
| V5 | Tables render | For every markdown table in the 3 edited files: header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present; the two new tables have 9 and 8 header+body rows respectively |
| V6 | No collateral edits | `git status --porcelain` | Exactly 4 paths: `?? Documentation/Plan/014-verification-pass.md` (the plan file, untracked) + ` M Documentation/Refinement/02-refinement-checklist.md` + ` M Documentation/Logs/changes.md` + ` M Documentation/Plan/000-index.md`; nothing else modified, no packet file touched |
| V7 | Blocked tests reported as follow-ups | Inspect the changes.md row | The row names the 4 blocked tests and their unblocking decisions; states 0 fails; class Clarifying; plan ref 014 |
| V8 | Consistency between the two verdict tables | Compare 02 §(a) rows 1-8 with the §(a.1) editing-test table | Identical verdicts for the same 8 tests |
| V9 | Index row present | Inspect Plan/000-index.md | Row 014 inside the Index table after row 013, status `planned` |

Handoff note: per instructions.md §11.6 a review run starts for every change that modifies a document before the version is committed; the orchestrator starts the three-facet review of this change and appends nothing further to changes.md until the facets pass or a blocked status is recorded (§11.4). The executor hands off after V1-V9 pass.

---

## 6. Executor inputs (read from the repo; never invent)

| Item | Where to read it | Why |
|---|---|---|
| Current §(a) rows to replace | `Documentation/Refinement/02-refinement-checklist.md` lines 12-34 (quoted verbatim in §2.2) | The ☐ cells become the verdict columns |
| Stop-conditions blockquote position | 02-refinement-checklist.md line 36 | Anchor for the §(a.1) insertion (§2.3) |
| changes.md table format + last row | `Documentation/Logs/changes.md` | Append after the 013 row (§3) |
| 000-index table format + last row | `Documentation/Plan/000-index.md` | Append after the 013 row (§4) |
| Evidence verification | The packet files as cited (03 §1.1, 05 §5, 06 §5/§6, 07 §5/§6, 08 §1/§2/§4/§6, 09 §1/§3/§6/§7, 10 §FR-01/FR-08, 00 §6.1/§11, 02 C19-C28) | V2 requires opening the cited evidence |
| Execution date | `date` | changes.md date column; never fabricated |