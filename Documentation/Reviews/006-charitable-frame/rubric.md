# Rubric Review - Change 006 (Charitable Frame Decision Record)

**Reviewer:** Rubric reviewer (threefold review, facet 2 of 3)
**Subject:** DR-06 charitable frame decision state recorded as undecided as of 2026-10-14; frame options (a)-(c) with the six-question commercial-benefit test applied, **not chosen**; state propagated to the source case and prospectus
**Files reviewed:** `Documentation/Prospectus/03-registers.md` (live DR-06 row, §1.1 entry, options-detail block), `01-source-case.md` (rows 3, 4, 5, 10; ten-statement #7; revision record), `00-prospectus.md` (§1, §3.1, §4.2, §8, §10.1, §11), `Logs/changes.md`, `Plan/000-index.md`; plan `006-charitable-frame.md`; constitution `Logs/instructions.md` §1-11; export §"Separate the businesses", §"Choose a charitable frame", §"Commercial-benefit test", §"it's both"; `Refinement/00-alignment-matrix.md` Table B (charitable-use row)
**Date:** 2026-10-14 · **Round:** 1

## Score table

| Dimension | Score (1-5) | What would raise it one point | Defect |
|---|---|---|---|
| Clarity | 4 | Restructure the options-detail table's commercial-benefit-test column into a per-question grid (Q1-Q6 rows per option) so each question's outcome scans without re-reading the cell | None material. The six-question outcomes are inline prose inside one cell per option - correctly ordered Q1-Q6 with the decisive Q3 verdicts bolded (**passes by design** / **fails**), but per-question comparison requires re-reading |
| Consistency | 4 | Correct the section attribution of the identity contrast: "Only the first is likely to fit this competition" sits at the close of export §"Commercial-benefit test" (line 2473), not in §"it's both" (lines 2482-2484), whose body is "Answer skipped." | The §1.1 entry and the options-detail intro cite the identity contrast to §"it's both". The quote is verbatim and the file is right; the section label is one heading off. Otherwise options, the six questions, and the undecided state derive verbatim from the export and agree with every referenced packet location |
| Enforceability | 5 | - (nothing material) | None. Owner named (program lead + counsel roles with `[INFORMATION NEEDED: named persons; required to own the frame decision and the charity-law review; blocks Mechanism, Ambition - DR-06]` markers); decision rule explicit in five clauses (public benefit primary and defined; private benefit no more than incidental, rules §3/§8; every commercial feature passes the six-question test incl. the revenue-zero question; only (a)-type frames fit this competition); next action is three concrete numbered steps with the owner as party; zero positive claims of an adopted frame anywhere (verified) |
| Completeness | 5 | - (nothing material) | None. State, options with test outcomes, decision rule, needed evidence (seven items), owner, deadline, and consequence of delay all present in one contiguous block; the review model was applied (adversarial test §7.8 per option, owner test §7.3, evidence grades §5 with the status ungraded mirroring DR-11, plan V1-V10 verification; threefold review running before commit per §11.6 - git shows the change uncommitted) |

## Verdict: **PASS** (all dimensions ≥ 3)

Single highest-priority defect if reviewed as FAIL: n/a - no FAIL. The one defect (citation attribution of the identity contrast to §"it's both") is minor and non-blocking; the quoted content is verbatim and located in the same export file. It belongs in the next revision, not in this round's gate.

## Executor deviations from plan 006 (checked - all sensible)

| Deviation | What changed vs. plan quote | Sensible? | Basis |
|---|---|---|---|
| Added budget cell | `01-source-case.md` revision-record row (2026-10-14, DR-06): plan §3.6 quoted 7 cells; executor inserted `-` for "Budget affected" (8th column) | Yes | The header has 8 columns; the plan's quoted row would have failed the pipe-count check (plan V6). The `-` matches changes.md's "no budget affected" and the row's evidence cell ("no new figures"). Same deviation as 005, previously judged sensible |

## Verification evidence

| Check | Result |
|---|---|
| Six-question test verbatim from export | Confirmed - export lines 2464-2469 (charitable result; who pays/benefits; revenue-zero; advantage to company/advertisers; rule preventing excessive private benefit; public access if advertising disappears) match the options-detail Q1-Q6 cells in wording and order; Q3's decisive role quoted per export line 2471 ("If the honest answer to the third question is no, the feature probably belongs in the business plan rather than the grant narrative") |
| Frame text verbatim | Confirmed - §1.1 entry quotes export line 2432 verbatim ("Provide publicly accessible cultural and recreational game installations...") with the §"Choose a charitable frame" attribution |
| Identity contrast | Quote verbatim (export line 2473: "Only the first is likely to fit this competition") - but it closes §"Commercial-benefit test", not §"it's both" (body: "Answer skipped."); see Consistency defect. The "commercial and promotional effects do not by themselves establish the charitable project" basis of option (b)'s weakest assumption is corroborated by export line 2490 |
| Undecided state matches packet reality | Confirmed - no adopted frame anywhere: source-case rows 3/4/5/10 ("undecided"/"not chosen"), ten-statement #7 UNKNOWN; prospectus §1/§3.1/§4.2/§8/§10.1/§11; evidence-register rows C19-C20 (E4, untested); alignment-matrix Table B charitable-use row ("ONE public-benefit frame; businesses separated...; commercial-benefit test applied to each feature", decision owner program lead + counsel) - the §1.1 cross-reference list is accurate |
| Uncertainty language (§5) | Confirmed - "Undecided as of 2026-10-14", "options, not chosen", "no positive claim", "ungraded - no positive claim, mirroring DR-11" throughout all five files |
| Evidence-grade discipline | Confirmed - E1 on frame text/test/identity-contrast sourcing (verified against export); the status itself ungraded (no positive claim); matches §5 "a sentence may move down in confidence, but never up" and the DR-11/DR-01 precedent |
| Decision rule | Confirmed - public benefit primary and defined; private benefit incidental only (rules §3/§8, E1; Table B charitable-use row); six-question test incl. the revenue-zero question; only (a)-type frames fit (export line 2473) |
| Owner test (§7.3) | Confirmed - every next-action verb (apply, confirm, record) has program lead + counsel as party; named-person `[INFORMATION NEEDED]` markers preserved with blocks list |
| Adversarial test (§7.8) | Confirmed - every option (a)-(c) carries a weakest-assumption cell labeling the untested E4 assumption or the base-case consequence |
| No frame chosen (plan V1) | Confirmed - zero positive claims of an adopted frame; "all recorded, not chosen" and "none approved is the base case" in the live row, §1.1 entry, and options table; prospectus §4.2 heading carries the undecided state |
| No prohibited words (plan V7) | Confirmed - 0 hits in the five changed packet files; the single grep hit is the plan's own V7 command line quoting the pattern (self-referential, not a content violation) |
| Cross-file consistency | Confirmed - "Undecided as of 2026-10-14", owner program lead + counsel, deadline before scope lock (not achieved), gate effect Open (scope not locked), class Clarifying - identical across 03-registers §1.1, source-case rows 3/4/5/10 + revision record, prospectus §1/§3.1/§4.2/§8/§10.1/§11, changes.md, 000-index (status planned) |
| Exact file set (plan V8) | Confirmed - git status: exactly 5 modified (changes.md, 000-index.md, 00-prospectus.md, 01-source-case.md, 03-registers.md) + 1 untracked (006-charitable-frame.md); no other file touched, no deletions; change uncommitted, consistent with §11.6 review-before-commit |
| Change class (§9.2) | Confirmed - Clarifying (records a decision state; adds missing information; no frame adopted, so no scope change); consistent with 004/005 precedent. The Foundational example "Scope-lock decision (DR-01/06/07)" presumes a decision, which is absent here |
| Note (pre-existing, not introduced by 006) | Prospectus §11 row 5 owner cell reads "Decision owner" (aggregates DR-06 + DR-07; matches DR-07's register owner); plan §4.6 changed only the Decision-ref cell, so 006 neither introduced nor worsened this |