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