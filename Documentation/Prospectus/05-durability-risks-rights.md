# Durability, Risk Register, and Rights Schedule - FTSArcade / Boundless San Francisco

**Version:** S0 · **Date:** 2026-10-14
**Rules:** A risk without a decision trigger is only a description. A post-grant benefit must have an owner other than "the community" unless a specific community body is defined. All asset ownership is **unknown** until the rights schedule is completed - the export flags IP review as particularly important for a game platform, and the competition rules require appropriate rights and licenses for third-party material included in the application.

---

## 1. Post-grant owner / operating model

**Status: not defined.** The methodology requires: named owner, operating cost, revenue or adoption mechanism, and retained access.

| Element | Required | Current status |
|---|---|---|
| Who legally controls the project and funds | Named entity with actual control | `[INFORMATION NEEDED: authorized officer; entity + written confirmation - DR-02]` |
| Who owns/licenses the technology | Named owner(s), license scope | **Unknown** - see rights schedule (§3); `[DR-09]` |
| Who pays operating costs after the grant | Named payer + annual cost | `[INFORMATION NEEDED: executive owner; operating-cost model - DR-10]` |
| How public access is retained | Access rule + responsible party | `[INFORMATION NEEDED: program lead; free-access rules - DR-06]` |
| What survives if the company changes or exits | Asset + owner + license continuity | `[INFORMATION NEEDED: rights owner; assignment/continuity terms - DR-09]` |
| What happens to access if advertising/commerce disappears | Contingency + rule | `[INFORMATION NEEDED: budget owner; commercial-benefit test outcome - DR-10]` |

