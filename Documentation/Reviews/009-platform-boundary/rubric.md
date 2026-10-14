# Rubric review - change 009 (platform boundary)

**Reviewer facet:** Rubric (threefold review)
**Artifact reviewed:** `Documentation/Prospectus/07-platform-boundary.md`
**Design authority:** `Documentation/Plan/009-platform-boundary.md` (§2.2 binding spec; file matches it verbatim)
**Date:** 2026-10-14
**Verdict: PASS**

## Score table

| Dimension | Score (1-5) | What would raise it one point | Defect |
|---|---|---|---|
| Clarity | 5 | - (at ceiling) | Minor: the outside-services set is enumerated three ways - 9 functions in §1.2, 8 rows (with Evaluation) in §2, "evaluate participants" in the §2 reading note. Reconciling the lists requires noticing the Evaluation row exists only in the table. Cosmetic; the boundary itself reads unambiguously at a glance (bolded status, 3-column table, reading notes). |
| Consistency | 4 | Source the Evaluation/outcome-measurement outside row to W-10/DR-07 in §1.2 so the does-not list and the §2 table enumerate the same set; replace "counsel" with a delivery-map role label (or define it as one). | (a) §2 outside row **Evaluation / outcome measurement** is not among the §3.2 excluded functions; all 9 §3.2 items are present (safeguarding+pastoral and advertising+business-selection combined), this row is an extra 10th, grounded in W-10/DR-07 but absent from §1.2's does-not list. (b) Provider cell "Program lead + counsel" names a role not present in delivery-map W-04..W-10 (counsel appears nowhere there). Both are extensions, not contradictions, and both are verbatim in the design authority §2.2 - design-level, not execution-level. |
| Enforceability | 5 | - (at ceiling) | None. Every outside cell is a marker + role; 16 inline markers follow instructions.md §5 format (`[INFORMATION NEEDED: <owner>; why; decision blocked]`); 0 prohibited words (incl. "unique"), 0 dollar figures, 0 person names, 0 org names beyond "TBD" role labels, 0 causal claims (the only "leads to" hit sits inside a non-claim prohibition quoting `00-prospectus.md` §4.1); §3 SF sources match facts-pack §(e) rows and LIVE/ARCHIVED statuses incl. the C6 caveat; §5 non-claims present with sources. |
| Completeness | 5 | - (at ceiling) | None material. All six required elements present: definition (§1), boundary table (§2), SF dependencies (§3), unknowns (§4 BU-01..BU-11 with owner/why/blocked/unblocks), non-claims (§5), decision gate (§6) plus revision record (§7). Minor: "running-route effects" (an E5-removed claim, `01-source-case.md` row 7) is not restated among the §5 non-claims - 5 of 6 E5 items covered; the section is not asserted exhaustive, so the cited sources remain accurate. |

## Verification evidence (checked against sources)

| Check | Source | Result |
|---|---|---|
| Inside cells verbatim | facts-pack §(d) facts 1-11 + does-NOT-show paragraph | 11/11 rows + paragraph byte-identical |
| §1.2 does-not list | `00-prospectus.md` §3.2 excluded-functions row | 9/9 items verbatim |
| Outside cells vs §3.2 | `00-prospectus.md` §3.2 | 9/9 §3.2 items present (2 pairs combined) + 1 Evaluation row not in §3.2 |
| Inference-rules quote | `00-prospectus.md` §3.2 (line 78) | Verbatim, incl. "**not** ability to deliver education or social services" |
| Non-claims sources | §3.2 non-claims row; source-case row 7 (E5); facts-pack does-NOT-show; registers DR-07 rule | Rows accurate; 5/6 E5 items covered ("running-route effects" omitted) |
| Provider roles | `04-delivery-and-budget.md` W-04..W-10 | W-05/W-06/W-10/W-08/W-09/W-04/W-07 labels match exactly; "counsel" is extra |
| Undecided-state propagation | `03-registers.md` §1.1 | DR-01/DR-06/DR-07 all "Undecided as of 2026-10-14"; propagated in preamble, §1.3, §2, §3, §6; gate §6 lists all three |
| T05/T06 linkage | `06-participant-pathway.md` | T05→T06 feed and preamble marker house-style identical |
| Marker count/format | instructions.md §5; plan §2.3 | 17 `[INFORMATION NEEDED:` grep hits = 16 inline markers + 1 status-line format description; each marker has owner + why + blocked decision |
| Prohibited words / figures / causality | instructions.md §6; plan V6/V7/V10 | 0 prohibited words incl. "unique"; 0 dollar figures; no causal claim (only prohibition-quote hit) |

## Verdict

**PASS** - all four dimensions ≥ 3 (Clarity 5, Consistency 4, Enforceability 5, Completeness 5). The artifact is an enforceable, E1-grounded boundary framework with accurate verbatim sourcing throughout. The two consistency deviations (the Evaluation outside row; the "counsel" provider label) are written into the design authority's binding spec §2.2 and executed verbatim - they are source-grounded extensions, not contradictions, and are non-blocking. Highest-priority follow-up (non-blocking): on gate opening, align §1.2's does-not list with the §2 outside column (add evaluation) and add "running-route effects" to §5.