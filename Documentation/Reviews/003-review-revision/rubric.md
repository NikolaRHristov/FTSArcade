# Rubric Re-Review - Change 003: Constitution §11 Revision (Run Trigger, §9.2 Citation, Verbatim Questions)

Reviewed document: `Documentation/Logs/instructions.md` §11 (revised per plan 003: Edit A §11.2 verbatim questions, Edit B new §11.6 run trigger, Edit C §11.4 §9.2 citation).
Facet: rubric. Reviewer: rubric re-reviewer. Date: 2026-10-14. Round: 2 (re-review of review 002's rubric round on the revised §11 only).
Scope: revised §11 only; changes.md/index rows and deferred items are tracked in plan 003 §3, not re-scored here.
Standard: repo constitution (instructions.md §1-§10) and plan 001 conventions, as in review 002.

## Score Table

| Dimension | Score (1-5) | What would raise it one point | Defect (if any) |
|---|---|---|---|
| Clarity | 4 | Resolve the two dangling references (page-budget table in §11.1, data dictionary in §11.2/§11.4) to their source locations, and scope the six comprehension questions (Q5/Q6 are narrative-flavored) to non-narrative sections | Unchanged from 002: §11.1 cites "a page budget" and §11.2/§11.4 cite "the data dictionary" with no in-constitution location (sources live in the Reference export and Prospectus/03-registers.md §2, per plan 002 §6); §11.1 applies review to every section of every document, but an agent reviewing a protocol or plan section still has no rule for mapping Q5 ("requested amount")/Q6 ("after funding ends"). New §11.6 is clean: one topic, imperative verbs, names when and who. |
| Consistency | 5 | Nothing material within §11; the only residuals are recorded deferrals outside §11 (changes.md row 002 class, plan-002 sweep numbering, run-index path rule - plan 003 §3 items 5-7) | None in revised §11. 002 defect (a) is closed: the §11.4 revision bullet now reads "Editorial-class fixes (§9.2)" (line 168), matching plan 002's integration summary claim. §11.6's citations resolve and state accurately: "binding per plan 002 §2.1" matches that section's rule (T01-T12 verification gains a threefold review; changes.md row appended only after all facets pass or blocked), and "follow-on packet sweep runs per plan 002 §2.2" matches the sweep plan there. §11.2's "six questions" label matches exactly six items and §11.4's "all six questions"; lead-in preserved; §11.6's hooks to §11.2/§11.3/§11.4 and §11.4's §3/§9.2 citations are all consistent with §3, §9.1, §9.2, and plan-001 conventions. |
| Enforceability | 4 | Define the severity vocabulary for the §11.3 findings table (allowed values "blocker\|minor" still exist only in plan 002 §3's template) and replace the self-attested "without looking back" comprehension test with a checkable proxy | 002 defect (b) is closed: §11.6 names the master-index-row owner - "The orchestrator starts the run - assigns the three reviewers (§11.2) and adds the run's row to the master index (§11.3)". 002 defects (a) and (c) remain but are recorded deferrals (plan 003 §3 items 1 and 3), so they are tracked, not silent. §11.6 itself is fully enforceable: imperative, owner named (orchestrator), sequencing constraint explicit ("changes.md row is appended only after all three facets pass or a blocked status is recorded"). |
| Completeness | 5 | Nothing material; the only remaining gaps are the recorded deferrals (severity vocabulary, facet-template ownership, checkable comprehension proxy - plan 003 §3 items 1-3), each with owner and reason, which §11.4's blocker-recording rule already permits | 002's sole completeness defect - the missing run trigger - is closed. §11.6 states both when (every document-modifying change, before the version is committed; plan 001 T01-T12 verification and every later plan's execution, with plan 002 §2.1/§2.2 binding folded in) and who (the orchestrator, with §11.2/§11.3/§11.4 hooks). §11 now covers all four required elements plus lifecycle: roles with named steps (§11.2), artifacts and indexes (§11.3, README row), iteration policy with round cap and blocked status (§11.4), paragraph acceptance (§11.5), and run trigger (§11.6). |

## Verdict

**PASS** - all four dimensions score ≥ 3 (lowest: 4).

Highest-priority residual (recorded deferral, not a FAIL defect): define the severity vocabulary in §11.3 and give the comprehension pass test a checkable proxy, so the two self-referential enforcement gaps close.

## Review 002 Follow-ups: Closed vs Deferred

| 002 follow-up | Source | Status | Where |
|---|---|---|---|
| Run-trigger rule: who initiates a run and when | Rubric, Completeness | **Closed** | New §11.6 (when: every document-modifying change before commit, incl. plan 002 §2.1/§2.2 binding; who: orchestrator, with §11.2/§11.3/§11.4 hooks) |
| §9.2 citation in the §11.4 revision bullet | Rubric, Consistency (a) | **Closed** | Line 168: "Editorial-class fixes (§9.2)"; resolves plan 002's integration-summary claim |
| Master-index-row owner | Rubric, Enforceability (b) | **Closed** | §11.6: "The orchestrator starts the run ... adds the run's row to the master index (§11.3)" |
| §11.2 comprehension questions verbatim from the Reference export | Evidence check 1a (002's FAIL) | **Closed** | Verified byte-identical to export lines 789-794, modulo the two-space nesting indent (plan 003 Edit A rule) |
| Severity vocabulary for §11.3 findings table | Rubric, Enforceability (a) | Deferred | Plan 003 §3 item 1 (separate Clarifying change) |
| Facet-file template ownership | Rubric observation | Deferred | Plan 003 §3 item 2 (separate change) |
| "Without looking back" checkable proxy | Rubric, Enforceability (c) | Deferred | Plan 003 §3 item 3 (needs a checkable proxy; separate change) |
| changes.md row 002 class Foundational vs Clarifying | Rubric, Consistency (b) | Deferred | Plan 003 §3 item 6 (recorded; no action in 003) |
| §11.3 path rule vs live run layout | Rubric run-compliance note | Deferred | Plan 003 §3 item 7 (orchestrator decision on whether the path rule is literal) |
| Plan-002 sweep numbering ("003-review-sweep" taken) | Plan 002 §2.2 | Deferred | Plan 003 §3 item 5 (sweep plan becomes 004-review-sweep) |

## Justifications

- **Clarity (4):** The new §11.6 is a model of the section's style - single topic, imperative bullets, explicit references. The verbatim question block in §11.2 renders as a clean nested list under an unchanged lead-in. The section's core mechanics remain self-contained (slugify, paths, pass rules). The two dangling references and the narrative-scoped question mapping - the 002 Clarity defects - are untouched by 003, and neither blocks the main workflow, so 4 is unchanged.
- **Consistency (5):** Every 002 consistency defect is resolved inside §11, and the new text's cross-references were verified against their targets (plan 002 §2.1/§2.2 read and matched; §9.2 Editorial row exists at line 87; §11.2/§11.3/§11.4 hooks all land). No in-§11 inconsistency found; residual items are recorded deferrals outside §11 with owners and reasons (plan 003 §3), which satisfies rather than violates the constitution's own tracking rules.
- **Enforceability (4):** One of three 002 gaps closed (master-index owner, via §11.6). The two remaining gaps are precisely the items 003 scoped out as recorded deferrals, so they are tracked with owner and reason. §11.6 is the most mechanically checkable subsection yet added (grep-able trigger line, named owner, sequenced gate). 4 stands until the severity vocabulary and the comprehension-proxy items land.
- **Completeness (5):** The 002 rubric's single completeness gap is closed with a dedicated subsection that answers the follow-up verbatim. §11 is now self-sufficient on when a review starts, who starts it, and what gates completion; the four structural elements (roles, artifacts, iteration, integration) were already present and remain intact. Remaining items are refinements already recorded as deferrals, not missing elements - no defect remains for this dimension.

## Verification notes (rubric facet, this round)

- §11.6 present as the last subsection of §11 and last block of the file (line 184; file ends on its second bullet).
- §11.2 six questions on disk match export lines 789-794 character-for-character; `diff` shows only the intended two-space list indent.
- §11.4 revision bullet contains `(§9.2)` after "Editorial-class fixes"; no other new §9.2 hit in the file (single hit, line 168).
- §11.6's plan 002 citations verified against `Documentation/Plan/002-review-model.md` §2.1 (line 152) and §2.2 (line 171).