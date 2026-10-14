# 010 - Claim Ledger Build-out: 25 Claims (plan 001 task T07)

> **For Hermes:** Execute this plan with one execute agent. The executor edits exactly three files (`Prospectus/02-claim-ledger.md`, `Logs/changes.md`, `Plan/000-index.md`), never commits, and reports the verified claim count. The orchestrator reviews, commits once (`docs(grant): claim ledger build-out to 25 claims (T07)`), and flips the 000-index row through the lifecycle.

**Goal:** Extend `Documentation/Prospectus/02-claim-ledger.md` from 24 table rows to a claim table of **25 live claims (E1-E4)** - the top of plan 001 T07's 15-25 band - by preserving the existing live rows, relocating the three E5 prohibition records, and adding four claims (C25-C28) that cover the missing claim categories: competition-fact supplement with conflicts C2/C5, platform workbench facts with C3, and the candidate scope options as one E4 assumption claim.

**Scope - in:** `Documentation/Prospectus/02-claim-ledger.md` (extend), `Documentation/Logs/changes.md` (one row), `Documentation/Plan/000-index.md` (one row).
**Scope - out:** any other packet file (the evidence-register rows for C25-C28 in `03-registers.md` §3 are a recorded follow-up, not part of this change); the plan file itself (written by the pre-plan agent; the executor does not modify it); git commits (orchestrator-only, rule R2).

---

## 0. Current state and design decisions

### 0.1 Current ledger (read verbatim from the file on 2026-10-14)

Header line (lines 3-4) and claim table (lines 6-31):

