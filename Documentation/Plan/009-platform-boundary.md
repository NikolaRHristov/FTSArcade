# 009 - Platform Boundary: What the Platform Is, Inside/Outside Split, Provider Map (T06)

> **For Hermes:** Execute this plan with an execute agent. Orchestrator reviews and commits once (`docs(grant): <change>`). This change creates `Documentation/Prospectus/07-platform-boundary.md` as a **structured boundary framework - not a draft boundary** - because DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided as of 2026-10-14** (`03-registers.md` §1.1). The executor writes the framework, tables, and placeholders exactly as specified in Section 2; **inventing any platform feature, provider, or promoted outcome is forbidden**.

**Goal:** Satisfy plan 001 task T06 (bucket CONTENT) by creating `Documentation/Prospectus/07-platform-boundary.md` - a STRUCTURED BOUNDARY FRAMEWORK document: (1) platform definition and function scope; (2) boundary table `inside platform | outside platform | provider of outside items`; (3) SF-ecosystem dependencies with source links; (4) boundary unknowns; (5) non-claims section; (6) decision-gate note - and appending the changes.md row and the 000-index.md row. No platform content is invented: inside cells carry only the E1 product facts from `facts-pack.md` §(d) verbatim; outside cells are `[INFORMATION NEEDED: ...]` markers; no gameplay-to-outcome claim is made anywhere.

**Change class: Clarifying.** Rationale (per `001-repo-scaffold.md` §0.2 and the T06 task detail): no scope change occurs - no option of DR-01/DR-06/DR-07 is chosen or redefined; the change adds missing information (the E1-grounded platform boundary framework and the propagated decision states) and creates one new packet document. This mirrors the Clarifying precedent of changes 004/005/006/007/008, which recorded undecided decision states and the pathway framework. Foundational would apply only if the decisions were made and changed scope; they are not. Operational would apply to delivery/budget numbers; the document adds none (zero dollar figures).

