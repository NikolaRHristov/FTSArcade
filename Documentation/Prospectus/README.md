# FTSArcade - Boundless San Francisco Stage 1 - Internal Grant Prospectus Packet

**Date:** 2026-10-15 (Thursday) - status fields updated by change 015 (plan 001 T12); packet content unchanged.
**Version label:** **S0 - Incomplete source packet; gap identification only.** Per the writing methodology (Reference/…/we're looking to prepare a grant application for h.md), S0 means the sources are not yet approved for drafting and this packet exists to surface gaps, not to persuade. **Unchanged: the relabel to D1 is deferred (see Readiness state).**
**Readiness state:** **Not ready** - the framework build is complete (all 12 plan-001 tasks executed; T01-T11 = plans 004-014, committed; T12 = change 015), but the packet is NOT Draftable: the verification pass recorded 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL across 29 rows (`Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)); 4 distinct tests are BLOCKED - deletion, substitution, proportionality, sign-off - and the eligibility gate (DR-11) is Blocked. Unblocking decisions: DR-01/DR-06/DR-07 scope lock (deletion, substitution) -> narrative prose; DR-04 funding scenario (proportionality) -> request + loss list; DR-02/DR-03/DR-09/DR-11 + named signatory (sign-off). D1 relabel = named future change: "Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)". Drafting a submission narrative is not yet permitted.
**Packet owner:** Decision owner (unnamed). **[INFORMATION NEEDED: named decision owner; required to close any foundational choice; blocks every gate]**

---

## 1. Packet index

| # | File | Contents | Status | Input still required from |
|---|------|----------|--------|---------------------------|
| 1 | `README.md` (this file) | Index, version label, readiness state, next action, deadlines | S0 | - |
| 2 | `00-prospectus.md` | Master internal prospectus, 10-section architecture with page budget | S0 | All section owners |
| 3 | `01-source-case.md` | Source-case table: 10 rows with completion tests | S0 | All owners (mostly empty) |
| 4 | `02-claim-ledger.md` | 15-25 graded, owned claims with permitted wording | S0 | Owners to confirm grades |
| 5 | `03-registers.md` | Decision register (10 open), data dictionary, evidence register | S0 | Decision owners |
| 6 | `04-delivery-and-budget.md` | Delivery map + budget workbook structure (4 layers, 3 scenarios) | S0 | Program + budget owners |
| 7 | `05-durability-risks-rights.md` | Post-grant model, risk register with triggers, rights schedule | S0 | Rights + executive owners |
| 8 | `06-participant-pathway.md` | Participant pathway framework | S0 | Decision owners (DR-01/DR-06/DR-07 close) |
| 9 | `07-platform-boundary.md` | Platform boundary framework | S0 | Decision owners (DR-01/DR-06/DR-07 close) |
| 10 | `08-first-year-operating-plan.md` | First-year operating plan framework | S0 | Program + budget owners (scope lock; DR-04) |
| 11 | `09-unit-cost-model.md` | Unit-cost model & funding scenarios | S0 | Budget owner (DR-04) |
| 12 | `10-narrative.md` | Narrative framework (prose blocked until Draftable) | S0 | All owners (scope lock; DR-04; DR-10/DR-09; signatory) |

**Authoritative sources for this packet (nothing else was used):**
- The prior-conversation export: `Documentation/Reference/we're looking to prepare a grant application for h.md` (read in full; contains the methodology, the competition rules/FAQ/rubric verbatim extracts, the team's commercial roster, and the export's own analysis).
- The FTSArcade site, retrieved live 2026-10-14: https://frymatic.us/FTSArcade
- Live competition pages retrieved 2026-10-14: https://boundless-sf.leverforchange.org/rules and /faq (key facts verified against the live pages; see §3).

**Nothing else.** No beneficiary, partner, cost, outcome, or ownership fact appears in this packet unless it came from those sources or is explicitly marked as an assumption or `[INFORMATION NEEDED: ...]`.

---

## 2. Version labels and readiness states (from the methodology)

| Label | Meaning | Permitted use |
|---|---|---|
| S0 | Incomplete source packet | Gap identification only (current state) |
| S1 | Approved for drafting | Controlled draft |
| D1 | First fidelity draft | Review, not submission |
| D2 | Decision revisions incorporated | Further review |
| D3 | Compressed and polished | Application preparation |
| F | Frozen submission version | Submission only |
| X | Rejected or superseded | Historical reference only |

| Readiness state | Definition | Current? |
|---|---|---|
| Not ready | Beneficiary, intervention, eligibility, or budget absent | **Yes - current state** |
| Draftable | S1 sources approved, gaps visible | No - requires source completion |
| Reviewable | D1 traces and exception report complete | No |
| Revisable / Compressible / Submittable / Blocked | Later states | No (see notes below) |

Note: "Blocked" would apply if eligibility/registration turns out to be unresolvable; the packet is currently *Not ready* because sources are absent, with the registration question as the immediate go/no-go (see §3, DR-03).

---

## 3. Critical dates (verified against live FAQ/rules pages, 2026-10-14)

| Event | Date | Status / implication |
|---|---|---|
| Initial registration deadline | Friday, September 11, 2026, 5:00 p.m. PT | **Passed.** Only registered organizations receive the application invitation. Registration status of the team is **unknown** - this is the first go/no-go (DR-03). |
| Application deadline | Thursday, October 15, 2026, 5:00 p.m. PT (extended from Oct 9) | One day away. 5:00 p.m. PT on Oct 15 = **03:00 EEST on Friday, October 16, 2026** (PDT = UTC−7). |
| Administrative eligibility review | After submission | Submission screened against rules before Participatory Review. |
| Participatory Review (peer review) | November-December 2026 | Each applicant reviews **4 peer applications (up to 6 if necessary), ~2.5 hours**, using the rubric; failure to complete can terminate participation. Assign an owner now (DR-08). |
| Evaluation Panel Review | Following Participatory Review | Top-scoring applications advance; panel uses the same rubric. |
| Finalists selected | By June 2027 | 3-7 finalists; each receives a project development grant (pool totals $1-3.5M) + technical assistance. |
| Finalist investment prospectus | August 2027 | Comprehensive proposal; **not** due now. |
| Final awards | Fall 2027 | Up to 3 awards of **$10M-$50M** (max $50M). |

Other verified rules used throughout the packet:
- Indirect costs: up to **29% of direct project or activity costs**, within the $50M award limit (Rules §7; not 29% of the total award).
- Geographic rule: project must primarily benefit the City and County of San Francisco (those who live and work in the city), with **no more than 25% of project activities** aimed at benefiting the broader Bay Area outside SF city limits.
- For-profit leads are eligible; award funds are then subject to **expenditure responsibility under IRC §4945(h)**, and all spending must serve charitable purposes with only incidental private benefit.
- Foreign-jurisdiction entities are listed as a category, but the FAQ frames eligibility as U.S.-based; **written confirmation is required** for a non-U.S. entity (e.g., a Bulgarian company).
- Applications **cannot be edited after submission**; submissions can be withdrawn.
- Individuals and single-member LLCs taxed as individuals **cannot** lead.

---

## 4. Top open decisions / unknowns surfaced by this packet (full register: `03-registers.md`)

1. **Registration status** - did any eligible entity register by Sept 11? (Go/no-go; DR-03)
2. **Legal applicant / Lead Organization** - entity type, jurisdiction, tax status, actual control of funds (DR-02)
3. **Beneficiary** - which defined SF population, inclusion/exclusion, geography, scale (DR-01)
4. **Single public outcome** - which one public result the portfolio serves (DR-07)
5. **Charitable frame** - cultural-installation program vs. commercial business with civic branding (DR-06)
6. **Intervention / participant pathway** - what participants actually receive beyond game access (DR-05/07)
7. **Funding scenario** - constrained / proposed / maximum request amount, from a cost model (DR-04)
8. **Outcome claim** - the highest claim supportable at E1-E4 (DR-05)
9. **San Francisco delivery capacity** - named people, locations, partners; currently none (DR-01/09)
10. **Platform rights** - ownership/licensing of code, art, audio, third-party components (DR-09)
11. **Post-grant durability model** - owner, payer, annual operating cost, retained access (DR-10)
12. **Peer-review owner** - who completes the mandatory ≥4 reviews Nov-Dec 2026 (DR-08)

Count: **12 open items surfaced**; of these, **10 are formal decision-register rows (DR-01…DR-10) in `03-registers.md`** - the register is the single source of truth for decisions. The remaining two items (participant pathway, SF delivery capacity) are resolved through DR-01/DR-05 as inputs rather than separate decisions.

---

## 5. Next actions (in order)

| # | Action | Owner | By |
|---|--------|-------|-----|
| 1 | Confirm whether any entity registered before Sept 11; if not, contact `boundless-sf@submittable.com` for an exception and record the answer in writing | Authorized officer (unnamed) | Oct 14-15 |
| 2 | Open the registered Submittable account and copy the exact application questions, word limits, and attachment requirements | Authorized officer | Oct 15 |
| 3 | Resolve the legal lead (entity documents, written eligibility confirmation for a non-U.S. entity) | Authorized officer | Before submission |
| 4 | Scope lock: choose beneficiary + one public outcome + charitable frame (DR-01, DR-06, DR-07) | Decision owner | Before any narrative drafting |
| 5 | Build participant pathway → platform boundary → claim ledger → first-year plan → unit-cost model (in that order) | Program + budget owners | After scope lock |
| 6 | **Do not** draft submission narrative until eligibility is confirmed and the packet reaches at least Draftable | Writer (not yet commissioned) | - |

If the team did **not** register, the correct output is a gap report, not a proposal draft (methodology stop condition).