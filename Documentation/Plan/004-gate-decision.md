# 004 - Gate Decision: Record Eligibility/Registration Status (DR-11)

> **For Hermes:** Execute this plan with the delegation model of `Documentation/Logs/instructions.md` §3 (pre-plan → execute → orchestrator review + one commit per version). This change executes plan 001 task T01 (bucket **GATE** - must land before Oct 15 2026, 03:00 EEST). The executor appends the changes.md row only after the threefold review run (§11.6) passes; the orchestrator commits exactly once (`docs(grant): record eligibility/registration gate decision (DR-11)`).

**Goal:** Record the eligibility/registration go/no-go as decision-register entry **DR-11** (decision value: **unknown** - no registration outcome is invented), keep the gate effect **Blocked**, and sync the gate status fields in `00-prospectus.md` and the root `README.md` banner so all files agree.

**Class:** Clarifying (records a decision + evidence grade; resolves the *record* of the go/no-go, not the outcome - §9.2: "New decision-register entry").
**Scope - in:** the 5 files in Section 2 only.
**Scope - out:** `Documentation/Prospectus/README.md` and `Documentation/Logs/research-log.md` (their DR-03 "unknown" wording remains true; not listed in plan 001 T01's output); email or promotional drafting (protocol R1 - the next action *describes* sending an email, it does not draft one); git commits (orchestrator-only, R2).

---

## 1. Design summary - the DR-11 record

| Field | Value | Source / rule |
|---|---|---|
| Ref | **DR-11** (next free number: register currently holds DR-01…DR-10) | `03-registers.md` §1 |
| Decision | Eligibility/registration gate: registration status + entity eligibility + geography | plan 001 T01; alignment matrix Table B rows 1-3 |
| Decided value | **Unknown** - no positive claim that any entity registered or did not register | plan 001 T01 ("never invent the registration status"); facts pack #9/#10 |
| Deciding owner | Authorized officer (role); named person `[INFORMATION NEEDED: …]` | owner test (§7); context spec "owner placeholder as INFORMATION NEEDED" |
| Date | Execution date `<date>` (expected 2026-10-14 or 2026-10-15 EEST); identical in every occurrence | `date` at execution |
| Evidence grade | **E1** for the gate facts (verified live 2026-10-14, facts-pack #9, #10, #25); the status itself is **ungraded** because it is unknown - no positive claim (evidence-register convention: documented absence = E1, positive claim = E5) | instructions.md §5; `03-registers.md` §3 C07/C08 row |
| Gate effect | **Blocked** (unchanged value; submission impossible without confirmed registration) | facts pack #9: "Only registrants can submit an application" |
| Next action (named) | Authorized officer: **one email to boundless-sf@submittable.com** covering (1) whether any registration exception is possible after Sep 11, (2) which rules §1 category fits a Bulgarian (non-U.S.) entity and how equivalency is evidenced (categories 7/9; conflict C2), (3) written confirmation of the geographic-rule application; record the written answer as a new DR entry or DR-11 addendum | alignment matrix Table B "Action" cells; facts pack #25 |

Uncertainty language (verbatim phrase, required where the status is unknown): **"As of [date], [source] shows…"** (instructions.md §5).

**Explicitly not done:** no email draft anywhere in the change (grep `dear|subject:|sincerely` → 0 hits, V6); no registration outcome invented (the entry records *unknown* and says so).

---

## 2. Files to change

**Executor preamble:** re-read each quoted row below before editing; if any quoted text no longer matches the file at execution time, STOP and report - do not adapt silently.

### 2.1 F1 - `Documentation/Prospectus/03-registers.md` (append DR-11)

Insert a new subsection between the decision-register table (last row DR-10) and the `---` separator that precedes `## 2. Data dictionary`.

Replace:

```
---

## 2. Data dictionary
```

with:

```
### 1.1 Recorded decisions

Entries are appended as decisions are made. An entry records the decided value, the deciding owner, the date, the evidence grade, the gate effect, and the named next action. Open rows (DR-01…DR-10) remain the live register; recorded entries are the audit trail.

| Ref | Decision | Decided value | Deciding owner | Date | Evidence grade | Gate effect | Next action |
|---|---|---|---|---|---|---|---|
| DR-11 | Eligibility/registration gate (registration status + entity eligibility + geography) | **Unknown as of <date>** - as of <date>, the facts pack (`Documentation/Research/facts-pack.md`, facts #9, #10, #25) shows registration closed Sep 11 2026, 5:00 p.m. PT and that only registrants may submit; no registration confirmation, invitation, or Submittable account for any team entity is located. No positive claim is made about registration; the status is recorded as unknown. | Authorized officer `[INFORMATION NEEDED: named person; required to confirm or deny registration and to own the follow-up email; blocks the gate - DR-03]` | <date> | E1 (gate facts, verified live 2026-10-14; documented absence of any registration confirmation; the status itself is ungraded - unknown, no positive claim) | **Blocked** | Authorized officer: send one email to boundless-sf@submittable.com covering (1) whether any registration exception is possible after Sep 11, (2) which rules §1 category fits a Bulgarian (non-U.S.) entity and how equivalency is evidenced (categories 7/9; conflict C2), (3) written confirmation of the geographic-rule application; record the written answer as a new DR entry or a DR-11 addendum. |

---

## 2. Data dictionary
```

**Rules for the inserted text:** `<date>` = the execution date, identical in the three occurrences (Decided value, Date column); the `Decided value` cell contains the verbatim uncertainty phrase "as of <date>, the facts pack … shows"; the entry must contain no salutation, subject line, or sign-off (no email draft).

### 2.2 F2 - `Documentation/Prospectus/00-prospectus.md` (gate status fields)

**(a)** Replace line 30 (Eligibility paragraph in Section 1):

```
**Eligibility:** Unresolved. Registration deadline (Sept 11, 2026, 5:00 p.m. PT) has passed; team registration status unknown. Legal entity, jurisdiction, and tax status unknown. Foreign (e.g., Bulgarian) entity eligibility requires written confirmation. `[INFORMATION NEEDED: authorized officer; required to establish a valid route to submit; blocks the application itself - DR-02/DR-03]`
```

with:

```
**Eligibility:** Recorded in DR-11 (<date>): registration status **unknown** - as of <date>, the facts pack shows registration closed Sep 11, 2026, 5:00 p.m. PT and that only registrants may submit; no registration confirmation is located. Gate effect: **Blocked**. Legal entity, jurisdiction, and tax status remain unknown (DR-02). Foreign (e.g., Bulgarian) entity eligibility requires written confirmation (rules §1 categories 7/9; conflict C2). Next action: one email to boundless-sf@submittable.com covering registration exception, entity eligibility, and geography (DR-11). `[INFORMATION NEEDED: authorized officer (named person); required to confirm or deny registration and to send the follow-up email; blocks the application itself - DR-02/DR-03/DR-11]`
```

**(b)** Replace line 32 (Bottom line):

```
**Bottom line:** As of 2026-10-14 this project is **Not ready** to draft a submission. One day remains to the Oct 15 deadline. The immediate action is the registration/eligibility go/no-go, not narrative writing.
```

with:

```
**Bottom line:** As of <date> this project is **Not ready** to draft a submission. The registration/eligibility go/no-go is recorded in DR-11: status unknown, gate **Blocked**; the immediate action is the confirmation email to boundless-sf@submittable.com, not narrative writing.
```

**(c)** Replace Section 11 table row 1 (Blocking unknowns):

```
| 1 | Registration status | Submission itself | Authorized officer | DR-03 |
```

with:

```
| 1 | Registration status | Submission itself | Authorized officer | DR-03, DR-11 (recorded unknown as of <date>) |
```

### 2.3 F3 - `README.md` (repo root, gate banner + status fields)

**(a)** Replace the banner's gate-status line (line 9):

```
> Current gate status: **Blocked** - see `Documentation/Prospectus/03-registers.md`.
```

with:

```
> Current gate status: **Blocked** (DR-11: registration status unknown as of <date>) - see `Documentation/Prospectus/03-registers.md`.
```

**(b)** Replace the Packet Status row (line 17):

```
| Eligibility/registration gate | Blocked |
```

with:

```
| Eligibility/registration gate | Blocked (DR-11 - unknown as of <date>) |
```

**(c)** Replace Next Actions item 1 (line 42):

```
1. Resolve the eligibility/registration gate (plan task T01, Section 2 of `Documentation/Plan/001-repo-scaffold.md`).
```

with:

```
1. Send the registration/eligibility/geography email to boundless-sf@submittable.com (recorded decision DR-11; gate remains **Blocked** until the written answer).
```

### 2.4 F4 - `Documentation/Logs/changes.md` (append row)

Append after the last row (the 003 row). Anchor to replace:

```
| 2026-10-14 | Clarifying | Constitution §11: §11.2 comprehension questions copied verbatim from the Reference export; new §11.6 run-trigger rule; §11.4 cites §9.2 | fix review 002's FAIL (evidence check 1a) and the rubric's trigger/citation follow-ups: the constitution must quote the export's comprehension questions verbatim and state when review runs start | - | Adopt the corrected §11 (verbatim questions; run trigger; §9.2 citation) | Logs/instructions.md (§11.2 block, new §11.6, §11.4 citation), Plan/000-index.md | 003 |
```

with the same row plus one new row:

```
| 2026-10-14 | Clarifying | Constitution §11: §11.2 comprehension questions copied verbatim from the Reference export; new §11.6 run-trigger rule; §11.4 cites §9.2 | fix review 002's FAIL (evidence check 1a) and the rubric's trigger/citation follow-ups: the constitution must quote the export's comprehension questions verbatim and state when review runs start | - | Adopt the corrected §11 (verbatim questions; run trigger; §9.2 citation) | Logs/instructions.md (§11.2 block, new §11.6, §11.4 citation), Plan/000-index.md | 003 |
| <date> | Clarifying | Record eligibility/registration gate decision (DR-11): registration status unknown as of <date>; gate stays Blocked; next action = one email to boundless-sf@submittable.com (registration exception + entity eligibility + geography) | plan 001 T01 requires the go/no-go recorded; no registration confirmation is located, so the record states the unknown state - no outcome invented | E1 gate facts (facts-pack #9/#10/#25); status itself ungraded (unknown); no budget affected | Recorded: status unknown; deciding owner = authorized officer (named person INFORMATION NEEDED); gate effect Blocked | Prospectus/03-registers.md, Prospectus/00-prospectus.md, README.md | 004 |
```

### 2.5 F5 - `Documentation/Plan/000-index.md` (append row)

Append after the 003 row. Anchor to replace:

```
| 003 | `Documentation/Plan/003-review-revision.md` | Review revision: verbatim comprehension questions, run-trigger rule, §9.2 citation (constitution §11) | committed | Committed in this version's single commit |
```

with the same row plus one new row:

```
| 003 | `Documentation/Plan/003-review-revision.md` | Review revision: verbatim comprehension questions, run-trigger rule, §9.2 citation (constitution §11) | committed | Committed in this version's single commit |
| 004 | `Documentation/Plan/004-gate-decision.md` | Gate decision: record eligibility/registration status (DR-11) | executed | Executed by the execute agent; orchestrator flips to "committed" in this version's single commit |
```

---

## 3. Verification (run in order; every check must pass before the executor handoff)

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | DR-11 entry present | `grep -n 'DR-11' Documentation/Prospectus/03-registers.md` | Exactly one DR-11 row in the new §1.1 table; all 8 columns populated; `<date>` replaced identically in all occurrences (grep the entry, count `<date>` = 0) |
| V2 | No invented outcome | Inspect the DR-11 `Decided value` cell | Contains "unknown"; asserts neither "registered" nor "not registered"; no registration confirmation/invitation named as existing |
| V3 | Uncertainty language | `grep -n 'as of ' Documentation/Prospectus/03-registers.md` (DR-11 row) and `Documentation/Prospectus/00-prospectus.md` (Eligibility line) | The verbatim phrase "as of <date>, … shows" present in the DR-11 Decided value and echoed in the 00-prospectus Eligibility line |
| V4 | Owner test (§7) | Underline every action verb in the DR-11 entry and the two edited 00-prospectus paragraphs | Every action ("send", "record", "confirm", "deny", "decide") names the authorized officer or carries the `[INFORMATION NEEDED: authorized officer …]` placeholder |
| V5 | Deletion test (§7) | Remove "FTSArcade" from the DR-11 entry (mentally or via scratch copy) | Entry remains fully intelligible: decision, owner, date, grade, gate effect, next action all stand without the project name |
| V6 | No email draft (protocol R1) | `grep -niE 'dear|subject:|sincerely' Documentation/Prospectus/03-registers.md Documentation/Prospectus/00-prospectus.md README.md Documentation/Logs/changes.md Documentation/Plan/000-index.md` | 0 hits |
| V7 | Gate-field consistency | Grep `Blocked` in README.md (banner + Packet Status), 00-prospectus.md (Eligibility + Bottom line) | All gate fields say **Blocked** and carry a DR-11 reference |
| V8 | Evidence grade present | Inspect DR-11 `Evidence grade` cell | "E1" stated for gate facts; no grade asserted on the unknown status; no causal verb ungraded |
| V9 | changes.md row | `grep -n '004' Documentation/Logs/changes.md` | One new row with class "Clarifying" and Plan ref 004; appended AFTER the threefold review run passes (§11.6) |
| V10 | Index row | `grep -n '| 004 |' Documentation/Plan/000-index.md` | Row 004 present, status `executed` |
| V11 | Tables render | Pipe-count check on the new/changed tables (DR-11 row, changes.md row, index row) | Header, separator, and body rows have equal pipe counts |
| V12 | No collateral edits | `git status --porcelain` before and after | Exactly the 5 files above modified; no other file touched; no deletions |

**Review run (instructions.md §11.6):** after V1-V12 pass, the orchestrator starts the threefold review (comprehension / rubric / evidence) of the changed documents; the changes.md row (F4) is appended only after all three facets pass or a blocked status is recorded. The orchestrator then commits exactly once: `docs(grant): record eligibility/registration gate decision (DR-11)`.

---

## 4. Executor inputs (read from the repo at execution; never invent)

| Item | Where to read it | Why |
|---|---|---|
| Next free DR number | `Documentation/Prospectus/03-registers.md` §1 table | Must still be DR-11 (DR-01…DR-10 occupied); if the register changed, stop and report |
| Execution date `<date>` | `date` at execution (EEST); expected 2026-10-14 or 2026-10-15 | Every `<date>` occurrence in this plan resolves to this one value |
| Current-row verification | Re-read each quoted row in Section 2 before editing | Any mismatch = stop and report; never adapt silently |
| Uncertainty phrase | instructions.md §5 verbatim list | "As of [date], [source] shows…" only |
| Evidence-grade definitions | instructions.md §5 (E1-E5 table) | E1 for verified gate facts; no positive claim → no grade on the status |
| facts-pack references | `Documentation/Research/facts-pack.md` #9 (registration closed), #10 (deadline), #25 (contact), C2 (foreign-entity conflict) | The DR-11 entry cites these; do not re-derive |