```
**Version:** S0 · **Date:** 2026-10-14
**Rules:** No prospectus sentence may introduce a claim absent from this ledger. Four claim types only: **Factual** (observable/documented), **Operational** (what the project will do), **Causal** (why an activity should produce a result), **Forward-looking** (what is expected to continue/change later). Evidence grades: **E1** direct, **E2** closely comparable, **E3** analogous, **E4** plausible untested assumption (must include a test), **E5** insufficient (remove). A claim may move down in confidence, never up. Owners are roles - **named persons are required** (`[INFORMATION NEEDED: ...]`). Claim count: **24** (within the 15-25 band).

| ID | Claim | Type | Evidence status | Owner | Budget link | Rubric link | Permitted wording |
|---|---|---|---|---|---|---|---|
| C01 | FTSArcade is a publicly accessible, browser-based arcade at frymatic.us/FTSArcade. | Factual | **E1** - site retrieved 2026-10-14 | Technical owner (unnamed) | None (product fact) | Ambition (context only) | "As of October 14, 2026, the FTSArcade website offers browser-based arcade play at frymatic.us/FTSArcade." |
| C02 | The arcade lists 24 cabinets; 15 are live playable and 8 are labeled work-in-progress builds with pre-launch warnings. | Factual | **E1** - site, 2026-10-14 | Technical owner | None | Viability (context) | "The site lists 24 cabinets, of which 15 were playable live and 8 were labeled work-in-progress as of October 14, 2026." Limitation: site changes. |
| C03 | Play on the site is free; no account or purchase step was observed before gameplay. | Factual | **E1** - site observation | Technical owner | None | Ambition/Viability | "The games are offered free of charge and playable without an account." Limitation: this states a technical condition, not realistic access for any population. |
| C04 | The platform includes settings for audio routing, CRT visual treatment, a reduced-motion option, and browser-local preference storage. | Factual | **E1** - site, 2026-10-14 | Technical owner | Technology budget (if developed further) | Viability (accessibility context) | "The platform includes a reduced-motion accessibility option and browser-local preference storage." Limitation: no accessibility audit performed; no assistive-tech compatibility evidence. |
| C05 | The site makes no claims about beneficiaries, community programs, learning/employment outcomes, partners, or San Francisco delivery. | Factual (documented absence) | **E1** - site + export analysis | Evidence reviewer | None | Evidence | "The website does not itself establish San Francisco community outcomes." Use only as a gap statement, not as a virtue. |
| C06 | The competition deadline is October 15, 2026, 5:00 p.m. PT; registration closed September 11, 2026, 5:00 p.m. PT; awards range $10M-$50M; rubric = 4 equally weighted criteria; indirect costs ≤29% of direct costs; ≤25% of activities may benefit beyond SF city limits; each applicant peer-reviews 4 (up to 6) applications; submitted applications cannot be edited. | Factual | **E1** - rules + FAQ pages retrieved 2026-10-14 | Authorized officer | None (compliance) | All | State as competition facts with the source. |
| C07 | The team's registration status with the competition is not confirmed. | Factual (documented absence) | **E1** - no registration evidence in sources | Authorized officer | None | Eligibility | "Registration status is not confirmed as of October 14, 2026." If not registered: stop drafting; request an exception from boundless-sf@submittable.com in writing. |
| C08 | The legal entity behind FTSArcade, its jurisdiction, and tax status are not documented in available sources. | Factual (documented absence) | **E1** | Authorized officer | None | Eligibility | "The legal applicant is not yet documented." No entity claim may be made. |
| C09 | The team will identify an eligible Lead Organization that exercises actual legal and operational control of any award funds. | Operational | **E4** - no entity, sponsor, or written confirmation exists | Authorized officer | Legal/admin budget | Viability/Durability | "The project will be led by an eligible organization with actual control of funds; the lead is being determined." Not: "a sponsor will receive and pass through funds" (prohibited arrangement). |
| C10 | The team will define one San Francisco beneficiary population with inclusion/exclusion rules before drafting. | Operational | **E4** - population not defined | Program lead | Participant-support budget (once defined) | Ambition/Viability | "The beneficiary population will be defined as [population] in [geography]." Until defined: only the plan to define it may be stated. |
| C11 | The team will choose one intervention with a defined participant pathway before drafting. | Operational | **E4** - no pathway exists | Program lead | Activity budget | Viability | "The intervention and participant pathway are being defined; no activity claim is made." |
| C12 | The team can develop and install custom arcade cabinets on order. | Operational (capability) | **E4** - team assertion only; no portfolio, order, or reference documented | Technical owner | Revenue model (not grant request) | Viability (capacity, if evidenced) | "The team reports capability to develop and install custom cabinets; evidence of prior builds is pending." Test: documented builds, orders, or letters of intent. |
| C13 | The team can develop custom games for cabinets. | Operational (capability) | **E4** - live games exist (C02) but no commissioned/custom delivery documented | Technical owner | Revenue model | Viability | "The team develops games for the arcade; commissioned custom development is not yet demonstrated." |
| C14 | Businesses will be able to order arcade installations. | Operational (forward plan) | **E4** - demand unverified; no orders, LOIs, or pipeline documented | Program lead | Revenue model | None (commercial, not grant case) | "Business orders are a proposed commercial offering, subject to confirmed demand." Test: orders or LOIs. |
| C15 | Games can potentially incorporate licensed San Francisco landmarks and businesses. | Operational (proposed) | **E4** - no permissions, licenses, or agreements exist | Rights owner | None | Ambition (only if mechanism defined) | "Featuring specific landmarks and businesses would require permission from their owners or responsible authorities; none has been obtained." |
| C16 | QR codes can connect gameplay to separately approved partner offers (e.g., ride referrals). | Operational (proposed) | **E4** - no partner agreements; export marks this as a commercial mechanism, not a charitable outcome | Program lead | None | None | "QR-linked partner offers are a proposed commercial mechanism requiring separate approvals." Not: improved mobility or convenience as a public benefit. |
| C17 | An internal game economy is under consideration. | Operational (proposed) | **E4** - needs a lawful charitable purpose and strong controls | Budget owner | Revenue model | Durability (candidate) | "An in-game economy is being investigated; it would require a documented charitable purpose and controls against private benefit." |
| C18 | Commercial revenue (cabinet sales, ad space, referrals) is being investigated as one post-grant sustainability mechanism. | Forward-looking | **E4** - no revenue, payer, or operating-cost model exists | Budget owner | Post-grant budget | Durability | "Commercial revenue is being investigated as one sustainability mechanism." Not: "the project will be sustainable through commerce." |
| C19 | The charitable frame - publicly accessible cultural/recreational installations documenting and increasing engagement with specific SF places, with commerce funding free public access - is a hypothesis to be tested, not an achieved result. | Causal (frame) | **E4** - no beneficiary, site plan, access rules, or evidence; every arrow in the chain unproven | Decision owner | All grant lines (once defined) | Ambition/Evidence | "The project will test whether publicly accessible game installations increase engagement with specific San Francisco places." Never state the frame's effects as fact. |
| C20 | Advertising/upselling will remain subordinate to a defined public purpose with only incidental private benefit. | Causal | **E4** - selection rules, access rules, and controls not designed; for-profit leads face IRC §4945(h) expenditure responsibility | Decision owner + counsel | Legal/admin budget | Ambition/Durability | "Advertising and commerce would remain subordinate to public access under rules that are being designed." |
| C21 | Playing the games produces learning, employment, wellbeing, or community outcomes. | Causal | **E5 - removed**; product engagement must not be relabeled as outcomes; no evidence exists | Evidence reviewer | None | Evidence | **PROHIBITED.** Permitted alternative: "The project will test whether [defined outcome] follows from [defined intervention]; engagement metrics alone do not establish it." |
| C22 | The project will revitalize old buildings, increase running/use of public routes, popularize San Francisco, produce economic development, or improve mobility via QR-linked rides. | Causal/Forward-looking | **E5 - removed**; the export explicitly forbids these without beneficiary, mechanism, evidence, owner, and budget | Evidence reviewer | None | Evidence/Ambition | **PROHIBITED** unless each claim gains a beneficiary, mechanism, evidence grade, delivery owner, and budget. Running-route data: `[INFORMATION NEEDED: research lead; source, date, permissions, relevance; no claim may use it]`. |
| C23 | The team has existing San Francisco presence or delivery capacity (people, locations, partners). | Factual | **E1 (absence)** - none documented; no confirmed partners | Program lead | Delivery budget | Viability | "No San Francisco delivery capacity or confirmed partner exists as of October 14, 2026; the plan to establish presence is [sequence]." Fiscal-sponsor candidates are proposed only. |
| C24 | Ownership and licensing of the platform's code, art, audio, and third-party components are documented and sufficient for the proposed use. | Factual | **E5 - not documented**; export flags IP review as important for a game platform; rules require appropriate rights for third-party material | Rights owner | Legal/admin budget | Eligibility/Durability | No claim may be made until the rights schedule (`05-durability-risks-rights.md`) is completed. `[INFORMATION NEEDED: rights owner; required to confirm the lead can lawfully use all assets; blocks submission - DR-09]` |
```

