# Delivery Map and Budget Workbook - FTSArcade / Boundless San Francisco

**Version:** S0 · **Date:** 2026-10-14
**Rules:** "Proposed," "in discussion," and "confirmed" must remain visible in this table and in any prose derived from it. No dollar figures are invented: every amount is `[INFORMATION NEEDED: <owner>; cost source]` until the budget owner supplies a verified figure. Budget quantities must come from the delivery plan (costs derive from activities, never the reverse).

---

## 1. Delivery map

Workstream rows follow the methodology template: Workstream · Output · Responsible party · Dependencies · Start condition · Failure response. Status labels: **confirmed** (none), **in discussion** (none), **proposed** (as marked). All responsible parties are unnamed roles until named persons are supplied.

| # | Workstream | Output | Responsible party | Dependencies | Start condition | Failure response | Status |
|---|---|---|---|---|---|---|---|
| W-01 | Registration & eligibility | Confirmed registration status; eligible Lead Organization with authority to control funds | Authorized officer (unnamed) | Registration confirmation/exception answer; entity documents; written foreign-entity confirmation if applicable | Evidence of valid route to submit (DR-02, DR-03) | Stop: do not draft; produce gap report only | Proposed (no evidence of registration) |
| W-02 | Scope lock | Approved beneficiary, single public outcome, charitable frame, outcome claim | Decision owner (unnamed) | DR-01, DR-05, DR-06, DR-07 decisions with written rationale | Decisions recorded in `03-registers.md` | Do not proceed to pathway design; revisit options | Not started |
| W-03 | Participant pathway design | One approved pathway: first contact → completion, with dose, setting, staffing, completion rule | Program lead (unnamed) | Scope lock (W-02) | Pathway documented and approved | Revise pathway or narrow scope | Not started |
| W-04 | Platform boundary | Essential/supporting/excluded/non-claim lists with acceptance tests per essential function | Technical owner (unnamed) | Pathway design (W-03) | Acceptance tests defined for every essential function | Manual fallback or delay launch; feature stays outside prospectus until tested | Partially started (provisional lists in `00-prospectus.md` §3.2; no acceptance tests) |
| W-05 | Recruitment | Eligible participants enrolled | Named org (TBD) | Access to population; agreed partner | Agreement + staffing in place | Alternative channel or reduced cohort | Not started |
| W-06 | Program delivery | Sessions completed | Named team (TBD) | Facilitators + facilities | Training complete | Pause cohort; do not expand | Not started |
| W-07 | Platform delivery | Required functions available and maintained | Technical owner (unnamed) | Licensing + maintenance funded (DR-09) | Acceptance test passed | Manual fallback or delay launch | Not started |
| W-08 | SF establishment | Named local leadership, locations, partner statuses, community input | Program lead (unnamed) | Scope lock (W-02) | Sequence, criteria, decision points documented | State plainly: local presence remains to be established | Not started |
| W-09 | Partner engagement | Written confirmations with accurate statuses | Program lead (unnamed) | Target list from W-08 | Approvals documented per status | Downgrade language to "proposed"; never upgrade without confirmation | Not started - fiscal sponsors (Community Initiatives; Intersection for the Arts) are **proposed** candidates only |
| W-10 | Evaluation | Usable outcome data against pre-registered indicators | Named evaluator (TBD) | Consent + instruments; baseline defined | Baseline defined before scaling | Correct method before scaling | Not started |
| W-11 | Budget & scenario selection | Four-layer cost model; selected scenario with proportionality statement | Budget owner (unnamed) | Delivery plan quantities (W-03-W-08) | Costs traceable to activities | Resize project or request | Not started |
| W-12 | Rights / IP clearance | Completed rights schedule covering proposed use | Rights owner (unnamed) | Asset inventory (code, art, audio, third-party, contributor agreements) | All ownership/licensing documented | Submission blocked (DR-09) | Not started |
| W-13 | Post-submission peer review | 4 (up to 6) peer applications reviewed, ~2.5 h, Nov-Dec 2026 | Named reviewer (TBD - DR-08) | Submission completed; invitation | Calendar slot assigned | Participation may terminate | Not started |

---

## 2. Budget workbook structure

### 2.1 Four layers (build order)

| Layer | Content | Current status |
|---|---|---|
| L1 **Unit cost** | Cost per session, participant, site, license, staff role | `[INFORMATION NEEDED: budget owner; cost source]` - no units defined until pathway exists (W-03) |
| L2 **Operating volume** | Number of cohorts, sites, users, months | `[INFORMATION NEEDED: budget owner; requires beneficiary + pathway decisions (DR-01, DR-05)]` |
| L3 **Support costs** | Management, evaluation, accessibility, data, administration required for that volume | `[INFORMATION NEEDED: budget owner; cost source]` |
| L4 **Contingency & sensitivity** | Costs affected by enrollment, facilities, staffing, delayed adoption | `[INFORMATION NEEDED: budget owner; requires L1-L3]` |

### 2.2 Line categories (from the methodology; each line needs quantity, unit cost, source of estimate, timing, intended result)

| Line | Required fields | Status |
|---|---|---|
| Community delivery and local partner costs | Quantity, unit cost, source, timing, result | Not started |
| Participant support or compensation (where appropriate) | Same | Not started |
| Program staff and management | Same | Not started |
| Technology development, accessibility, security, maintenance | Same | Not started - product facts only; no maintenance cost documented |
| Independent evaluation and data collection | Same | Not started |
| Legal, safeguarding, insurance, financial administration | Same | Not started |
| Indirect costs | Allocation method; **cap: 29% of direct project/activity costs, within the $50M award limit** (E1, rules §7) | Rule known; allocation method not defined |

### 2.3 Three scenarios (no amounts; all figures `[INFORMATION NEEDED]`)

| Scenario | Definition | Content required | What is lost if cheaper scenario chosen |
|---|---|---|---|
| **Constrained** | Essential pilot and evidence-building only | Pilot cohorts, minimum platform work, independent evaluation, legal/compliance | - |
| **Proposed** | Scale justified by delivery capacity | Full delivery plan volumes (W-03-W-08) | State which outputs disappear at constrained level |
| **Maximum** | Scale requiring additional confirmed capacity, not merely more money | Confirmed partners, staff, sites, adoption commitments | State which outputs cannot yet be executed responsibly |

**Proportionality rules (binding):** the request must equal supported costs; do not start from $50M and reverse-engineer activities. Indirect costs are included within the award limit (not added on top). Reduce the request by half and state exactly which outputs disappear - that test justifies the original figure. For a for-profit lead, funds are subject to expenditure responsibility (IRC §4945(h)) and cannot be used entirely for general operating support; a documented charitable-purpose budget with spending controls is required.

### 2.4 Budget narrative formula (apply to every major cost)

1. Name the operating assumption. 2. Show quantity and unit cost. 3. Connect to an output. 4. State what happens if the assumption changes. 5. Identify any cost that continues after the grant (feeds durability model, DR-10).

---

## 3. First-year operating plan boundary

| Horizon | May include | Must not include | Status |
|---|---|---|---|
| First year | Capacity that named people and partners can deliver | Scale dependent on unsigned partners | Nothing named yet → first-year plan cannot be built |
| Years 2-5 | Expansion triggered by stated results (metric, threshold, review date, authorized approver) | Automatic growth without decision thresholds | No triggers defined |
| After grant | Retained assets, adopted activities, funded operations | Every activity continuing unchanged by default | Post-grant model open (DR-10) |

Expansion is a decision, not an assumption: each trigger needs a metric, threshold, review date, and the person authorized to approve expansion.