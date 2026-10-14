# Operating Protocol - Instructions for All Agents Working in This Repo

## 1. What this repo is

Plans only. The repo holds PLANS of what the team will build - formatted, presented, and refined neatly over versions, one commit per version. No email drafting. No promotional content drafting. If a task asks for either, stop and report the protocol violation.

## 2. The four operating rules

- **R1** No drafting - see §1. Every artifact is a plan, a register, a log, or a refinement of one.
- **R2** Delegation - the orchestrator does not manage content; it re-orders and delegates. Every change to a document is delegated: FIRST a pre-plan agent designs the change (writes Plan/NNN), THEN an execute agent implements it. One step of separation for every change, every time.
- **R3** Progress is saved after each change in SEPARATE files: planning steps, research steps, instructions, and changes - so later commits can be distilled easily.
- **R4** Writing quality - a chosen, consistent style (this spec); validity checks applied always (§5-§7).

## 3. Delegation model

- **pre-plan agent:** designs the change, writes `Documentation/Plan/NNN-*.md`, never edits packet documents.
- **execute agent:** implements the approved plan exactly, appends the changes.md row, never commits.
- **orchestrator:** re-orders and delegates, reviews, commits exactly one commit per version (`docs(grant): <change>`). Agents never commit, never push.
- **review agents:** three independent reviewers per section (comprehension, rubric, evidence - see §11); they report findings and verdicts only, never revise content.

## 4. Commit discipline

One commit per version. Message: `docs(grant): <change>`. The commit is made by the orchestrator only, after the execute agent's handoff.

## 5. Evidence & uncertainty language

Evidence grades E1-E5 on every material claim (definitions copied verbatim from the Reference export, writing methodology section):

| Grade | Meaning | Permitted treatment |
| :-- | :-- | :-- |
| E1 | Direct evidence from this project and population | State as demonstrated, with metric and limitation |
| E2 | Direct evidence from a closely comparable program | State similarity and relevant differences |
| E3 | Relevant analogous evidence | Use to support the mechanism, not identical outcomes |
| E4 | Plausible but untested assumption | Label as an assumption and include a test |
| E5 | Insufficient support | Remove from the prospectus |

A sentence may move down in confidence, but never up. For example, an E3 finding cannot be rewritten as "proven." If removing an E5 claim damages the project logic, the project design - not the prose - needs revision.

- Partner statuses: confirmed / in discussion / proposed - never a bare partner name without a status.
- Unknowns: `[INFORMATION NEEDED: <owner>; why; decision blocked]` - never silently resolved.
- Uncertainty phrases (use verbatim):
  - "As of [date], [source] shows…"
  - "Comparable evidence suggests…"
  - "The project will test whether…"
  - "The planning target is…"

## 6. Prohibited words & phrases

- revolutionary, world-class, unique, cutting-edge
- empower / unlock / transform - only with a defined change
- scalable - only with a unit cost
- sustainable - only with a named payer
- "partners include" - when the list is incomplete
- "data shows" - when the statement is an assumption

## 7. Editing tests (validity) - apply to every document

- **Deletion test:** Remove FTSArcade from the paragraph. If no intelligible intervention remains, the project is underdefined.
- **Substitution test:** Replace the beneficiary with a different city. If no San Francisco-specific facts remain, viability is too generic.
- **Owner test:** Underline every action. Any action without a responsible party is not yet operational.
- **Evidence test:** Underline every causal verb, such as "improves," "leads to," or "enables." Each must point to an evidence grade.
- **Budget test:** Underline every promised output. Each must have a cost or an explicit zero-cost explanation.
- **Durability test:** End the grant on paper. Identify which activities, jobs, maintenance, and participant benefits survive.
- **Proportionality test:** Reduce the request by half. State exactly which outputs disappear and why the original request is consequently justified.
- **Adversarial test:** A reviewer challenges the weakest assumption. The draft should acknowledge and test it before the reviewer discovers it.

## 8. Build order for the grant packet