**Scope - in:** the 3 files listed in Section 1 (F2-F4) plus this plan file (F1, already written by the pre-plan agent).
**Scope - out:** choosing or recommending any option of DR-01/DR-06/DR-07; inventing platform features, providers, SF locations, or outcomes; edits to `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `04-delivery-and-budget.md`, `06-participant-pathway.md`, root `README.md`, `Documentation/Research/*`, `Documentation/Refinement/*`; drafting (protocol R1); commits (orchestrator-only, rule R2).

---

## 1. Target files (this change)

| # | Path | Action |
|---|---|---|
| F1 | `Documentation/Plan/009-platform-boundary.md` | This plan (already written by the pre-plan agent; no action) |
| F2 | `Documentation/Prospectus/07-platform-boundary.md` | **New file** (verified absent): the platform boundary framework - write the Section 2.2 content verbatim |
| F3 | `Documentation/Logs/changes.md` | Modify: append one row (class Clarifying, plan ref 009) after the plan-008 row (currently line 17) |
| F4 | `Documentation/Plan/000-index.md` | Modify: append row 009, status `planned`, after the plan-008 row (currently line 16) |

---

## 2. F2 - `Documentation/Prospectus/07-platform-boundary.md` (NEW FILE)

### 2.1 File-level rules (binding)

- Write the file exactly as the fenced content in §2.2: headers verbatim, tables verbatim, cell text verbatim, relative links only. Do not add, remove, or reword any section, row, cell, or marker.
- All owners are **roles** (per `03-registers.md` rules: "All owners are roles; named persons are `[INFORMATION NEEDED: ...]`"). No person's name, no organization name (beyond the delivery-map role labels "named org (TBD)", "named team (TBD)", "named evaluator (TBD)"), and no SF location may be invented.
- No causal claims: the only causal wording is inside the quoted `00-prospectus.md` §3.2 inference rules and quoted decision-state references; no dollar figures.
- No prohibited words (instructions.md §6): revolutionary, world-class, unique, cutting-edge, empower, unlock, transform, scalable, sustainable, "partners include", "data shows" - 0 hits. In particular, the word "unique" must NOT appear (source-case wording "uniquely contributes" is paraphrased as "contribution ... is undefined", never quoted).
- Quote fidelity: before writing Section 1.1, re-read `Documentation/Research/facts-pack.md` §(d) facts 1-11 and the "What the site does NOT show" paragraph; before writing the §1.2 inference-rules quote and the §5 non-claim sources, re-read `Documentation/Prospectus/00-prospectus.md` §3.2 and `01-source-case.md` row 7. If the recorded wording drifted from what §2.2 quotes, **stop and report - do not paraphrase or patch blind** (mirrors plan 008's quote-fidelity rule).
- Cross-links to planned files (`08-first-year-operating-plan.md`, `02-claim-ledger.md`) are plain backticked text, NOT markdown links - they do not exist yet, and dangling links fail V9.

### 2.2 Complete file content (write exactly this)

```
# Platform Boundary - FTSArcade / Boundless San Francisco

**Version:** S0 (boundary only) · **Date:** 2026-10-14
**Status:** **BOUNDARY ONLY - NOT DRAFTABLE.** As of 2026-10-14, DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) are all **undecided** (`03-registers.md` §1.1); no intervention is defined anywhere (`01-source-case.md` rows 1, 3, 5). The **inside** of the boundary (what the platform is) is recorded from E1 product facts; the **outside** (who provides the human/partner services around the platform) is `[INFORMATION NEEDED: ...]` markers; **no feature, provider, or outcome is invented, and no gameplay-to-outcome claim is made.** The boundary becomes fully draftable only when the three scope-lock decisions close (Section 6).
**Purpose:** Define the platform's boundary - what is inside the platform (E1 product facts), what is outside it (human/partner services), who provides the outside items, and where the platform ends - as the **framework** the concrete intervention attaches to once DR-01/DR-06/DR-07 close. This file is the T06 deliverable of plan 001 (bucket CONTENT) and feeds T07 (claim ledger) and T08 (first-year operating plan).
**Sources:** `../Research/facts-pack.md` §(d) (platform facts 1-11, E1, quoted verbatim), `00-prospectus.md` §3.2 (provisional platform boundary; inference rules), `01-source-case.md` row 4 (platform role, provisional) and row 7 (E5-removed claims), `04-delivery-and-budget.md` workstreams W-04/W-05/W-06/W-07/W-08/W-09/W-10, `06-participant-pathway.md` (T05 framework).
**Cross-links:** planned files `08-first-year-operating-plan.md` (T08), `02-claim-ledger.md` (T07). All owners are roles (per `03-registers.md` rules); named persons are `[INFORMATION NEEDED: program lead; required to name the person for each role (owner test); blocks the whole document - DR-01]`.

## 1. Platform definition and function scope

### 1.1 What the platform is (E1 product facts, verbatim from facts-pack §(d))

**No-inference rule in force (from the facts pack):** the facts below are observations of what the site displays; they are NOT converted into outcome claims (users, engagement, learning, employment, or charitable benefit are NOT stated anywhere on the page).

| # | Observed fact (what the live page shows) | Verification |
|---|------------------------------------------|--------------|
| 1 | HTML title: "FishTacoStand Arcade"; in-page heading "FTS ARCADE". | verified |
| 2 | Marquee: "INSERT COIN" and "── SELECT GAME · CABINET ART · 24 CABINETS ──". | verified |
| 3 | Banner text: "FREE PLAY" and "FREE PLAY · 15 LIVE"; instruction "tap a cabinet to play". No login, payment, or access-gate text visible on the page. | verified |
| 4 | Badges: "NEW · JUST WIRED" on 3 cabinets (COVEN BLITZ, @UNDERHALL, VECTOR SIEGE); "COMING SOON · 8 ON THE BENCH" for the workbench section. | verified |
| 5 | Fifteen (15) live/playable cabinets listed: ASTROIDS (Obliteratus Vector Survival), CAVE RACER (Cave Runner), COVEN BLITZ, CRAWFORD COUNTY (Volumetric Explorer), GRACE BLAND (Clocktower Boss Arena), GRID WARDEN (Tower Defense), MINESWEEPER (Stockpile Steward), NEON INVADERS (Fixed Shooter), PACKMAN (Postal Maze), PLINKO (Physics Chance), RED EYE (Observe), ZITTRIS (Chain Stacker), @UNDERHALL (Turn-Based Delve), VECTOR SIEGE (City Aegis), SOVTHPAW'S ZOMBIE GOLF (Golf Survival). | verified |
| 6 | Work-in-progress section: 9 entries marked "COMING SOON" + "WIP BUILD": CAVE DEFENDER, TOURNAMENT CONDUCTOR, EXCITE BIKE MOTOCROSS, HEX PUZZLE, RC RACER, MOONSHOT PINBALL, ASTRO VULPIS, AUXor, BOG FROG (BOG FROG additionally labeled "PLACEHOLDER · UNSTYLED · N=1 TILE - AWAITING ART & ACCENT PASS"). | verified |
| 7 | Observed arithmetical note (not an inference): page labels "24 CABINETS" and "8 ON THE BENCH", but 15 live + 9 WIP entries = 24 cabinets and 9 WIP entries listed. Counts as displayed are internally inconsistent by one on the bench count. | verified (label vs list) |
| 8 | WIP warning dialog ("CABINET STILL ON THE BENCH"): "This build is playable, but it is still being tuned. Expect unfinished art, balance, controls, or save behavior." Buttons: "STAY IN ARCADE" / "PLAY WIP BUILD". | verified |
| 9 | Settings control panel ("SETTINGS CONTROL PANEL · FTS ARCADE · FLOOR ENVIRONMENT"): audio routing (Master Volume; Crowd Ambience from crowd.mp3; Jukebox - "Disabled by default until a stream or direct audio URL is configured"; Cabinet SFX), display/accessibility (CRT Treatment - "Scanlines, screen vignette, and cabinet-screen texture"; Reduced Motion), "Preferences are stored locally on this browser", "AUDIO WAITS FOR THE FIRST PLAYER INPUT." | verified |
| 10 | Navigation: "◄ EXIT ARCADE" / "WORKBENCH EXIT"; "ESC · EXIT ARCADE". | verified |
| 11 | Game flavor text references SF-adjacent place/game content (e.g., CRAWFORD COUNTY "WALK · SPRINT · MAP · DISCOVER", PACKMAN "POSTAL MAZE - DELIVER · COLLECT PARCELS · EVADE GHOSTS", VECTOR SIEGE "SAVE SIX CITIES") - recorded as displayed labels only; no interpretation. | verified (as labels) |

**What the site does NOT show (equally important):** no user counts, no play metrics, no engagement figures, no learning/employment/economic-outcome claims, no SF-benefit claim, no partner list, no funding model, no stated public-outcome mission. Any such claim in an application must be labeled as an assumption/proposal, not a site fact.

### 1.2 Function scope - what the platform does and does not do

**Functions the platform performs (all E1, all live as of 2026-10-14):**

| Function (what the platform does) | Evidence | Status |
|---|---|---|
| Free browser-based play of 15 live cabinets; no login, payment, or access gate | `../Research/facts-pack.md` §(d) facts 1, 3, 5 (E1) | Live |
| Workbench: 9 WIP builds labeled "COMING SOON" + "WIP BUILD", with a warning dialog before play | facts 4, 6, 8 (E1) | Live |
| Settings/accessibility: audio routing, CRT Treatment, Reduced Motion; preferences stored locally on the browser | fact 9 (E1) | Live |
| Cabinet selection, play session, and exit navigation | facts 2, 10 (E1) | Live |
| SF-adjacent game flavor labels - displayed labels only, no interpretation | fact 11 (E1) | Recorded as labels only |

**Functions the platform does NOT perform** (from `00-prospectus.md` §3.2, excluded-functions row): recruitment, supervision, instruction, assessment, safeguarding, pastoral support, partner management, advertising-standards control, business selection. None of these appears on the site (facts-pack §(d), "What the site does NOT show": no partner list, no funding model, no stated public-outcome mission). These are the outside column of Section 2.

**Site-observation inference rules** (quoted verbatim from `00-prospectus.md` §3.2, binding): a playable game = publicly accessible game, **not** improved learning/employment; several titles = titles available, **not** a community/pipeline; WIP warning = product under development, **not** ready for citywide deployment; no account required = stated technical condition, **not** realistic access for a target population; browser access = browser access, **not** institutional adoption; team built the site = product-development capability, **not** ability to deliver education or social services.

### 1.3 Boundary statement

The platform is a browser-based arcade website (facts-pack §(d), E1). It currently performs no intervention role: no participant pathway, no charitable frame, and no public outcome are defined (DR-01/DR-06/DR-07 undecided as of 2026-10-14, `03-registers.md` §1.1). The boundary therefore separates what the platform itself provides (inside - the E1 facts in Section 1.1) from what humans and partner organizations must provide around it (outside - Section 2), with the provider of each outside item named as a delivery-map role or left as a marker. The platform's contribution to an intervention is undefined until the intervention is chosen (source case row 4); the essential-function list with per-function acceptance tests is `[INFORMATION NEEDED: technical owner + program lead; required to list the essential functions with current readiness, required development, acceptance test, owner, and operating cost per function (delivery-map W-04); blocks Section 1 - DR-05/DR-01]`.

## 2. Boundary table: inside platform | outside platform | provider of outside items

**Reading note:** the platform provides the inside column (E1 product facts); every outside service is performed by humans or partner organizations and is `[INFORMATION NEEDED]` because the beneficiary (DR-01), charitable frame (DR-06), and single public outcome (DR-07) are undecided as of 2026-10-14. The provider column carries delivery-map roles (`04-delivery-and-budget.md` §1); named persons are `[INFORMATION NEEDED]` (BU-06). The boundary ends where the site ends: the platform does not recruit, supervise, instruct, assess, safeguard, manage partners, control advertising, select businesses, or evaluate participants.

| Inside platform | Outside platform | Provider of outside items |
|---|---|---|
| Free browser-based play of 15 live cabinets; no login, payment, or access gate (facts 1, 3, 5; E1) | **Recruitment** of participants into the intervention: `[INFORMATION NEEDED: program lead; required to name the recruitment organization and its SF grounding once DR-01 closes; blocks this outside service - DR-01]` | Named org (TBD - W-05) |
| Workbench: 9 WIP builds honestly labeled "COMING SOON" + "WIP BUILD", with a warning dialog before play (facts 4, 6, 8; E1) | **Supervision** of participants during play: `[INFORMATION NEEDED: program lead; required to specify who supervises play sessions once the intervention is defined; blocks this outside service - DR-01/DR-06]` | Named team (TBD - W-06) |
| Settings/accessibility: audio routing, CRT Treatment, Reduced Motion; preferences stored locally (fact 9; E1) | **Instruction / facilitation** of sessions: `[INFORMATION NEEDED: program lead; required to specify facilitation staffing per the chosen intervention (source case row 3); blocks this outside service - DR-01/DR-05]` | Named team (TBD - W-06) |
| Cabinet selection, play session, exit navigation (facts 2, 10; E1) | **Assessment** of learning or progression: `[INFORMATION NEEDED: named evaluator; required to specify the assessment instrument once DR-07 closes; blocks this outside service - DR-07/DR-05]` | Named evaluator (TBD - W-10) |
| SF-adjacent game flavor labels - displayed labels only, no interpretation (fact 11; E1) | **Safeguarding / pastoral support** for participants: `[INFORMATION NEEDED: program lead; required to name the safeguarding owner and policy once the pathway is defined; blocks this outside service - DR-01/DR-06]` | Program lead; named team (TBD - W-06) |
| No platform function (not on the site - facts-pack §(d) does-NOT-show list) | **Partner management** (site partners, community organizations): `[INFORMATION NEEDED: program lead; required to name partner targets and statuses once DR-06 closes; blocks this outside service - DR-06]` | Program lead (W-08, W-09) |
| No platform function (not on the site) | **Advertising-standards control; business selection** (only if commercial elements are adopted): `[INFORMATION NEEDED: program lead + counsel; required once DR-06 closes; blocks this outside service - DR-06]` | Program lead + counsel |
| No platform function (not on the site) | **Evaluation / outcome measurement** of participants: `[INFORMATION NEEDED: named evaluator; required to specify the pre-registered outcome indicator once DR-07 closes; blocks this outside service - DR-07]` | Named evaluator (TBD - W-10) |

## 3. SF-ecosystem dependencies (with source links)

**Reading note:** the platform is a website and depends on an SF ecosystem only where an intervention uses it. Given DR-06 (charitable frame) is undecided as of 2026-10-14, every ecosystem dependency below is a marker, not a commitment; source links point to the facts-pack §(e) resource rows, which hold the live URLs and archive statuses.

| Dependency | What the platform depends on it for | SF source | Status |
|---|---|---|---|
| SF site/facility partner (physical installation of cabinets; space, power, access) | A permitted public location to install and operate cabinets | `../Research/facts-pack.md` §(e): SF Recreation and Park Department (ARCHIVED - conflict C6; re-verify live before use) | `[INFORMATION NEEDED: program lead + counsel; site plan and facility partner - DR-06]` |
| City permissions / permits | Legal operation at the chosen location | facts-pack §(e): SF Recreation and Park Department (ARCHIVED - C6) | `[INFORMATION NEEDED: program lead + counsel; permissions per site - DR-06]` |
| Community / neighborhood organizations | Referral and supervision of participants at the site | facts-pack §(e): SF Cultural Districts Program (LIVE); no organization confirmed | `[INFORMATION NEEDED: program lead; partner statuses - DR-01/DR-06]` |
| City arts & culture framework | Frame-alignment wording for a cultural-installation direction | facts-pack §(e): SF Arts Commission - Mission & Values (LIVE) | `[INFORMATION NEEDED: program lead; adopted only if DR-06 closes on a cultural frame - DR-06]` |
| Economic / workforce ecosystem | Recruitment and employment pathways (only if DR-01 option (a) is chosen) | facts-pack §(e): OEWD; Office of Small Business reports (LIVE) | `[INFORMATION NEEDED: program lead; option (a) not chosen - DR-01]` |
| Fiscal sponsor / lead entity | Legal route to submit and control funds | facts-pack #15 (rules §1); candidates proposed only (source case row 6) | `[INFORMATION NEEDED: authorized officer; registration and entity status - DR-02/DR-03]` |
| Jukebox audio source (stream or direct audio URL) | Optional ambience; disabled by default until configured | facts-pack §(d) fact 9 (E1) | Disabled by default; configuration = technical owner (W-07) |
| SF-adjacent content provenance | Flavor labels' SF grounding | facts-pack §(d) fact 11 (E1, as labels) | Recorded as labels only; no interpretation |

## 4. Boundary unknowns - INFORMATION NEEDED list

| # | Unknown | Owner | Why | Decision blocked | Unblocks |
|---|---|---|---|---|---|
| BU-01 | Essential-function list (current readiness, required development, acceptance test, owner, operating cost per function) | Technical owner | `00-prospectus.md` §3.2 requires per-function acceptance tests (delivery-map W-04); none documented | DR-05/DR-01 | Sections 1-2 |
| BU-02 | Platform's contribution to an intervention | Program lead | Source case row 4 is provisional only; the function list is empty until the intervention is chosen | DR-01/DR-05 | Section 1 |
| BU-03 | Providers of outside services (recruitment, supervision, instruction, assessment, safeguarding, pastoral support, partner management, advertising control, business selection) | Program lead | §3.2 excluded list is "Mandatory; no owner named"; frame and outcome undecided | DR-01/DR-06/DR-07 | Section 2 |
| BU-04 | Site plan and facility partner (physical installation) | Program lead + counsel | DR-06 frame requires a defined site plan | DR-06 | Section 3 |
| BU-05 | Permissions/permits for SF locations | Program lead + counsel | Rec & Park source archived (C6); no site chosen | DR-06 | Section 3 |
| BU-06 | Named person per role | Program lead | Owner test needs named parties | DR-01 | Whole document |
| BU-07 | Platform operating cost and maintenance owner (post-grant) | Executive owner | Durability test needs a named payer | DR-10 | Sections 2-3 (W-07) |
| BU-08 | Rights/IP schedule (code, art, audio, third-party components, contributor agreements) | Rights owner | Rules require appropriate rights for third-party material; the export flags IP review for a game platform | DR-09 | Whole document |
| BU-09 | Jukebox audio source configuration | Technical owner | Disabled until a stream or direct audio URL is configured (fact 9) | None (technical) | Section 1 |
| BU-10 | Count-conflict C3 resolution ("24 CABINETS" / "8 ON THE BENCH" labels vs 15 live + 9 WIP listed) | Research | Cosmetic (facts-pack C3); do not assert counts from labels | None (label hygiene) | Section 1 (fact 7) |
| BU-11 | Full Application PDF link 404 (facts-pack C4) | Research | Box link returns HTTP 404; application-form details unverifiable without a real-browser check | DR-02 (submission route) | Section 3 (fiscal-sponsor row) |

## 5. Non-claims - what the platform is NOT asserted to produce

**Rule:** the platform's gameplay is not asserted to produce any of the outcomes below. Each non-claim carries the source of its prohibition; any gameplay-to-outcome statement in an application must carry an evidence grade and be labeled an assumption/proposal, never a site fact (instructions.md §5; facts-pack §(d) no-inference rule).

| Non-claim (NOT asserted) | Why it is not asserted | Source of the prohibition |
|---|---|---|
| Learning gains from gameplay | A playable game is a publicly accessible game, not improved learning; the site states no learning claim | `00-prospectus.md` §3.2 inference rules; `../Research/facts-pack.md` §(d) no-inference rule |
| Employment outcomes from gameplay | "Completing a game leads to employment" is not automatic; the site states no employment claim | `00-prospectus.md` §3.2, §4.1 |
| Community formation | Several titles available = titles available, not a community or pipeline | `00-prospectus.md` §3.2 inference rules |
| City popularity | No popularity claim on the site; unsupported popularity claims removed | `01-source-case.md` row 7 (E5) |
| Building/street revitalization | Revitalization claims removed | `01-source-case.md` row 7 (E5) |
| Economic development | Economic-development claims removed | `01-source-case.md` row 7 (E5) |
| Mobility improvement | Mobility-via-QR claims removed | `01-source-case.md` row 7 (E5) |
| Equitable business benefit | Equitable-business-benefit claims removed | `01-source-case.md` row 7 (E5) |
| User counts, play metrics, or engagement figures | The site displays none; they are not convertible into claims | `../Research/facts-pack.md` §(d), "What the site does NOT show" |
| Engagement metrics as outcomes | Engagement metrics are never outcomes (DR-07 decision rule) | `03-registers.md` §1.1 DR-07 |
| SF-benefit claim, partner list, funding model, public-outcome mission | The site states none; any such claim must be labeled an assumption/proposal, not a site fact | `../Research/facts-pack.md` §(d), "What the site does NOT show" |

## 6. Decision gate - when the boundary becomes draftable

The boundary's **inside** (what the platform is) is recorded from E1 product facts and stands on its own; the boundary's **outside** (who provides the human/partner services, which SF dependencies are real) **cannot be drafted while DR-01, DR-06, and DR-07 are undecided** (all recorded **undecided as of 2026-10-14**, `03-registers.md` §1.1; consequence of delay: all downstream work pauses; the packet stays Not ready). This document is the framework those decisions attach to.

**Gate:** DR-01 (beneficiary), DR-06 (charitable frame), and DR-07 (single public outcome) each closed in `03-registers.md` §1.1 with a decided value, deciding owner, date, and evidence grade (plans 001 T02-T04 recorded the undecided states; changes 005/006/007).

**Once the gate opens:** a follow-on plan (successor to this plan, still T06 content) replaces every placeholder and `[INFORMATION NEEDED]` cell in Sections 2-4 with concrete content, per delivery-map workstream W-04 (`04-delivery-and-budget.md` §1: start condition = pathway design W-03; output = essential/supporting/excluded/non-claim lists with acceptance tests per essential function) under the scope-lock record W-02. This file is then re-verified with the full editing-test set (instructions.md §7).

**Until then:** no draftable boundary exists; this framework stands on its own - the deletion test passes (the boundary framework does not depend on the FTSArcade name) and the substitution test passes (inside cells are site facts that hold under substitution; outside cells carry no invented SF facts).

## 7. Revision record (per methodology)

| Date | Proposed change | Class | Reason | Evidence affected | Budget affected | Decision | Updated documents |
|---|---|---|---|---|---|---|---|
| 2026-10-14 | Platform boundary framework created (boundary-only: platform definition carries the E1 facts from facts-pack §(d) verbatim; function scope does/does-not with the site-observation inference rules; boundary table format inside platform \| outside platform \| provider of outside items with outside cells as INFORMATION NEEDED markers; SF-ecosystem dependencies table; boundary unknowns list (BU-01-BU-11); non-claims section; decision-gate note) | Clarifying | Plan 001 T06 (CONTENT) requires the platform boundary; DR-01/DR-06/DR-07 are undecided as of 2026-10-14, so the change records the E1-grounded boundary framework - no invented features, providers, or promoted outcomes | DR-01/DR-06/DR-07 decision states (E1, source: `03-registers.md` §1.1; ungraded - undecided); E1 platform facts (facts-pack §(d) facts 1-11) embedded verbatim; no new figures | None - zero dollar figures | No decision closed; boundary outside stays not draftable until scope lock | 07-platform-boundary.md (new), Logs/changes.md, Plan/000-index.md |
```

### 2.3 INFORMATION NEEDED markers list (must appear in the file)

The file's Section 4 table (BU-01…BU-11) is the consolidated unknowns list; the complete inline marker texts appear in Sections 1-3 exactly as written in §2.2. Count: **16 inline `[INFORMATION NEEDED: ...]` markers** (1 in the preamble cross-links line, 1 in §1.3, 8 in the Section 2 boundary table, 6 in the Section 3 dependencies table), each with owner + why + decision-blocked fields per instructions.md §5, each grouped into exactly one of the BU rows above. (The Status-line phrase "`[INFORMATION NEEDED: ...]`" is a format description, not a marker; `grep -c` on the file will read 17 hits including it - V3 accounts for this.)

| ID | Owner | Decision blocked | Unblocks |
|---|---|---|---|
| BU-01 | Technical owner | DR-05/DR-01 | Sections 1-2 (essential-function list) |
| BU-02 | Program lead | DR-01/DR-05 | Section 1 (platform contribution) |
| BU-03 | Program lead | DR-01/DR-06/DR-07 | Section 2 (outside providers) |
| BU-04 | Program lead + counsel | DR-06 | Section 3 (site plan, facility partner) |
| BU-05 | Program lead + counsel | DR-06 | Section 3 (permissions/permits) |
| BU-06 | Program lead | DR-01 | Whole document (named persons) |
| BU-07 | Executive owner | DR-10 | Sections 2-3 (operating cost, W-07) |
| BU-08 | Rights owner | DR-09 | Whole document (rights/IP schedule) |
| BU-09 | Technical owner | None (technical) | Section 1 (jukebox configuration) |
| BU-10 | Research | None (label hygiene) | Section 1 (count conflict C3) |
| BU-11 | Research | DR-02 (submission route) | Section 3 (PDF 404, C4) |

---

## 3. F3 - `Documentation/Logs/changes.md`

**Append one row after the plan-008 row (currently line 17), same column format (8 columns; pipes inside cells escaped as `\|` where table formats are named):**

```
| 2026-10-14 | Clarifying | Create platform boundary document (`Prospectus/07-platform-boundary.md`, new): boundary-only - platform definition carries the E1 product facts from facts-pack §(d) verbatim (15 live cabinets, 9 WIP builds, work-in-progress warnings, accessibility incl. reduced motion, browser access, no-account condition, count conflict C3); function scope does/does-not with the site-observation inference rules; boundary table inside platform \| outside platform \| provider of outside items with outside cells as INFORMATION NEEDED markers (recruitment, supervision, instruction, assessment, safeguarding/pastoral support, partner management, advertising-standards control, business selection); SF-ecosystem dependencies table (all markers given DR-06 undecided); boundary unknowns list (BU-01-BU-11); non-claims section (what the platform is NOT asserted to produce); decision-gate note (boundary outside draftable only after DR-01/DR-06/DR-07 close) | Plan 001 T06 (CONTENT) requires the platform boundary; DR-01/DR-06/DR-07 are all undecided as of 2026-10-14, so the change records the E1-grounded boundary framework - no invented features, providers, or promoted outcomes | DR-01/DR-06/DR-07 decision states propagated (E1, source: 03-registers.md §1.1; ungraded - undecided); E1 platform facts (facts-pack §(d) facts 1-11) embedded verbatim; no new figures; no budget affected | No decision closed - boundary outside stays not draftable until scope lock | Prospectus/07-platform-boundary.md (new), Logs/changes.md, Plan/000-index.md | 009 |
```

---

## 4. F4 - `Documentation/Plan/000-index.md`

**Append one row after the plan-008 row (currently line 16):**

```
| 009 | `Documentation/Plan/009-platform-boundary.md` | Platform boundary: what the platform is, inside/outside split, provider map (plan 001 T06) | planned | Pre-plan agent wrote the plan; orchestrator flips status after execution and commit |
```

---

## 5. Verification (run in order; every check must pass before handoff)

Per plan 001 §2 task detail T06: substitution test; owner test; no "scalable" without a unit cost; plus the boundary-honesty checks below. Per instructions.md §11.6, the orchestrator starts the threefold review run before the version is committed; the changes.md row is appended only after all three facets pass or a blocked status is recorded (the execute agent appends the row at handoff per T06; the orchestrator holds the commit).

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No invented platform content | Read `Documentation/Prospectus/07-platform-boundary.md` against §2.2 of this plan | The file matches §2.2 verbatim: the only inside functions are the 5 E1-grounded rows of §1.2; every outside cell is exactly the `[INFORMATION NEEDED: ...]` text specified; 0 concrete features beyond facts-pack §(d) facts 1-11, 0 named persons, 0 organization names beyond the delivery-map "TBD" role labels, 0 SF locations, 0 outcome claims appear anywhere |
| V2 | E1 facts match facts-pack verbatim | Compare the §1.1 fact table and the "What the site does NOT show" paragraph against `Documentation/Research/facts-pack.md` §(d) facts 1-11 (row-by-row text match) | All 11 fact rows and the does-NOT-show paragraph match verbatim; counts preserved (15 live / 9 WIP / label-inconsistency wording of fact 7); the file asserts no count from labels beyond fact 7's wording |
| V3 | INFORMATION NEEDED markers complete | `grep -c "\[INFORMATION NEEDED:" Documentation/Prospectus/07-platform-boundary.md` + inspect each marker | ≥ 16 markers (a 17th hit is the Status-line format description "`[INFORMATION NEEDED: ...]`" - not a marker, no owner field); every marker has the format `[INFORMATION NEEDED: <owner>; <why>; ... <decision blocked>]` with a named role owner and a blocked decision; the §4 table contains exactly rows BU-01…BU-11 and every inline marker maps to one of them |
| V4 | Owner test (every action verb has a named party) | Underline every action verb in the new file | Each action is either (a) performed by a named role (technical owner, program lead, named org/team/evaluator TBD, etc.) or (b) inside an `[INFORMATION NEEDED: <owner>; ...]` marker naming the owner; 0 unattributed action verbs |
| V5 | Substitution test (city changed → SF facts remain) | Replace "San Francisco"/"SF" with another city in a copy of the file | Every cell that names SF either cites an E1 source (facts-pack §(d) facts; §(e) dependency rows) or carries `[INFORMATION NEEDED: ...]`; 0 city-specific facts stated without a source; the inside cells (browser arcade, 15 live, 9 WIP, settings, no-account) remain true under substitution |
| V6 | Non-claims section present | Inspect Section 5; `grep -niE "improves|leads to|enables|increases|drives|creates|produces" Documentation/Prospectus/07-platform-boundary.md` | Section 5 exists with ≥ 10 non-claim rows, each naming a prohibition source; 0 causal-claim hits; the word "outcome" appears only in non-claim/prohibition or DR-07-rule contexts; no sentence asserts a gameplay-to-outcome effect |
| V7 | No "scalable" without a unit cost (T06 rule) | `grep -ni "scalable" Documentation/Prospectus/07-platform-boundary.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits (the word never appears; the T06 condition is trivially satisfied - no unit cost is needed where no scalability claim exists) |
| V8 | Tables render | For every table in the new file (Sections 1.1, 1.2, 2, 3, 4, 5, 7): header row, separator row, and body rows have equal pipe counts | Equal pipe counts per table; separator row present in each; the `\|` escapes inside the §7 revision-record cell render as a literal pipe without breaking the row |
| V9 | Cross-links resolve | `test -f Documentation/Prospectus/03-registers.md Documentation/Prospectus/01-source-case.md Documentation/Prospectus/00-prospectus.md Documentation/Prospectus/04-delivery-and-budget.md Documentation/Prospectus/06-participant-pathway.md Documentation/Research/facts-pack.md; echo "EXIT:$?"` + extract every `](…)` target from the new file | All six files exist (EXIT:0); every relative link target in the file resolves with `test -f`; 0 dangling links (planned-file cross-links `08-first-year-operating-plan.md` / `02-claim-ledger.md` are backticked text, not links) |
| V10 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' Documentation/Prospectus/07-platform-boundary.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits in the three executed files (the plan file and instructions.md §6's own list are exempt by construction); grep "unique" likewise - 0 hits |
| V11 | Exact file set | `git status --porcelain` (compare against the pre-execution snapshot) | The change touches exactly 1 new file (`Documentation/Prospectus/07-platform-boundary.md`) + exactly 2 modified files (`Documentation/Logs/changes.md`, `Documentation/Plan/000-index.md`); `Documentation/Plan/009-platform-boundary.md` appears as the pre-plan artifact (added/untracked); no other file touched; no deletions |
| V12 | changes.md row | Inspect `Documentation/Logs/changes.md` | One new row: class **Clarifying**, plan ref 009, date 2026-10-14, documents updated listing the new file + `Plan/000-index.md`; appended after the plan-008 row; existing rows unchanged |
| V13 | Index self-consistency | Inspect `Documentation/Plan/000-index.md` | Row 009 present, status `planned`; existing rows 001-008 unchanged |

---

## 6. Executor inputs (read from the repo, never invent)

| Item | Where to read it | Why |
|---|---|---|
| E1 platform facts, verbatim | `Documentation/Research/facts-pack.md` §(d) facts 1-11 + "What the site does NOT show" paragraph | Section 1.1 embeds them verbatim; quote-fidelity rule (stop if drifted, do not patch blind) |
| §3.2 provisional boundary + inference rules | `Documentation/Prospectus/00-prospectus.md` §3.2 | Sections 1.2 and 5 draw the excluded-functions list, the non-claims list, and the inference-rules quote verbatim |
| E5-removed claims list | `Documentation/Prospectus/01-source-case.md` row 7 | Section 5 non-claim sources |
| DR-01/DR-06/DR-07 recorded entries (verbatim undecided wording) | `Documentation/Prospectus/03-registers.md` §1.1 | Preamble and Section 6 carry the states; quote-fidelity rule |
| Role names for provider cells | `Documentation/Prospectus/04-delivery-and-budget.md` §1 (W-04, W-05, W-06, W-07, W-08, W-09, W-10) | Provider cells must match the delivery map's roles exactly (program lead, technical owner, named org/team/evaluator TBD) |
| SF ecosystem source rows + archive statuses | `Documentation/Research/facts-pack.md` §(e) (LIVE/ARCHIVED legend; C6 caveat) | Section 3 dependency rows cite the facts-pack rows and preserve the archive caveat |
| Marker syntax + change-class definitions | `Documentation/Logs/instructions.md` §5, §9.2 | `[INFORMATION NEEDED: <owner>; why; decision blocked]` format; class Clarifying |
| Current row positions in F3/F4 | `Documentation/Logs/changes.md` (line 17), `Documentation/Plan/000-index.md` (line 16) | Append after the plan-008 rows; re-check at execution |

**Explicitly out of scope for the executor:** choosing or recommending any option of DR-01/DR-06/DR-07 (including naming an indicator, population, site, or provider - any such action violates this plan); inventing any platform feature, SF location, provider, or outcome; editing `03-registers.md`, `01-source-case.md`, `00-prospectus.md`, `04-delivery-and-budget.md`, `06-participant-pathway.md`, root `README.md`, `Documentation/Research/*`, or `Documentation/Refinement/*` (their records already exist and are referenced, not duplicated); drafting any email or promotional copy (protocol R1); committing (orchestrator-only, rule R2).