### 0.2 Band arithmetic and counting rule

- Current table: **24 rows** = **21 live claims (E1-E4:** C01-C20, C23**) + 3 E5 prohibition records (C21, C22, C24)**.
- The ledger's own grade definitions: E5 = "insufficient (remove)" - an E5 row is a prohibition record, **not a claim**. Plan 001 T07's band [15,25] therefore counts claims (E1-E4); E5 records are excluded from the count.
- Design consequence: keeping all 24 rows in the claim table would leave room for at most one addition. This change instead **relocates** the three E5 records (verbatim text) to a new "Removed claims (E5)" bullet section directly below the table, so the claim table holds exactly the claims. The file keeps exactly **one** pipe-table, which keeps plan 001's count command (`grep -c '^|'` adjusted for header rows) valid: header + separator + **25 rows** = 27 pipe lines, minus 2 = **25**.
- After the change: **25 live claims, in [15,25]** (top of band), plus 3 E5 records preserved below as prohibition records.

### 0.3 What the new rows cover (T07 claim mix)

| New row | Category | Grade | Conflict ref | Trace |
|---|---|---|---|---|
| C25 | Competition fact: foreign-entity eligibility + fiscal sponsorship | E1 | C2 | facts-pack #15, #16, #18, #19 (rules §1/§2, FAQ, readiness tool) |
| C26 | Competition fact: finalist stage / project-development funding | E1 | C5 | facts-pack #4, timeline table (rules §13.8, /timeline, LFC open-call page) |
| C27 | Platform fact: workbench WIP builds + cabinet-count labels | E1 | C3 | facts-pack §(d) facts 4, 6, 7, 8 (frymatic.us/FTSArcade) |
| C28 | E4 assumption claim: candidate scope options (DR-01/DR-06/DR-07) recorded, not chosen | Causal (hypothesis) E4, with test | - | 03-registers.md §1.1 option details; 06-participant-pathway.md §1; 07-platform-boundary.md §6 |

Conflict cross-references land on: **C1 + C4** on C06 (deadline widget; full-Application-PDF link 404 - both affect application-mechanics facts), **C3** on C02 (label "8 ON THE BENCH" vs the 9 WIP entries listed; C27 records the detail), **C2** on C25, **C5** on C26, **C6** on C23 (the only SF-ecosystem row; its §(e) sources are archived/unverifiable live - re-verify before any SF-ecosystem quote).