participant pathway → platform boundary → claim ledger (15-25 claims) → first-year operating plan → unit-cost model → narrative LAST. The narrative is drafted only after the other artifacts exist and agree (the Reference export's immediate production sequence).

## 9. Version labels & change classes

### 9.1 Version label scheme

| Scope | Scheme | Current | Example |
|---|---|---|---|
| Grant packet | S0 → D1 → D2 → … (letter = stage, number = iteration) | S0 (incomplete source packet) | D1 = first draftable packet |
| Plan files | `NNN-<slug>.md`, monotonic 001, 002, … | - | `001-repo-scaffold.md` |
| Commits | `docs(grant): <change>` - one commit per version | - | `docs(grant): scaffold repo with plan and log structure` |

Commit discipline: the executor never commits; the orchestrator makes exactly one commit per executed version, message `docs(grant): <change>`.

### 9.2 Change-class model

| Class | Meaning | Typical trigger | Example |
|---|---|---|---|
| Editorial | Wording, formatting, style only; no fact, number, or decision changes | Typo, tone, table layout | Reflow a table |
| Clarifying | Adds missing information, resolves an unknown, records a decision or evidence grade | `[INFORMATION NEEDED]` resolved; evidence upgraded | New decision-register entry |
| Operational | Changes plans, delivery, budget, or unit-cost numbers | New cost figure, revised schedule | First-year budget update |
| Foundational | Changes scope, beneficiary, charitable frame, eligibility posture, or core claims | Scope-lock decision (DR-01/06/07) | Beneficiary redefined |

Every executed task appends one row to `Documentation/Logs/changes.md` with its class.

## 10. File map

| Directory | Contents |
|---|---|
| `Documentation/Reference/` | Methodology export (the source of this spec) |
| `Documentation/Research/` | Verified facts, sources, conflicts |
| `Documentation/Prospectus/` | The packet itself (00-05; 06+ planned) |
| `Documentation/Refinement/` | Alignment matrix, gap report, editing checklist |
| `Documentation/Plan/` | Plan files (this repo's change designs) |
| `Documentation/Logs/` | Instructions, research log, changes |
| Documentation/Reviews/ | Threefold review artifacts: comprehension.md, rubric.md, evidence.md per section; run + master indexes (§11) |

## 11. Review model - threefold review of every section

### 11.1 Granularity - sections are the unit of work
- Split every document into review sections: each existing ## heading is one
  section; where a page budget applies, each budgeted page starts a new section.
- Review every paragraph inside a section individually, in reading order; never
  skip, sample, or merge paragraphs.
- A section is reviewed, revised, and re-reviewed on its own; never batch two
  sections into one review.
- Slugify every section heading (lowercase, hyphens) for artifact naming (§11.3).

### 11.2 The three reviewer roles
- One section's review consists of THREE separate review agents, run
  independently: comprehension, rubric, evidence.
- Comprehension reviewer: an unfamiliar reader restates the section without
  looking back and answers the six questions:
  1. Who in San Francisco benefits?
  2. What problem does the project address?
  3. What does the team actually deliver?
  4. Why should that produce the claimed outcomes?
  5. Why is the requested amount justified?
  6. What remains after funding ends?
- Rubric reviewer: scores the section 1-5 on the four rubric criteria
  (transformative ambition, viability, evidence of results, durability),
  justifies each score, and names the strongest claim, the most important
  unsupported assumption, the main execution risk, and what would raise each
  score.
- Evidence reviewer: checks every factual, partnership, budget, legal, and
  outcome claim against the source case; verifies evidence grades (§5), figures
  against the data dictionary, no silent inference, no prohibited words (§6),
  and the editing tests (§7).
- Each reviewer runs the named steps of its facet in order and writes one
  artifact per round (§11.3); reviewers never edit the section - findings and
  verdicts only.

### 11.3 Review artifacts
- Every round writes to Documentation/Reviews/<NNN>-<slug>/<section-slug>/:
  comprehension.md, rubric.md, evidence.md - one file per facet per section;
  rounds append, never rewrite.
- Each facet file records: reviewer, date, round, findings table
  (paragraph | finding | rule violated | severity), and verdict PASS or FAIL.
- Each run's index Documentation/Reviews/<NNN>-<slug>/index.md holds one row per
  section: section | comprehension | rubric | evidence | rounds | status |
  pass date.
- The master index Documentation/Reviews/README.md holds one row per review run;
  add the row when the run starts.
- Superseded findings stay in the files (audit trail); delete nothing after a
  round.

### 11.4 Pass rules and iteration
- Comprehension passes when the reviewer answers all six questions without
  looking back and each answer names the beneficiary, action, responsible
  party, evidence basis, and limitation without inference.
- Rubric passes when all four criteria carry a score with justification and
  every named blocker ("what would raise the score") is answered in the section
  or recorded as [INFORMATION NEEDED: <owner>; why; decision blocked].
- Evidence passes when every material claim has an evidence grade and source,
  no E5 claim remains, figures match the data dictionary, and no prohibited
  word (§6) or failed editing test (§7) remains.
- A section passes only when all three facets pass in the SAME round; a single
  FAIL sends the section back to revision.
- Revision runs through the standard cycle (§3): a pre-plan agent designs the
  revision (Editorial-class fixes (§9.2) may use an addendum to the producing plan),
  an execute agent implements it, then all three facets re-review.
- Rounds are capped at three per section per facet; after round three with any
  facet failing, status becomes blocked and the orchestrator chooses: a new
  plan, a section cut (page-budget rule), or a recorded [INFORMATION NEEDED].
- The orchestrator records pass and blocked statuses in the run index; it never
  overrides a reviewer's FAIL without a new round.

### 11.5 Paragraph acceptance - five questions per paragraph
- Review every paragraph with five yes-or-no questions: (1) does the first
  sentence state its claim, (2) can the claim be traced, (3) is its certainty
  correctly labeled, (4) does it add exactly one new idea, (5) would deleting
  it remove useful information rather than tone.
- Retain the paragraph only if all five answers are yes; any no is a finding
  naming the failed question.

### 11.6 Run trigger - when a review starts
- A review run starts for every change that modifies a document, before the
  version is committed: at each task's verification per plan 001 T01-T12 and
  at every later plan's execution (binding per plan 002 §2.1; the follow-on
  packet sweep runs per plan 002 §2.2).
- The orchestrator starts the run - assigns the three reviewers (§11.2) and
  adds the run's row to the master index (§11.3) - and the change's changes.md
  row is appended only after all three facets pass or a blocked status is
  recorded (§11.4).