**Candidate mechanisms (options only, per methodology's standard of proof):** commercial revenue (cabinet sales, ad space, QR referrals) is *being investigated* as one sustainability mechanism - but "intention to seek future funding" is not a sustainability plan, commercial revenue cannot become the project's real purpose, and open-source code or free access alone is not a complete operating plan. Institutional adoption and public funding are unnamed options.

**Commercial-benefit test (apply to every revenue feature before it enters the budget):**
1. What charitable result does it produce?
2. Who pays, and who benefits?
3. Would the feature still belong if it generated no revenue?
4. Could it advantage the company or advertisers more than the public?
5. What rule prevents excessive private benefit (for a for-profit lead: IRC §4945(h) expenditure responsibility)?
6. What happens to public access if advertising disappears?

If the honest answer to question 3 is "no," the feature belongs in the business plan, not the grant narrative.

---

## 2. Risk register (7 categories; each requires a decision trigger)

| Risk category | Question | Candidate response | Decision trigger (what result → what action) | Owner | Status |
|---|---|---|---|---|---|
| **Demand** | Will intended participants enroll? | Pilot recruitment threshold before expansion | Enrollments below [X] in pilot period → reduce cohort, change channel, or revise beneficiary (DR-01) | Program lead | Trigger thresholds `[INFORMATION NEEDED: program lead]` |
| **Delivery** | Can staff deliver the model? | Training and maximum caseload | Facilitator caseload/session quality below standard → pause cohort; do not expand | Program lead | No staff named |
| **Mechanism** | Will activities produce outcomes? | Staged evaluation before scaling | Pre-registered outcome metric misses [threshold] → correct method or redesign intervention before scaling | Evidence reviewer | No outcome chosen (DR-05) |
| **Adoption** | Will institutions continue it? | Early adoption commitments or alternative owner | No adoption commitment by [date] → pursue named alternative owner (DR-10) | Executive owner | No institutions named |
| **Technical** | Will the platform support delivery? | Acceptance criteria + non-platform fallback | Acceptance test fails → manual fallback or delay launch; feature stays outside prospectus until tested | Technical owner | No acceptance tests defined (W-04) |
| **Financial** | Will costs exceed assumptions? | Trigger for redesign or reduced cohort size | Cost model variance > [X%] → resize scenario or request (DR-04) | Budget owner | No cost model |
| **Control** | Can the lead supervise funds and partners? | Approval rights, audit trail, segregation of duties | Control finding in [review period] → remediation plan; unresolved → stop spending | Authorized officer | Lead unresolved (DR-02) |
| **Eligibility/registration** (added, decisive) | Is there a valid route to submit? | Written confirmation or exception | No registration/exception by Oct 15 → stop drafting; gap report only (DR-03) | Authorized officer | **Immediate go/no-go** |

**Scoring note:** risks are scored by their effect on the project logic, not by general seriousness. Each risk must be matched to a design choice, contingency, or evaluation question in the prospectus.

---

## 3. Rights schedule

**Status: all ownership/licensing **unknown** unless marked otherwise.** The export notes "We own everything" is not a sufficient basis; the rules require appropriate rights for third-party material, and IP review is flagged as particularly important for a game platform. Complete before submission (DR-09).

| Ref | Asset | Owner | License | Restriction | Third-party components | Needed information |
|---|---|---|---|---|---|---|
| R-01 | Platform source code (site, games, lobby) | **Unknown** | **Unknown** | **Unknown** | **Unknown** | `[INFORMATION NEEDED: rights owner; repo provenance, contributors, contributor agreements]` |
| R-02 | Game titles and gameplay code (15 live + 8 WIP titles) | **Unknown** | **Unknown** | **Unknown** | **Unknown** | `[INFORMATION NEEDED: rights owner; per-title provenance]` |
| R-03 | Artwork, sprites, cabinet art | **Unknown** | **Unknown** | **Unknown** | **Unknown** | `[INFORMATION NEEDED: rights owner; art assets, artist agreements, AI/asset-store provenance]` |
| R-04 | Audio (cabinet SFX, crowd ambience, jukebox source) | **Unknown** | **Unknown** | **Unknown** | crowd.mp3 and any stream/URL config noted on site | `[INFORMATION NEEDED: rights owner; sample licenses, stream licensing, music licensing scope]` |
| R-05 | Branding (FTS Arcade / FishTacoStand Arcade name and marks) | **Unknown** | **Unknown** | **Unknown** | n/a | `[INFORMATION NEEDED: rights owner; trademark status]` |
| R-06 | Third-party libraries/frameworks and their licenses | **Unknown** | **Unknown** | **Unknown** | **Unknown - must be inventoried** | `[INFORMATION NEEDED: technical owner; dependency license audit]` |
| R-07 | Running-route data (claimed by team) | **Unknown** | **Unknown** | **Unknown** | Data source, collection method, permissions | `[INFORMATION NEEDED: research lead; source, date, permissions, relevance - no claim may use it until documented]` |
| R-08 | Landmark/business depictions in future games | **Unknown - none licensed** | **Unknown** | **Unknown** | Property owners / rights holders | `[INFORMATION NEEDED: program lead; permission from owners or responsible authorities - DR-06]` |
| R-09 | Future grant-funded work product | **Undefined** | **Undefined** | **Undefined** | Grant agreement terms | `[INFORMATION NEEDED: authorized officer + counsel; IP terms in any grant/sponsorship agreement]` |

**Contractual coverage needed** (for any fiscal-sponsor or partnership arrangement, per export): budget authority; program accountability; staff/contractor hiring and conflicts of interest; reporting; technology/IP use rights and term; termination (remaining funds, unfinished work, participant commitments). Proposed negotiation points - not required attachments, but the lead must genuinely control the project and funds; "receive the money and immediately pass it all to us" is not acceptable.

**Ownership documentation standard (per export):** asset, owner, license, restriction - with written proof for each. Fields marked unknown must literally say "unknown"; a blank is not permission to infer.

---

## 4. Governance controls for a for-profit lead (if selected - DR-02)

- Documented charitable purpose and permitted-use budget
- Project-specific accounting and spending controls
- Financial and outcome reporting procedures
- Policies for owner compensation, related-party transactions, and IP licensing
- Procedures to identify and prevent prohibited spending
- U.S. nonprofit-tax attorney and accountant review (recommended, not a substitute for the grant agreement)

---

## 5. Review and audit sequence (run at each version, in order)

1. Eligibility audit (lead, authority, geography, registration, charitable use) - **currently fails: DR-02/DR-03 unresolved**
2. Logic audit (beneficiary, intervention, mechanism, outcome agree) - **fails: no beneficiary/intervention**
3. Evidence audit (every causal statement has a grade and limitation) - **passes for E1 rows; causal rows E4 with tests pending**
4. Operations audit (capacity, timeline, partner status support the plan) - **fails: no named capacity**
5. Financial audit (costs, scenarios, request agree) - **fails: no cost model**
6. Traceability audit (paragraphs map to claims and figures) - not applicable at S0
7. Compression audit - not applicable at S0
8. Sign-off audit (unresolved items cannot affect a central claim) - **fails; signatory cannot approve at S0**

The correct current output is this gap-identification packet, not a proposal draft (methodology stop conditions apply).