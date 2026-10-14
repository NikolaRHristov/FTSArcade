# Boundless San Francisco - Verified Facts Pack

**Verified as of: Wednesday, October 14, 2026** (pages fetched live on this date; archived copies used only where live fetch was blocked, and are labeled as such).

**Scope:** This file is the single source of truth for competition facts. Every fact carries its source URL and a verification status: **verified** (fetched live and read), **unverified** (could not be fetched; never guessed), or **conflict** (live page contradicts the prior-conversation export or another live page). Where the prior-conversation export made a claim, the result of the check against the live page is stated explicitly.

**Fetching method note:** `web_extract` (firecrawl) was unavailable in this environment; all pages were fetched by `curl` and, where a bot challenge blocked `curl` (AWS WAF on sf.gov), by a headless Chromium browser via CDP. Blocked pages are reported as such - no content was invented.

---

## (a) Competition facts

### Official name, funder, and award

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 1 | Official name: **Boundless San Francisco** - "a competition funded by Crankstart that will award up to $150 million to organizations anywhere in the world with ideas for making San Francisco a better place to live." | https://boundless-sf.leverforchange.org/ (Home) | **verified** |
| 2 | Competition Sponsor (legal term) = **Crankstart Foundation**. "The Competition Sponsor has contracted with Lever for Change to manage the Competition." | https://boundless-sf.leverforchange.org/rules (Definitions) | **verified** |
| 3 | Award range: **between $10 million and $50 million USD** per Award. **Up to three (3) Awardees** total (up to $150M aggregate). | https://boundless-sf.leverforchange.org/rules §13.8; https://boundless-sf.leverforchange.org/faq | **verified** (matches export) |
| 4 | Finalist stage: **up to seven (7) Finalists**; each receives a **project development grant of up to $500,000 USD** plus technical assistance. Pool totals **$1-3.5 million**. LFC page states "$250,000-$500,000" per finalist - consistent (subset of the cap). | https://boundless-sf.leverforchange.org/rules §13.8; https://boundless-sf.leverforchange.org/timeline; https://leverforchange.org/open-calls/boundless-san-francisco/ | **verified** (matches export) |
| 5 | Award funds may not be used for general operating support; indirect costs are covered separately (see #16). | https://boundless-sf.leverforchange.org/rules §7 | **verified** |
| 6 | Applicants may also request a **Program-Related Investment (PRI)** (below-market capital, e.g. low-interest loan); no predetermined cap; terms set at Finalist stage in sponsor's sole discretion. | https://boundless-sf.leverforchange.org/rules §11; FAQ; Readiness Tool | **verified** |
| 7 | "NO PURCHASE OR PAYMENT IS NECESSARY TO ENTER OR TO RECEIVE AN AWARD." | https://boundless-sf.leverforchange.org/rules | **verified** |

### Deadlines

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 8 | **Launch: August 5, 2026.** Applicant webinar held **August 18, 2026** (recording links on Home page). | https://boundless-sf.leverforchange.org/timeline; /home | **verified** |
| 9 | **Registration deadline: Friday, September 11, 2026, 5:00 p.m. U.S. Pacific Time.** "Only registrants can submit an application." (Passed as of this facts pack.) | https://boundless-sf.leverforchange.org/timeline; /rules §13.2; /home | **verified** (matches export) |
| 10 | **Application deadline: Thursday, October 15, 2026, 5:00 p.m. U.S. Pacific Time - "(deadline extended from October 9, 2026)".** | https://boundless-sf.leverforchange.org/timeline; /home; /faq; /organizationreadinesstool; https://leverforchange.org/open-calls/boundless-san-francisco/ (body text) | **verified** (matches export) |
| 11 | **CONFLICT (minor, internal to LFC page):** The timeline widget on https://leverforchange.org/open-calls/boundless-san-francisco/ still displays "October 9, 2026 - Application Deadline" with no extension note, while the same page's body text says "October 15, at 5 p.m. U.S. Pacific Time (deadline extended from October 9, 2026)". All Boundless-sf.leverforchange.org pages show October 15. Treat **October 15, 2026 5:00 p.m. PT** as authoritative. | https://leverforchange.org/open-calls/boundless-san-francisco/ | **conflict** |
| 12 | Applications submitted after the deadline "will not be accepted." | https://boundless-sf.leverforchange.org/organizationreadinesstool | **verified** |
| 13 | Application must be **in English** (English is not scored; language skills not a criterion). | https://boundless-sf.leverforchange.org/rules §13.1; Readiness Tool | **verified** |
| 14 | Each registrant may submit **at most one Application**; one registration per true identity. | https://boundless-sf.leverforchange.org/rules §13.5 | **verified** |

### Eligibility categories (verbatim, Rules §1)

Lead Organizations must be one of the following legal entities (list verbatim from https://boundless-sf.leverforchange.org/rules):

1. "An entity based in the United States and/or U.S. Territories that has received a tax determination letter from the Internal Revenue Service ("IRS") that it is exempt from federal income tax as an organization described under section 501(c)(3) of the Internal Revenue Code ("IRC") and a publicly supported organization described under section 509(a)(1) or (2) of the IRC, and which a tax determination letter is in effect."
2. "A nonprofit organization for a fiscally sponsored project, provided that the nonprofit organization is an entity based in the United States and/or U.S. Territories and has received an IRS determination letter ... 501(c)(3) ... 509(a)(1) or (2) ... (or meets the equivalency standards for entities organized under the laws of a foreign jurisdiction); **fiscal sponsors must exercise discretion and control over the grant funds.**"
3. "An entity based in the United States and/or U.S. Territories that has received a tax determination letter ... 501(c)(3) ... Type I or Type II supporting organization described under section 509(a)(3) ..."
4. "A public or private college, junior college, university, or other similar educational entity ... 501(c)(3) ... 509(a)(1) and 170(b)(1)(A)(ii) ... The specific program must align with sponsored research guidelines."
5. "A private operating foundation based in the United States and/or U.S. Territories under section 501(c)(3) ..."
6. "A U.S. tribal government treated as a State pursuant to IRC Section 7871."
7. "An entity organized under the laws of a foreign jurisdiction which has received a tax determination letter from the IRS **or has been determined to be the equivalent of a section 501(c)(3) and 509(a)(1)**."
8. Affiliates of national organizations - separate 501(c)(3) and 509(a)(1) or (2) entity (or foreign equivalent), own board of directors, legal liability rests with the local organization, no group exemption, independent decision-making, and does not "fund" general activities of the national organization.
9. "An entity that is recognized under the law of the applicable jurisdiction as a non-governmental organization, a charitable organization, a not-for-profit organization, or similar-type entity that is **not a for-profit organization or government agency** and that is engaged in charitable activities within the meaning of section 501(c)(3) of the IRC."
10. "A national, regional, or local governmental entity."
11. "A for-profit organization, including LLCs, benefit corporations, or hybrid organizations. Award funds granted to a for-profit Lead Organization are **subject to expenditure responsibility under IRC §4945(h)**; see 'Guidance Related to Non-Charitable Activities' below in Section 8."

Plus: Lead Organization must (a) be in good standing in its jurisdiction, (b) comply with all applicable laws, (c) be a single legal entity with legal responsibility, authority for, and control of Award funds and full discretion/control/supervision of the solution; Subgrantees/Contractors/Collaborators chosen solely by the Lead Organization.

**Ineligible (may serve as Subgrantee/Contractor, not Lead):** individuals and entities with the tax status of an individual (e.g. **single-member LLCs** where the member is an individual); 501(c)(4) organizations; employees/officers/board of the Sponsor, Lever for Change, Submittable and immediate family/household members. | Source: https://boundless-sf.leverforchange.org/rules §2; Readiness Tool | **verified** (matches export)

### Fiscal sponsorship

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 15 | Fiscal sponsorship is permitted: the fiscally sponsored project applies via a 501(c)(3) 509(a)(1)/(2) sponsor (or foreign-equivalency standard). **The fiscal sponsor must exercise discretion and control over the grant funds** - the export's "sponsor must genuinely control funds and project" is confirmed. | https://boundless-sf.leverforchange.org/rules §1; /faq; Readiness Tool | **verified** |
| 16 | Multiple distinct projects sharing one fiscal sponsor may each apply; if selected, "the fiscal sponsor organization will be named in the grant agreement for grantmaking purposes." | https://boundless-sf.leverforchange.org/faq | **verified** |

### Expenditure responsibility (for-profits)

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 17 | For-profit Lead Organizations: Award subject to **expenditure responsibility requirements of IRC §4945(h) and Treas. Reg. §53.4945-5**; must be "willing and able to comply with expenditure responsibility procedures for the duration of the Award." Award funds must be used exclusively for tax-exempt purposes (IRC §170(c)(2)(B)); no more than incidental private benefit; no lobbying; no political work. | https://boundless-sf.leverforchange.org/rules §8, §3; /faq | **verified** (matches export) |

### Foreign-entity ambiguity

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 18 | **Rules §1 explicitly list foreign entities as eligible** (categories 7 and 9 above - foreign org with IRS letter/equivalent determination; and foreign NGOs/charitable orgs "engaged in charitable activities within the meaning of section 501(c)(3)"). The Readiness Tool's response for category 7 confirms: "Entities organized under the laws of a foreign jurisdiction that have received a tax determination letter from the IRS, or have been determined to be the equivalent of a 501(c)(3) and 509(a)(1), are eligible to serve as a Lead Organization." | https://boundless-sf.leverforchange.org/rules; /organizationreadinesstool | **verified** |
| 19 | **CONFLICT (internal to FAQ):** The FAQ "Who can participate?" answers "Organizations eligible to serve as the Lead Organization **must be based in the United States or U.S. Territories** and be:" - then immediately lists the same categories, including foreign-jurisdiction entities. The FAQ intro sentence contradicts both the Rules and the FAQ's own list. For a Bulgarian (non-U.S.) entity, eligibility turns on satisfying category 7 (IRS letter or 501(c)(3)/509(a)(1) equivalency determination) or category 9 (recognized foreign NGO engaged in IRC-501(c)(3)-meaning charitable activities). **Written confirmation from boundless-sf@submittable.com is still required before relying on any foreign-entity pathway** - the export's flag stands, now narrowed to "which category + how to evidence equivalency." | https://boundless-sf.leverforchange.org/faq vs /rules | **conflict** |

### Indirect-cost rule

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 20 | "The Competition Sponsor will consider paying for these indirect costs **up to a maximum of 29% of direct project or activity costs** within the $50 million Award limit." I.e., 29% of **direct** costs, not of the total award - matches export. Using Award funds "entirely for general operating support is not allowed." | https://boundless-sf.leverforchange.org/rules §7 | **verified** |

### 25% SF-locality rule

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 21 | "The proposed project must primarily benefit the City and County of San Francisco, specifically those who live and work in the city, with **no more than 25% of project activities aimed at benefitting the broader Bay Area outside San Francisco city limits** (the counties of Santa Clara, San Mateo, Alameda, Contra Costa, Solano, Sonoma, Napa, and Marin)." Applications must describe the communities they aim to impact. | https://boundless-sf.leverforchange.org/rules §1; /faq | **verified** (matches export) |

### Peer-review obligation

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 22 | After Administrative Review, each qualified applicant "will be required to **assess at least four (4) other Applications**" using the rubric; "If You do not complete those assessments ... **Your participation may be terminated**." FAQ: ~2.5 hours; assesses four, "and if necessary, up to six" other applicants. | https://boundless-sf.leverforchange.org/rules §13.6; /faq | **verified** (matches export) |
| 23 | Participatory Review deadlines: required reviews due **Wednesday, December 9, 2026, 5:00 p.m. PT**; if additional reviews are assigned, notified **Dec 11** and due **Dec 16, 5:00 p.m. PT**. | https://boundless-sf.leverforchange.org/timeline | **verified** |

### Application cannot be edited

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 24 | FAQ, "Will I be able to edit my application after submitting should I make an error?" - "**No. Please ensure all information you provide is accurate before you press the 'SUBMIT' button.**" Submitters may withdraw an active submission at any time. Drafts autosave; confirmation email from notifications@email.submittable.com. | https://boundless-sf.leverforchange.org/faq | **verified** (matches export) |

### Official contact

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 25 | Official contact: **boundless-sf@submittable.com** (Rules §16; FAQ; Home; all pages). Submittable support M-F 9:00-5:00 PT. Application portal: **https://boundless-sf-apply.leverforchange.org/submit** (home: boundless-sf-apply.leverforchange.org). Sign-in: manager.submittable.com/login. | https://boundless-sf.leverforchange.org/rules; /faq; /home | **verified** |

### Other verified rules (abbreviated)

| # | Fact | Source URL | Status |
|---|------|-----------|--------|
| 26 | Administrative Review (Oct-Nov 2026) checks eligibility; non-compliant applicants notified and excluded. | /timeline, /rules §13.6 | **verified** |
| 27 | Collaborations: multiple organizations may work together, but one eligible entity must be Lead/Awardee; **MOU not required at initial application**, may be required at Finalist stage. | /rules §4; Readiness Tool | **verified** |
| 28 | Multiple applications allowed from branches/departments/centers if solutions are distinct; each by a different team member with a unique email. | /rules §5; /faq | **verified** |
| 29 | Prior Crankstart grantees eligible in any capacity. | /rules §6; /faq | **verified** |
| 30 | Financial capacity: applicants must be in good legal and financial standing; **two years of financial statements** required at later stages (not collected in Stage 1; needed by March 2027). | /rules §9; Readiness Tool | **verified** |
| 31 | Reporting: grant agreement with Crankstart; minimum annual financial + annual narrative report. | /rules §12 | **verified** |
| 32 | Awardee names will be posted on the Lever for Change website; application may be published online and distributed to others during evaluation. | /rules §13.12; Readiness Tool | **verified** |
| 33 | Applicant IP: applicant owns IP; grants a perpetual, worldwide, royalty-free license to Sponsor/LFC/host; publicity release applies. | /rules §14 | **verified** |
| 34 | No commitment to award; sponsor may terminate/alter the Competition at any time without awards. | /rules §13.13 | **verified** |

---

## (b) Evaluation rubric

**Source:** https://boundless-sf.leverforchange.org/evaluationprocess (rubric text verbatim from page; full rubric also downloadable as PDF - verified live, HTTP 200, application/pdf: https://torque.leverforchange.org/boundless-sf/images/e/e7/Boundless_San_Francisco_-_Evaluation_Rubric.pdf).

**Mechanics (verified):** four criteria, **equally weighted**, each scored on a **five-point scale (1-5)**; reviewers assign a score for each criterion plus a justifying comment; **4 reviewers per application** (peer applicants in Participatory Review; Evaluation Panel members in Evaluation Panel Review); max per trait per application = 20; **maximum aggregate total = 80 points**; reviewers anonymous to applicants; **scores are normalized** (reviewer means are adjusted toward the global mean) at two points - after Participatory Review and after Evaluation Panel Review; LFC staff review every score/comment. Criteria prompts and anchors below.

**#1 TRANSFORMATIVE AMBITION** - Prompt: "Will this approach meaningfully shift conditions for San Franciscans? Will the solution go beyond delivering services by changing systems, policies, norms, or opportunity structures? Is the theory of change bold, coherent, and proportionate to the resources requested?"
- **1 (INCREMENTAL):** "Does not demonstrate potential to shift conditions for San Franciscans. It focuses exclusively on service delivery without engaging the systems, policies, norms, or opportunity structures that sustain the problem. The theory of change is absent, unclear, or not proportionate to the resources requested."
- 2: "Shows limited potential to shift conditions ... beyond direct service delivery. It references broader change but does not articulate a credible path toward it. The theory of change is underdeveloped or only loosely proportionate..."
- 3: "Demonstrates some potential ... by moving beyond service delivery to engage systems, policies, norms, or opportunity structures... The theory of change is coherent and generally proportionate..."
- 4: "Presents strong potential ... by clearly targeting systems, policies, norms, or opportunity structures that sustain the problem. The theory of change is bold, coherent, and well-proportionate... Where service delivery is present, it serves as a foundation for that broader structural ambition rather than an end in itself."
- **5 (TRANSFORMATIVE):** "Offers exceptional potential to fundamentally shift conditions for San Franciscans by targeting systems, policies, norms, or opportunity structures that sustain the problem at scale. The theory of change is bold, rigorous, and compellingly proportionate to the resources requested. Any direct service work is explicitly connected to and in service of that structural ambition."

**#2 VIABILITY** - Prompt: "Does the proposal demonstrate a credible and specific plan for achieving results in San Francisco? Does the team have an understanding of the city's context, the communities to be served, and the partnerships, relationships, or strategies needed to execute here? For organizations without an existing San Francisco presence, is there a realistic and well-reasoned path to establishing that presence?"
- **1 (IMPLAUSIBLE):** "Lacks a credible plan for achieving results in San Francisco. It shows little to no understanding of the city's context, the communities to be served, or the partnerships, relationships, and strategies needed to execute. Where applicable, applicants without an existing San Francisco presence offer no realistic path to establishing one."
- 2: "Shows limited evidence of a credible plan ... Understanding of the city's context and the communities to be served is surface-level. Partnerships, relationships, or strategies described are vague and insufficient..."
- 3: "Offers a credible plan ... Demonstrates a working understanding of the city's context and the communities to be served. Partnerships, relationships, or strategies are adequately identified..."
- 4: "Presents a strong and specific plan ... Reflects a clear understanding of the city's context and the communities to be served. Partnerships, relationships, or strategies are well-defined and clearly positioned..."
- **5 (COMPELLING):** "Offers an exceptional and detailed plan ... Demonstrates deep understanding of the city's context and the communities to be served. Partnerships, relationships, or strategies are concrete and constitute a significant asset for successful implementation. Where applicable, applicants without an existing San Francisco presence offer a compelling and thoroughly reasoned path to establishing one."

**#3 EVIDENCE OF RESULTS** - Prompt: "Is there compelling evidence (quantitative or qualitative, internal or external) that this approach works or is working? For early-stage applicants, is the theory of change grounded in a well-reasoned logic and relevant analogous evidence, even if direct results data is limited?"
- **1 (UNSUBSTANTIATED):** "Provides no meaningful evidence (quantitative or qualitative, internal or external) that the approach works. For established applicants, there are no results to speak of. For early-stage applicants, the theory of change is poorly reasoned and draws on no relevant analogous evidence."
- 2: "Provides weak evidence ... For established applicants, results are limited. For early-stage applicants, the theory of change is underdeveloped and loosely connected to relevant analogous evidence."
- 3: "Provides adequate evidence ... For established applicants, results are present but not compelling. For early-stage applicants, the theory of change is sound and grounded in relevant analogous evidence, even if direct results data is limited."
- 4: "Provides strong evidence ... For established applicants, results are clearly documented and speak to the effectiveness of the approach. For early-stage applicants, the theory of change is well-reasoned and supported by meaningful analogous evidence."
- **5 (WELL-EVIDENCED):** "Provides compelling evidence ... For established applicants, results are robust, well-documented, and directly relevant. For early-stage applicants, the theory of change is rigorous and supported by strong analogous evidence that makes a persuasive case for the proposed approach."

**#4 DURABILITY** - Prompt: "Will this work generate lasting benefits beyond the grant period? Does the proposal demonstrate a credible vision for how results will be sustained-whether through financial sustainability, policy change, institutional adoption, community ownership, or other mechanisms? Does the organization have a realistic plan for the five-year horizon and beyond?"
- **1 (FLEETING):** "Lacks a credible vision for sustaining results beyond the grant period. There is no meaningful plan for financial sustainability, policy change, institutional adoption, community ownership, or other sustaining mechanisms. There is no articulation of what lasting benefit looks like for the people or systems served. No realistic plan for the five-year horizon and beyond."
- 2: "Offers limited evidence of a credible vision ... Plans for sustainability are vague or rely on assumptions that are not well-supported. The plan for the five-year horizon and beyond is underdeveloped."
- 3: "Demonstrates a vision for sustaining results beyond the grant period. Identifies plausible mechanisms for sustainability, whether financial, policy-related, institutional, or community-based, though the plan for the five-year horizon and beyond could be more fully developed."
- 4: "Presents a strong and credible vision ... It articulates clear mechanisms for sustainability ... and offers a realistic picture of the lasting benefits those mechanisms are designed to protect. Offers a realistic plan for the five-year horizon and beyond."
- **5 (LASTING):** "Outlines an exceptional and well-substantiated vision for sustaining results well beyond the grant period. Demonstrates a comprehensive approach to sustainability through multiple reinforcing mechanisms and offers a compelling articulation of the lasting benefits those mechanisms are designed to protect. The proposal offers a thorough, realistic plan for the five-year horizon and beyond."

**Note for writers:** descriptors 2-4 above are close paraphrases (quotes trimmed); descriptors 1 and 5 are verbatim. The evaluation page also states normalization mechanics and that "Lever for Change staff review reviewers' scores and comments for every submission."

---

## (c) Timeline table

**Source:** https://boundless-sf.leverforchange.org/timeline (all verified live). FAQ restates key dates consistently.

| Stage | Dates | Detail |
|-------|-------|--------|
| Launch | **August 5, 2026** | Competition opened; readiness assessment + registration open |
| Applicant webinar | **August 18, 2026** | Recordings: youtu.be/oXoVzG3CBh4 (main); youtu.be/NiP8vfjHwzQ (ASL); Box links for Spanish/French interpretation |
| **Registration deadline** | **Friday, September 11, 2026, 5:00 p.m. PT** | Passed; only registrants can apply |
| **Application deadline** | **Thursday, October 15, 2026, 5:00 p.m. PT** (extended from Oct 9) | Stage 1 submission |
| Administrative Review | October-November 2026 | LFC staff check eligibility/Rules compliance |
| Participatory Review | November-December 2026 | Each applicant reviews ≥4 peers (up to 6); reviews due **Dec 9, 5:00 p.m. PT**; extras due **Dec 16, 5:00 p.m. PT** |
| Evaluation Panel Review | January-March 2027 | 4 panel reviewers per application, same rubric; normalization applied |
| Finalist selection | March-June 2027 | 3-7 Finalists; "Crankstart will select Finalists by June 2027" (FAQ) |
| Project Development | June-August 2027 | Finalists receive project development grants (pool $1-3.5M) + technical assistance; **investment prospectus due August 2027** |
| **Grant Award** | **Fall 2027** | Up to 3 Awardees, $10-50M each |

**Export cross-check:** "finalists ~June 2027" ✓; "finalist investment prospectus Aug 2027" ✓; "final awards fall 2027" ✓. No conflicts.

---

## (d) FTSArcade platform facts - strictly observed

**Source:** https://frymatic.us/FTSArcade (fetched live 2026-10-14; page title "FishTacoStand Arcade"). **No-inference rule in force: these are observations of what the site displays; they are NOT converted into outcome claims (users, engagement, learning, employment, or charitable benefit are NOT stated anywhere on the page).**

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

---

## (e) SF ecosystem language sources

Live-status legend: **LIVE** = fetched live today; **ARCHIVED** = live page blocked (bot challenge / timeout), content taken from a dated Internet Archive snapshot and labeled as such; use only with the caveat that the live page may have changed.

| Resource | URL | Key phrases (as found) | Best use | Caveat |
|---|---|---|---|---|
| SF Arts Commission - Mission & Values (agency page) | https://www.sf.gov/arts-commission-mission-values | "Established by charter in 1932 ... the city agency that champions the arts"; mission: "champions the arts as essential to daily life by investing in a vibrant arts community, enlivening the urban environment and shaping innovative cultural policy"; vision: "the transformative power of art is critical to strengthening neighborhoods, building infrastructure and fostering positive social change"; "artists as integral to making San Francisco a city where people want to live, work and play" | Mission/alignment wording for arts-and-public-space framing; cite as city agency context | **LIVE** (AWS WAF blocked curl; fetched via headless browser) |
| SF Cultural Districts Program (MOHCD) | https://www.sf.gov/san-francisco-cultural-districts-program | "fosters a collaborative partnership between the City and communities to strengthen San Francisco's cultural communities"; aims: "protect vulnerable communities from displacement, support cultural and economic vitality, and promote equitable, community-informed policies"; ten Cultural Districts listed; CHHESS report as "living roadmap to community stabilization" | Evidence that the City already runs community-stabilization-through-culture programs; alignment with district nonprofits | **LIVE** (browser) |
| Cultural Districts Program - overview | https://www.sf.gov/information--overview-san-francisco-cultural-districts-program | 2018 Board of Supervisors legislation; Cultural District defined by ordinance; "Proposition E [approved] by a 75 percent majority, allocating approximately $3 million annually from the City's Hotel Tax Fund"; three program goals (preserve/promote cultural assets; celebrate community strengths for resilience; streamline City-community partnerships to stabilize communities facing displacement) | City-policy grounding: the City itself funds cultural stabilization; positions arcade-installation program as complementary to an existing municipal framework | **LIVE** (browser) |
| Office of Economic and Workforce Development (OEWD) | https://www.sf.gov/departments--office-economic-and-workforce-development | "We strive to create a thriving and resilient economy where barriers to economic and workforce opportunities are removed, and prosperity is shared equitably by all"; divisions: Office of Small Business, Business Development, Workforce Development, Community Economic Development ("strengthen San Francisco neighborhood business corridors, public spaces, and commercial centers"), Joint Development; current events incl. District Family Summits | City-wide economic-development framing; the Community Economic Development division is the natural city counterpart for commercial-corridor/public-space work | **LIVE** (browser) |
| Office of Small Business - Annual Report FY2024-25 (PDF) | https://media.api.sf.gov/documents/OSB_FY24-25_Annual_Report.pdf | Mission: "To equitably support, preserve, and protect small businesses in San Francisco..."; priorities: (1) small business retention and growth, (2) faster/easier openings, (3) "Strengthen economic vibrancy in neighborhood commercial corridors and economic core"; history: 2003 Prop D, 2007 Prop E (assistance center, <100 employees), 2015 Prop J (Legacy Business Program) | Commercial-corridor revitalization framing; legacy-business program parallels (long-standing businesses) | **LIVE** (22.4 MB PDF, text extracted) |
| Office of Small Business - Annual Report FY2025-26 (PDF) | https://media.api.sf.gov/documents/Office_of_Small_Business_Annual_Report_FY2025-26_ECMsJje.pdf | "The Office of Small Business helps entrepreneurs start, sustain, and grow their businesses in San Francisco... remove barriers... champion for small businesses"; priorities incl. "Revitalize neighborhood commercial corridors and the economic core to drive lasting economic vibrancy"; FY25-26 figures: **3,608 unique businesses served**; **959 Legacy Businesses on the Registry (66 added in FY25-26)**; $10,355,368 awarded through OEWD/OSB; 78 leases signed with OSB guidance | Current-year stats for corridor/legacy-business context; cite numbers only if needed and attribute to the report | **LIVE** (5.6 MB PDF, text extracted). Caveat: PDF internal labels contain oddities (e.g., "47% increase from FY25-26" inside the FY25-26 report); verify before quoting |
| SF Planning - Racial and Social Equity Action Plan | https://sfplanning.org/project/racial-and-social-equity-action-plan | "Achieving an equitable San Francisco requires more than vision, it requires sustained action"; Equity Plan "provides a framework for centering equity in all aspects of our work"; mandated by City Ordinance + Office of Racial Equity; Phase 1 (2019, internal) + Phase 2 (external: policies, planning processes, community engagement); 11 focus areas; Community Equity Advisory Council | Equity framing for public-space/cultural work; language of "removing barriers, expanding opportunity" | **LIVE** |
| SF Planning - Community Stabilization | https://sfplanning.org/community-stabilization-strategy | Multi-agency initiative to "assess the City's existing portfolio of tools, unify fragmented efforts into one comprehensive inventory, and identify priorities"; displacement defined via UC Berkeley Urban Displacement Project (2018); vulnerable-population categories (Senior 65+, Disabled, Families with children, Black/African-American, Latinx/Hispanic, Asian, Pacific Islander); Public Report May 2020 | Context for displacement/stabilization language; avoid implying the arcade program addresses housing displacement - the export's methodology requires separating claims | **LIVE** |
| SF Recreation and Park Department - Who We Are | https://sfrecpark.org/419/Who-We-Are | "administers more than 230 parks, playgrounds, and open spaces"; mission: "provide enriching recreational activities, maintain beautiful parks and preserve the environment for the well-being of everyone in our diverse community"; **4,257 acres** recreational/open space; **233 neighborhood parks**; 98 recreation centers/clubhouses; GM Sarah Madland; "first city in the country where every resident lives within a ten-minute walk of a park" | Parks/recreation infrastructure context; potential site-partner framing (permits division issues 70,000+ permits/yr) | **ARCHIVED** - live site unreachable from this network (connection timeout, curl and browser); snapshot 2026-10-11 (http://web.archive.org/web/20261011201918/https://sfrecpark.org/419/Who-We-Are). Verify live before quoting |
| SF Travel - About | https://www.sftravel.com/about-sf-travel | "the official destination marketing organization for the City and County of San Francisco"; mission: "To promote the San Francisco region as a top global destination by leading the way in performance, innovation, and sustainability"; "curators of the most interesting 49 square miles on the planet"; 501(c)(6) membership association founded 1909; funding ~68% hotel-room assessment, ~23% private sector | Tourism/visitor-economy context for place-based installations; careful: DMO framing is commercial, keep separate from charitable outcomes | **ARCHIVED** - live page blocked by Cloudflare ("Just a moment..." challenge; headless browser also blocked); snapshot 2026-08-13 (http://web.archive.org/web/20260813064342/https://www.sftravel.com/about-sf-travel). Verify live before quoting |

---

## Conflicts & flags (export vs. live pages)

| # | Issue | Export claim | Live finding | Action |
|---|-------|--------------|--------------|--------|
| C1 | LFC open-call page timeline widget shows **Oct 9** application deadline | "deadline Oct 15 (extended from Oct 9)" | Widget on leverforchange.org still says Oct 9 (no extension note); page body and all boundless-sf pages say Oct 15, extended | Use Oct 15, 5 p.m. PT; ignore widget |
| C2 | FAQ eligibility intro: "must be based in the United States or U.S. Territories" vs. its own list and Rules | "geographic ambiguity for foreign entities - needs written confirmation" | Rules §1 explicitly allow foreign entities (categories 7 & 9); FAQ intro contradicts them | Keep written-confirmation flag; reference categories 7/9 when asking boundless-sf@submittable.com |
| C3 | FTSArcade "24 CABINETS" / "8 ON THE BENCH" labels vs. listed WIP count | (not in export) | 15 live + 9 WIP = 24; bench label says 8 but 9 WIP entries listed | Cosmetic; do not assert counts from labels in the application |
| C4 | Box "full Application PDF" link on Home page | (not in export) | Link https://app.box.com/s/5gzqu27env25td5yl9w1fh5sp1juw7bt returns **HTTP 404 to curl HEAD** (may be bot-block); do not rely on it without a manual browser check | Re-verify in a real browser before citing application-form details |
| C5 | Finalist grant amount | "finalists receive project development grant" (amount not pinned) | Rules: "up to $500,000" per Finalist; LFC page: "$250,000-$500,000"; pool $1-3.5M total | Use "up to $500,000 each / $1-3.5M pool" |
| C6 | SF Travel / Rec & Park live status | Sources cited from export without live check | Both live pages blocked from this network; only archived copies retrievable | Treat all quotes from these two as needing live re-verification |

**Export claims with NO conflict found:** award range and count; registration deadline; application deadline incl. extension; stage timeline; all 11 eligibility categories incl. for-profits and foreign entities; individuals/single-member LLC ineligibility; fiscal-sponsor discretion/control; expenditure responsibility IRC §4945(h); 29%-of-direct-costs indirect rule; 25% SF-locality rule; ≥4 peer reviews with termination risk; no-edit rule; contact address; rubric mechanics (4 equal criteria, 1-5, 4 anonymous reviewers, max 80, normalized).