### 0.4 What is deliberately NOT added

- No claim from the 07-platform-boundary §5 non-claims list (learning gains, employment outcomes, community formation, city popularity, revitalization, economic development, mobility, equitable business benefit, user counts/play metrics, engagement-as-outcome, SF-benefit/partner-list/funding-model claims). C28 names the DR-07 option "community connection" only as a register option label, never as an asserted outcome.
- No duplication of C19 (the DR-06 frame hypothesis stays C19; C28 covers the DR-01/DR-06/DR-07 option sets and the outcome-testing commitment) and no duplication of C06's bundled competition mechanics (deadline, registration, award range, 29% indirect, 25% rule, peer review, no-edit - all already in C06).
- No ungraded causal verbs: every causal/forward-looking row carries an E1-E5 grade (V4).

---

## 1. Exact edits - `Documentation/Prospectus/02-claim-ledger.md`

### 1.1 Header line (claim-count sentence)

Replace the sentence `Claim count: **24** (within the 15-25 band).` (end of line 4) with:

`Claim count: **25** (within the 15-25 band). The band counts claims graded E1-E4; E5 records (C21, C22, C24) are prohibition records - "E5 insufficient (remove)" - listed under "Removed claims (E5)" below and not counted.`

The rest of lines 3-4 (version, date, rules) is unchanged.

### 1.2 Table header and separator (8 columns -> 11 columns)

Replace:

```
| ID | Claim | Type | Evidence status | Owner | Budget link | Rubric link | Permitted wording |
|---|---|---|---|---|---|---|---|
```

with (column order maps the T07 outline `claim # | claim | evidence grade | source URL | status | conflict ref` onto the ledger's existing columns):

```
| ID | Claim | Type | Evidence status | Source URL | Source status | Conflict ref | Owner | Budget link | Rubric link | Permitted wording |
|---|---|---|---|---|---|---|---|---|---|---|
```

### 1.3 Preserved live rows C01-C20 and C23: insert three cells

For each of the 21 preserved live rows, insert the three cells `Source URL | Source status | Conflict ref` **immediately after the Evidence status cell** (i.e. before the existing Owner cell), preserving every existing cell verbatim. New cell values:

| ID | Source URL (inserted) | Source status (inserted) | Conflict ref (inserted) |
|---|---|---|---|
| C01 | https://frymatic.us/FTSArcade (fetched live 2026-10-14) | verified | - |
| C02 | https://frymatic.us/FTSArcade (fetched live 2026-10-14) | verified (label-vs-list) | C3 |
| C03 | https://frymatic.us/FTSArcade (fetched live 2026-10-14) | verified | - |
| C04 | https://frymatic.us/FTSArcade (fetched live 2026-10-14) | verified | - |
| C05 | https://frymatic.us/FTSArcade (fetched live 2026-10-14); Reference export analysis | verified (documented absence) | - |
| C06 | https://boundless-sf.leverforchange.org/rules; /faq; /timeline (retrieved 2026-10-14) | verified (conflicts on related pages) | C1; C4 |
| C07 | https://boundless-sf.leverforchange.org/timeline (registration deadline); no registration evidence located | verified (documented absence) | - |
| C08 | None - documented absence across all available packet sources | verified (documented absence) | - |
| C09 | None - team assertion; no entity, sponsor, or written confirmation exists | E4 - no evidence located | - |
| C10 | `03-registers.md` §1.1 DR-01 (options recorded, not chosen) | E4 - population not defined | - |
| C11 | `06-participant-pathway.md` §3 (framework; step cells placeholders) | E4 - no pathway exists | - |
| C12 | https://frymatic.us/FTSArcade (live games exist); capability claim = team assertion | E4 - no portfolio, order, or reference | - |
| C13 | https://frymatic.us/FTSArcade (live games exist); delivery claim = team assertion | E4 - no commissioned delivery documented | - |
| C14 | None - team assertion; no orders, LOIs, or pipeline | E4 - demand unverified | - |
| C15 | None - team assertion; no permissions, licenses, or agreements | E4 - no permissions or licenses | - |
| C16 | None - team assertion; no partner agreements | E4 - no partner agreements | - |
| C17 | None - under consideration | E4 - under consideration | - |
| C18 | None - investigation only; no revenue, payer, or operating-cost model | E4 - no model exists | - |
| C19 | `../Reference/we're looking to prepare a grant application for h.md` §"Choose a charitable frame"; `03-registers.md` §1.1 DR-06 (option a, recorded not chosen) | E4 - hypothesis, unproven | - |
| C20 | `../Reference/we're looking to prepare a grant application for h.md` §"Commercial-benefit test"; `../Research/facts-pack.md` #17 (expenditure responsibility, E1) | E4 - controls not designed | - |
| C23 | `01-source-case.md`; `03-registers.md`; `../Research/facts-pack.md` §(e) (no confirmed partner documented) | E1 (absence); C6 affects the SF source base | C6 |

**Worked example (C01, full row after the edit):**

```
| C01 | FTSArcade is a publicly accessible, browser-based arcade at frymatic.us/FTSArcade. | Factual | **E1** - site retrieved 2026-10-14 | https://frymatic.us/FTSArcade (fetched live 2026-10-14) | verified | - | Technical owner (unnamed) | None (product fact) | Ambition (context only) | "As of October 14, 2026, the FTSArcade website offers browser-based arcade play at frymatic.us/FTSArcade." |
```

**Worked example (C06, full row after the edit):**

```
| C06 | The competition deadline is October 15, 2026, 5:00 p.m. PT; registration closed September 11, 2026, 5:00 p.m. PT; awards range $10M-$50M; rubric = 4 equally weighted criteria; indirect costs ≤29% of direct costs; ≤25% of activities may benefit beyond SF city limits; each applicant peer-reviews 4 (up to 6) applications; submitted applications cannot be edited. | Factual | **E1** - rules + FAQ pages retrieved 2026-10-14 | https://boundless-sf.leverforchange.org/rules; /faq; /timeline (retrieved 2026-10-14) | verified (conflicts on related pages) | C1; C4 | Authorized officer | None (compliance) | All | State as competition facts with the source. |
```

### 1.4 Relocate E5 records C21, C22, C24

Delete the three rows C21, C22, C24 from the claim table (no blank line may open between C20 and C23; the table body stays contiguous). Immediately after the table (i.e. after row C23 until this step, after row C28 once 1.5 is applied - see Section 1.5 for order), insert a new section before `## Prohibited-claims quick list`:

```
## Removed claims (E5) - prohibition records

These rows are E5 - "insufficient (remove)" - and are **not claims**; they are preserved verbatim as prohibition records and are excluded from the claim count.

- **C21 (E5 - removed; prohibited).** Claim: "Playing the games produces learning, employment, wellbeing, or community outcomes." Type: Causal. Evidence status: **E5 - removed**; product engagement must not be relabeled as outcomes; no evidence exists. Owner: Evidence reviewer. Budget link: None. Rubric link: Evidence. Permitted wording: **PROHIBITED.** Permitted alternative: "The project will test whether [defined outcome] follows from [defined intervention]; engagement metrics alone do not establish it."
- **C22 (E5 - removed; prohibited).** Claim: "The project will revitalize old buildings, increase running/use of public routes, popularize San Francisco, produce economic development, or improve mobility via QR-linked rides." Type: Causal/Forward-looking. Evidence status: **E5 - removed**; the export explicitly forbids these without beneficiary, mechanism, evidence, owner, and budget. Owner: Evidence reviewer. Budget link: None. Rubric link: Evidence/Ambition. Permitted wording: **PROHIBITED** unless each claim gains a beneficiary, mechanism, evidence grade, delivery owner, and budget. Running-route data: `[INFORMATION NEEDED: research lead; source, date, permissions, relevance; no claim may use it]`.
- **C24 (E5 - not documented).** Claim: "Ownership and licensing of the platform's code, art, audio, and third-party components are documented and sufficient for the proposed use." Type: Factual. Evidence status: **E5 - not documented**; export flags IP review as important for a game platform; rules require appropriate rights for third-party material. Owner: Rights owner. Budget link: Legal/admin budget. Rubric link: Eligibility/Durability. Permitted wording: No claim may be made until the rights schedule (`05-durability-risks-rights.md`) is completed. `[INFORMATION NEEDED: rights owner; required to confirm the lead can lawfully use all assets; blocks submission - DR-09]`.
```

Content above is the verbatim content of the current C21/C22/C24 rows, reflowed as bullets; no wording is changed.

### 1.5 Append new rows C25-C28

Append the four rows **immediately after row C23's row** (before the `---` that closes the table section), keeping the table body contiguous - no blank line between C23 and C25 or between any new rows:

```
| C25 | Rules §1 list foreign entities as eligible Lead Organizations (categories 7 and 9) and permit fiscal sponsorship, with the fiscal sponsor exercising discretion and control over grant funds; the FAQ "Who can participate?" intro contradicts the Rules, so written confirmation from boundless-sf@submittable.com is required before any foreign-entity pathway is relied on. | Factual | **E1** - rules + FAQ + readiness pages retrieved 2026-10-14 | https://boundless-sf.leverforchange.org/rules (§1, §2); /faq; /organizationreadinesstool | verified (conflict C2) | C2 | Authorized officer | Legal/admin budget | Eligibility | "Rules §1 permit foreign entities as Lead Organizations (categories 7 and 9: IRS determination or 501(c)(3)/509(a)(1) equivalency, or a recognized foreign NGO engaged in 501(c)(3)-meaning charitable activities) and permit fiscal sponsorship; the fiscal sponsor must exercise discretion and control over grant funds (facts-pack #15, #16, #18). The FAQ intro contradicts the Rules (conflict C2); written confirmation from boundless-sf@submittable.com is required before relying on any foreign-entity pathway (facts-pack #19)." Not: assert foreign-entity eligibility without written confirmation. |
| C26 | Up to seven finalists are selected (by June 2027 per the FAQ); each receives a project development grant of up to $500,000 plus technical assistance, with the pool totaling $1-3.5 million; the LFC open-call page phrases the per-finalist range as $250,000-$500,000 (conflict C5); finalists' investment prospectus is due August 2027. | Factual | **E1** - rules §13.8 + timeline + LFC page retrieved 2026-10-14 | https://boundless-sf.leverforchange.org/rules (§13.8); /timeline; https://leverforchange.org/open-calls/boundless-san-francisco/ | verified (amount phrasing conflict C5) | C5 | Authorized officer | Project-development budget (if selected as Finalist) | All | "Up to seven finalists each receive a project development grant of up to $500,000 plus technical assistance; the pool totals $1-3.5 million; the LFC page phrases the range as $250,000-$500,000 (conflict C5); the investment prospectus is due August 2027." Not: assert a specific per-finalist amount without resolving C5. |
| C27 | The site's workbench lists 9 work-in-progress entries labeled "COMING SOON" and "WIP BUILD" with a warning dialog before play; the page label "8 ON THE BENCH" is internally inconsistent with the 9 entries listed (conflict C3); cabinet counts must be stated from the entry list, not from the label. | Factual | **E1** - site, 2026-10-14 | https://frymatic.us/FTSArcade (facts-pack §(d) facts 4, 6, 7, 8) | verified (label-vs-list conflict C3) | C3 | Technical owner | Technology budget (WIP completion) | Viability (context) | "The workbench lists 9 work-in-progress entries labeled 'COMING SOON' and 'WIP BUILD', each with a warning dialog before play; the page's '8 ON THE BENCH' label is internally inconsistent with the 9 listed entries (conflict C3); cabinet counts are stated from the entry list, not from the label." Limitation: site changes. |
| C28 | The candidate beneficiary options (DR-01 a-d), charitable frames (DR-06 a), and single public outcomes (DR-07 a-f) are recorded, not chosen, as of 2026-10-14; the project will test whether the chosen option's intended outcome follows from the defined intervention, measured by a pre-registered indicator at capability, progression, or system level; engagement metrics are never outcomes. | Causal (hypothesis) | **E4** - options recorded 2026-10-14, not chosen; no beneficiary, frame, or outcome is defined | `03-registers.md` §1.1 (DR-01/DR-06/DR-07 option details); `06-participant-pathway.md` §1; `07-platform-boundary.md` §6 | E4 - options not chosen | - | Program lead | All grant lines (once defined) | Ambition/Evidence | "The candidate options are recorded, not chosen; the project will test whether the chosen option's intended outcome follows from the defined intervention under a pre-registered indicator at capability, progression, or system level (DR-07 decision rule); engagement metrics are never outcomes." Not: state any candidate option's effect as fact. Test: pre-registered indicator per the DR-07 decision rule (baseline, target, instrument, collection timing, decision affected) once DR-01/DR-06/DR-07 close. |
```

**Order note (1.4 + 1.5):** apply 1.5 (append C25-C28 after C23) first, then 1.4 (delete C21/C22/C24 and insert the Removed-claims section after the table's closing `| C28 | ... |` row, before the `---`). Either order is acceptable as long as the final layout is: claim table rows C01-C20, C23, C25, C26, C27, C28 (contiguous) -> blank line -> `---` -> blank line -> `## Removed claims (E5) - prohibition records` (3 bullets) -> blank line -> `## Prohibited-claims quick list` (unchanged) -> `## Evidence-register linkage` (updated, 1.6).

### 1.6 Evidence-register linkage (bottom section)

Replace the sentence `C19 and C20 are the only causal claims currently graded E4 with tests; C21 and C22 are removed; C12-C18 are operational/forward-looking with tests to be defined by their owners.` with:

`C19, C20, and C28 are the causal claims graded E4 with tests; C21 and C22 are removed (see "Removed claims (E5)" above); C12-C18 are operational/forward-looking with tests to be defined by their owners. C25-C27 (E1 factual) and C28 (E4 causal) need evidence-register rows in `03-registers.md` §3; they are added when that file is next touched (follow-up, not this change).`

---

## 2. changes.md row (append after the last row; `Documentation/Logs/changes.md`)

One row; `\|` escapes pipes inside the What-changed cell (same convention as rows 008/009):

```
| 2026-10-14 | Clarifying | Claim ledger build-out (plan 001 T07): claim table unified to the T07 format (ID \| claim \| type \| evidence status \| source URL \| source status \| conflict ref \| owner \| budget link \| rubric link \| permitted wording); rows C01-C20 and C23 preserved verbatim with the three new cells filled; E5 prohibition records C21/C22/C24 relocated verbatim to a new "Removed claims (E5)" section (not claims - excluded from the count); rows added: C25 (foreign-entity eligibility + fiscal sponsorship; E1; conflict C2), C26 (finalist stage and project-development funding; E1; conflict C5), C27 (workbench WIP builds and cabinet-count labels; E1; conflict C3), C28 (candidate scope options recorded, not chosen; Causal E4 with test); conflict refs added: C1 + C4 on C06, C3 on C02, C6 on C23; evidence-register linkage updated (C19/C20/C28 are the causal E4 claims with tests) | plan 001 T07 (CONTENT) requires the ledger at 15-25 claims; the ledger held 24 rows (21 live claims E1-E4 + 3 E5 records), so the change adds the missing claim categories (competition-fact supplement with conflicts C2/C5, platform workbench facts with C3, scope-option assumption claim) and lands at the top of the band | **Claim count: 25 (in [15,25])** - executor-verified; E1 competition facts (rules §1/§2/§13.8, FAQ, timeline, LFC page - verified 2026-10-14); E1 platform facts (facts-pack §(d) facts 4/6/7/8); E4 scope-options claim (03-registers.md §1.1, E1 option records; hypothesis graded E4); conflict refs C1-C6 cross-referenced; no new dollar figures; no budget lines changed | No decision closed - scope options remain recorded, not chosen | Prospectus/02-claim-ledger.md, Logs/changes.md, Plan/000-index.md | 010 |
```

## 3. 000-index.md row (append after the row 009 row; `Documentation/Plan/000-index.md`)

```
| 010 | `Documentation/Plan/010-claim-ledger.md` | Claim ledger build-out: unified T07 columns, added C25-C28, live claim count 25 (plan 001 T07) | planned | Pre-plan agent wrote the plan file; orchestrator to approve, then execute | |
```

---

## 4. Verification - how the executor proves the change is correct

Run in order; every check must pass before handoff. All commands run from the repo root.

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | Claim count in [15,25] | `grep -c '^|' Documentation/Prospectus/02-claim-ledger.md` | Output **27**; minus 2 (header + separator) = **25 claim rows**, in [15,25]. The file must contain exactly one pipe-table (V6 confirms; the Removed-claims section is bullets). **Record `25` in the changes.md row (Section 2).** |
| V2 | Every claim has grade + source | `awk -F'|' '/^\| C[0-9][0-9] / {g=$5; gsub(/[* ]/,"",g); if (g !~ /^E[1-5]/) print "NO-GRADE: " $2; s=$6; gsub(/ /,"",s); if (s=="") print "NO-SOURCE: " $2}' Documentation/Prospectus/02-claim-ledger.md` | 0 lines printed (each of the 25 rows has an E1-E5 Evidence status and a non-empty Source URL cell) |
| V3 | Conflicts cross-referenced | `for c in 1 2 3 4 5 6; do awk -F'|' -v c="C$c" '/^\| C[0-9][0-9] / {if ($7 ~ c) f=1} END {if (!f) print "MISSING C" c}' Documentation/Prospectus/02-claim-ledger.md; done` | No MISSING lines. Expected mapping: C1+C4 on C06; C2 on C25; C3 on C02 + C27; C5 on C26; C6 on C23 |
| V4 | No ungraded causal verbs | `awk -F'|' '/^\| C[0-9][0-9] / {t=$4; gsub(/ /,"",t); g=$5; gsub(/[* ]/,"",g); if ((t ~ /Causal/ || t ~ /Forward/) && g !~ /^E[1-5]/) print "UNGRADED: " $2}' Documentation/Prospectus/02-claim-ledger.md` | 0 lines printed (C18 Forward E4; C19/C20/C28 Causal E4 - all graded) |
| V5 | No prohibited claims in new rows (07-boundary §5 non-claims list) | `awk -F'|' '/^\| C(25|26|27|28) / {print $2 " | " $3}' Documentation/Prospectus/02-claim-ledger.md | grep -icE 'learning|employment|revitaliz|popularity|economic development|mobility|equitable business|user counts|play metrics'` | Output **0**. (C28's option label "community connection" is a register option name, allowed - not a community-formation claim; "engagement metrics are never outcomes" is the DR-07 rule statement, allowed.) |
| V6 | Tables render (pipe counts + row contiguity) | `awk '/^\|/ {print gsub(/\|/, "")}' Documentation/Prospectus/02-claim-ledger.md | sort | uniq -c` | Output exactly `27 12` (27 pipe lines, all 12 pipes = 11 columns). No pipe lines outside the claim table. No blank line between the separator row and C01, between C20 and C23, or between C23 and C28 (inspect the block; a blank line inside the body strands rows) |
| V7 | No prohibited words (claim table + Removed-claims section) | `sed -n '1,/^## Prohibited-claims/p' Documentation/Prospectus/02-claim-ledger.md | grep -icE 'revolutionary|world-class|unique|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows'` | Output **0** (the file's own quick-list section, below the sed cutoff, is the only allowed occurrence) |
| V8 | No drafting boundary | `grep -niE 'dear|subject:|sincerely' Documentation/Prospectus/02-claim-ledger.md` | 0 hits (protocol R1; no email text introduced) |
| V9 | Git status exact file set | `git status --porcelain` | Exactly: ` M Documentation/Prospectus/02-claim-ledger.md`, ` M Documentation/Logs/changes.md`, ` M Documentation/Plan/000-index.md`, `?? Documentation/Plan/010-claim-ledger.md`. No other entries, no deletions |
| V10 | Plan index row | `grep -c '| 010 |' Documentation/Plan/000-index.md` | Output 1; the row's status is `planned` (orchestrator flips it through the lifecycle after review) |

---

## 5. Executor inputs (not derivable from this plan - read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| Exact cell text of the preserved rows C01-C20, C23 | `Documentation/Prospectus/02-claim-ledger.md` (live file) | Section 0.1 quotes are reference; the live file is authoritative for the verbatim cell text the executor preserves when inserting the three new cells |
| Current end of `changes.md` / `000-index.md` | `Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md` | Append Section 2 / Section 3 rows after the last row; do not modify existing rows |
| E1 fact wording for the new cells (C25-C27 source cells) | `Documentation/Research/facts-pack.md` (#15/#16/#18/#19; #4; §(d) facts 4/6/7/8; conflicts C2/C5/C3) | The new rows' text and source cells trace to these facts; if the executor quotes fact text, copy verbatim from facts-pack |

**Executor discipline:** (1) do not modify `Documentation/Plan/010-claim-ledger.md`; (2) do not reorder existing rows relative to this plan (V6 catches stranded rows); (3) do not silently resolve any `[INFORMATION NEEDED]` marker; (4) report any mechanical deviation (e.g. a pipe-count fix) as a flagged deviation in the handoff; (5) record the verified count `25` in the changes.md row.