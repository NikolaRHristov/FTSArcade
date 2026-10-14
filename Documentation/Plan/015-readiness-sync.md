# 015 - Readiness Status-Field Sync: Framework-Complete S0 Recorded, D1 Relabel Deferred (plan 001 T12)

> **For Hermes:** Execute this plan with subagent-driven-development (one execute agent for the whole change). The orchestrator reviews and commits once. This change updates status fields and indices only; it does NOT change any packet content file and does NOT relabel the packet.

**Goal:** Execute plan 001 T12 (VERIFY bucket) honestly: keep the packet's version label **S0** and readiness **Not ready** everywhere, update the status fields to record that the framework build is complete (all 12 plan-001 tasks executed), list the blocked tests with their unblocking decisions, and explicitly defer the D1 relabel as a named future change - then sync all indices (root README, Prospectus/README, plan index) and append the changes.md row.

**Scope - in:** exactly 5 files - `README.md` (root), `Documentation/Prospectus/README.md`, `Documentation/Prospectus/00-prospectus.md`, `Documentation/Plan/000-index.md`, `Documentation/Logs/changes.md` - plus this plan file (015), all committed by the orchestrator in one commit.

**Scope - out:** any packet content file (`Prospectus/00-10`, `Refinement/`, `Research/`, `Reference/`, `Logs/instructions.md`, `Logs/research-log.md`); the D1 relabel itself (deferred, never executed by this change); git commits (orchestrator-only, rule R2); email or promotional drafting (prohibited by R1).

**Why not relabel:** Relabeling to D1 would be FALSE. The editing-test verification pass (change 014, plan 001 T11) recorded **14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL** across 29 rows (`Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)). 7 rows are BLOCKED across **4 distinct tests - deletion, substitution, proportionality, sign-off** - and those block Draftable status. The eligibility/registration gate (DR-11) is **Blocked** (registration status unknown as of 2026-10-14). D1 ("first draftable packet", scheme: plan 001 §0.1) is therefore NOT reached; this change records the true state (framework-complete S0, not Draftable) and defers the relabel.

---

## 1. Status-field design (the values this change writes)

Canonical values - used verbatim (or truncated to fit a table cell) in every file below:

| Field | Canonical value | Where written |
|---|---|---|
| Version label | **S0** (incomplete source packet) - unchanged; not relabeled | root README Packet Status; Prospectus/README header + §2; 00-prospectus header |
| Readiness | **Not ready** (content) - framework-complete S0 | root README Packet Status; Prospectus/README header; 00-prospectus header |
| Eligibility/registration gate | **Blocked** (DR-11 - registration status unknown as of 2026-10-14) | root README Packet Status + banner (banner text unchanged); Prospectus/README §3 (unchanged); 00-prospectus §1 Eligibility (unchanged) |
| Framework-complete note | all 12 plan-001 tasks executed (T01-T11 = plans 004-014, committed; T12 = this change); Draftable NOT reached - 7 of 29 verdict rows BLOCKED across 4 distinct tests (deletion, substitution, proportionality, sign-off; 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL - `Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)) + eligibility gate Blocked | the Readiness rows of the three status files |
| Blocked tests + unblocking decisions | deletion → DR-01/DR-06/DR-07 scope lock → narrative prose (T10 successor) re-runs it; substitution → DR-01 (SF problem analysis) + DR-06 (site plan) → T05/T06 successors fill IN-07/BU-04; proportionality → DR-04 (funding scenario + request amount + loss list; 09 §6 gate (1)) → T09 successor; sign-off → DR-02/DR-03/DR-11 (registration + entity), DR-09 (rights schedule), DR-04, DR-10, scope lock + named signatory (05 §5 step 8) | root README "D1 relabel" row; Prospectus/README readiness; 00-prospectus status block; changes.md Decision |
| D1 relabel (deferred) | Named future change, verbatim: **"Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)."** | root README "D1 relabel" row; Prospectus/README readiness; 00-prospectus status block; changes.md Decision; 000-index row 015 |

Rules: every value cell STARTS with the mandated short value (S0 / Not ready / Blocked) so the label reads first and greps verify by prefix; the framework note and deferral follow after a dash. No file may assert the packet IS D1 or Draftable. "Framework-complete" describes the BUILD (tasks executed), never the readiness state.

---

## 2. Files to change - exact edits (current rows quoted)

### F1 - `README.md` (root), Packet Status table (currently lines 13-18)

Current:

```
| Item | Value |
|---|---|
| Version label | S0 (incomplete source packet) |
| Readiness | Not ready (content) |
| Eligibility/registration gate | Blocked (DR-11 - unknown as of 2026-10-14) |
| Next milestone | D1 - first draftable packet (roadmap: `Documentation/Plan/000-index.md`) |
```

Replace the whole table with:

```
| Item | Value |
|---|---|
| Version label | S0 (incomplete source packet) |
| Readiness | Not ready (content) - framework-complete S0: all 12 plan-001 tasks executed (T01-T11 = plans 004-014, committed; T12 = this change); Draftable NOT reached - 7 of 29 verdict rows BLOCKED across 4 distinct tests (deletion, substitution, proportionality, sign-off; 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL - `Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)) + eligibility gate Blocked |
| Eligibility/registration gate | Blocked (DR-11 - registration status unknown as of 2026-10-14) |
| D1 relabel | Deferred - named future change: "Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)". Unblocking decisions: DR-01/DR-06/DR-07 scope lock (deletion, substitution) -> narrative prose (T10 successor); DR-04 funding scenario (proportionality) -> request + loss list (T09 successor); DR-02/DR-03/DR-09/DR-11 + named signatory (sign-off) |
| Next milestone | D1 - first draftable packet (roadmap: `Documentation/Plan/000-index.md`) |
```

### F1b - `README.md` (root), Packet Tree: insert the 06-10 rows and update the Refinement row

Current rows (currently lines 33-34):

```
| `Documentation/Prospectus/05-durability-risks-rights.md` | Durability/risks/rights | S0 |
| `Documentation/Refinement/` | Alignment matrix, gap report, 21-test checklist | Current |
```

Replace with:

```
| `Documentation/Prospectus/05-durability-risks-rights.md` | Durability/risks/rights | S0 |
| `Documentation/Prospectus/06-participant-pathway.md` | Participant pathway framework | S0 |
| `Documentation/Prospectus/07-platform-boundary.md` | Platform boundary framework | S0 |
| `Documentation/Prospectus/08-first-year-operating-plan.md` | First-year operating plan framework | S0 |
| `Documentation/Prospectus/09-unit-cost-model.md` | Unit-cost model & funding scenarios | S0 |
| `Documentation/Prospectus/10-narrative.md` | Narrative framework (prose blocked until Draftable) | S0 |
| `Documentation/Refinement/` | Alignment matrix, gap report, 21-test checklist with recorded verdicts (14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL) | Current |
```

(All other Packet Tree rows and the ⚠ Deadline & Gate banner, Next Actions, and For Agents sections stay verbatim.)

### F2 - `Documentation/Prospectus/README.md`, header status fields (currently lines 3-5)

Current:

```
**Date:** 2026-10-14 (Wednesday)
**Version label:** **S0 - Incomplete source packet; gap identification only.** Per the writing methodology (Reference/…/we're looking to prepare a grant application for h.md), S0 means the sources are not yet approved for drafting and this packet exists to surface gaps, not to persuade.
**Readiness state:** **Not ready** - beneficiary, intervention, eligibility, and budget are all absent or unresolved. Per the methodology's final readiness states, the next action is to complete the source packet; drafting a submission narrative is not yet permitted.
```

Replace with:

```
**Date:** 2026-10-15 (Thursday) - status fields updated by change 015 (plan 001 T12); packet content unchanged.
**Version label:** **S0 - Incomplete source packet; gap identification only.** Per the writing methodology (Reference/…/we're looking to prepare a grant application for h.md), S0 means the sources are not yet approved for drafting and this packet exists to surface gaps, not to persuade. **Unchanged: the relabel to D1 is deferred (see Readiness state).**
**Readiness state:** **Not ready** - the framework build is complete (all 12 plan-001 tasks executed; T01-T11 = plans 004-014, committed; T12 = change 015), but the packet is NOT Draftable: the verification pass recorded 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL across 29 rows (`Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)); 4 distinct tests are BLOCKED - deletion, substitution, proportionality, sign-off - and the eligibility gate (DR-11) is Blocked. Unblocking decisions: DR-01/DR-06/DR-07 scope lock (deletion, substitution) -> narrative prose; DR-04 funding scenario (proportionality) -> request + loss list; DR-02/DR-03/DR-09/DR-11 + named signatory (sign-off). D1 relabel = named future change: "Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)". Drafting a submission narrative is not yet permitted.
```

(The `**Packet owner:**` line, §2 label/readiness tables, §3 dates, §4 open items, §5 next actions stay verbatim.)

### F2b - `Documentation/Prospectus/README.md`, packet index table: append rows 8-12 after row 7

Current last row (line 20):

```
| 7 | `05-durability-risks-rights.md` | Post-grant model, risk register with triggers, rights schedule | S0 | Rights + executive owners |
```

Append:

```
| 8 | `06-participant-pathway.md` | Participant pathway framework | S0 | Decision owners (DR-01/DR-06/DR-07 close) |
| 9 | `07-platform-boundary.md` | Platform boundary framework | S0 | Decision owners (DR-01/DR-06/DR-07 close) |
| 10 | `08-first-year-operating-plan.md` | First-year operating plan framework | S0 | Program + budget owners (scope lock; DR-04) |
| 11 | `09-unit-cost-model.md` | Unit-cost model & funding scenarios | S0 | Budget owner (DR-04) |
| 12 | `10-narrative.md` | Narrative framework (prose blocked until Draftable) | S0 | All owners (scope lock; DR-04; DR-10/DR-09; signatory) |
```

### F3 - `Documentation/Prospectus/00-prospectus.md`, status block (currently lines 3-4)

Current:

```
**Version:** S0 (incomplete source packet - gap identification only) · **Date:** 2026-10-14
**Status:** **Not ready.** Every section below either documents what is actually known (product facts, competition rules) or marks what is missing. No section asserts a beneficiary, intervention, partner, cost, or outcome that is not known.
```

Replace with:

```
**Version:** S0 (incomplete source packet - gap identification only) · **Date:** 2026-10-15
**Status:** **Not ready** - framework-complete S0: all 12 plan-001 tasks executed (T01-T11 = plans 004-014, committed; T12 = change 015; framework documents 06-10 in place). Draftable is NOT reached: 3 of the 8 editing tests and 4 of the 21 checklist tests are BLOCKED - 4 distinct tests: deletion, substitution, proportionality, sign-off (14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL - `Documentation/Refinement/02-refinement-checklist.md` §(a)/§(a.1)) - and the eligibility gate (DR-11) is Blocked. Unblocking decisions: DR-01/DR-06/DR-07 scope lock (deletion, substitution) -> narrative prose (T10 successor); DR-04 funding scenario (proportionality) -> request + loss list; DR-02/DR-03/DR-09/DR-11 + named signatory (sign-off). D1 relabel deferred - named future change: "Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)". Every section below either documents what is actually known (product facts, competition rules) or marks what is missing. No section asserts a beneficiary, intervention, partner, cost, or outcome that is not known.
```

(All body sections 1-11 stay verbatim.)

### F4 - `Documentation/Plan/000-index.md`, append row 015 INSIDE the Index table after row 014 (currently line 22)

Current last row:

```
| 014 | `Documentation/Plan/014-verification-pass.md` | Editing-test verification pass: verdicts for the 8 editing tests + 21 checklist tests (plan 001 T11) | committed | Committed in this version's single commit |
```

Append (status `executed` at append time; the orchestrator flips it to `committed` in this version's single commit, per the file's Status Lifecycle):

```
| 015 | `Documentation/Plan/015-readiness-sync.md` | Readiness status-field sync: framework-complete S0 recorded, D1 relabel deferred, indices synced (plan 001 T12) | executed | Flipped to "committed" by the orchestrator in this version's single commit |
```

### F5 - `Documentation/Logs/changes.md`, append row 015 after the last Record row (currently line 22, ending `| 014 |`)

Appended row (class **Clarifying**, plan ref **015**):

```
| 2026-10-15 | Clarifying | Readiness status-field sync (plan 001 T12): status fields updated to record the completed framework build - version label stays S0, readiness stays Not ready, gate stays Blocked; D1 relabel explicitly deferred as a named future change ("Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)"); indices synced - root README Packet Status (Readiness row carries the framework-complete note; new D1-relabel row lists the 4 blocked tests with unblocking decisions) + Packet Tree rows for Prospectus/06-10, Prospectus/README header status fields + packet index rows 8-12, 00-prospectus.md status block, plan index row 015 | plan 001 T12 (VERIFY) requires the readiness relabel + index sync; the packet is framework-complete but NOT Draftable - 7 of 29 verdict rows are BLOCKED across 4 distinct tests (deletion, substitution, proportionality, sign-off; 14 PASS / 8 PARTIAL / 7 BLOCKED / 0 FAIL) and the eligibility gate (DR-11) is Blocked, so relabeling to D1 would be a false claim; the change records the true state and defers the relabel | No new figures; no budget affected; evidence = Refinement/02-refinement-checklist.md §(a)/§(a.1) verdicts (recorded by change 014) + DR-11 gate state (Blocked, 03-registers.md) | Recorded: packet = framework-complete S0; readiness Not ready; gate Blocked; D1 relabel deferred until the 4 blocked tests unblock (unblocking decisions: DR-01/DR-06/DR-07 scope lock -> deletion/substitution; DR-04 -> proportionality; DR-02/DR-03/DR-09/DR-11 + named signatory -> sign-off) | README.md, Prospectus/README.md, Prospectus/00-prospectus.md, Plan/000-index.md, Logs/changes.md | 015 |
```

Ordering note (constitution §11.6): the changes.md row is appended only after the orchestrator's three-reviewer run passes or a blocked status is recorded. Apply F1-F4 first, run §3 verification V1-V6, then append F5 after the review run, then re-run V7-V8.

---

## 3. Verification (run in order; every check must pass before handoff)

| # | Check | Command / method | Pass rule |
|---|---|---|---|
| V1 | No D1 label assigned as current status | `grep -rn 'D1' README.md Documentation/Prospectus/README.md Documentation/Prospectus/00-prospectus.md` (full listing) and `grep -rnE '^\| Version label \| D1|^\*\*Version label:\*\* \*\*D1|^\*\*Version:\*\* D1|^\| Readiness \| Draftable|^\*\*Readiness state:\*\* \*\*Draftable|^\*\*Status:\*\* \*\*Draftable' README.md Documentation/Prospectus/README.md Documentation/Prospectus/00-prospectus.md` | The `D1` listing shows only permitted forms: (a) deferral wording - the verbatim future-change name "Relabel to D1 once the 4 blocked tests unblock (deletion, substitution, proportionality, sign-off)" or any sentence stating the D1 relabel is deferred; (b) root README "Next milestone" row (roadmap reference) and "D1 relabel" row (the deferral record); (c) Prospectus/README §2 methodology table rows (`\| D1 \| First fidelity draft \|`, `\| Reviewable \| D1 traces and exception report complete \|`). The current-state grep returns 0 hits - no file assigns D1 or Draftable to the packet's version label or readiness. |
| V2 | S0 / Not ready / Blocked consistent | `grep -n 'Version label' README.md; grep -n 'Readiness' README.md; grep -n 'gate' README.md; grep -n 'Version label' Documentation/Prospectus/README.md; grep -n 'Readiness state' Documentation/Prospectus/README.md; grep -n 'Version:' Documentation/Prospectus/00-prospectus.md; grep -n 'Status:' Documentation/Prospectus/00-prospectus.md` | The 7 lines start with the mandated values: `\| Version label \| S0`, `\| Readiness \| Not ready (content) - framework-complete S0`, `\| Eligibility/registration gate \| Blocked (DR-11`, `**Version label:** **S0`, `**Readiness state:** **Not ready**`, `**Version:** S0`, `**Status:** **Not ready**`. No file shows a different value; no line asserts Draftable/D1 as current state. |
| V3 | New files listed in the indices | `for f in 06-participant-pathway 07-platform-boundary 08-first-year-operating-plan 09-unit-cost-model 10-narrative; do grep -q "Documentation/Prospectus/$f.md" README.md || echo "MISSING $f"; done; echo "EXIT:$?"` and `grep -cE '^\| (8|9|10|11|12) \|' Documentation/Prospectus/README.md` | No MISSING lines; EXIT:0; the row-ID count is 5 (rows 8-12); `test -f` each of the 5 files passes (they exist). |
| V4 | All relative links resolve | `python3 - <<'EOF'` with the script in §3.1 | Prints `DANGLING: []`; zero unresolved targets. |
| V5 | Tables render | `python3 - <<'EOF'` with the script in §3.2 | Prints `BAD: []`; every table in the 5 changed files has a separator row and equal pipe counts across rows. |
| V6 | No prohibited words | `grep -rniE 'revolutionary|world-class|cutting-edge|empower|unlock|transform|scalable|sustainable|partners include|data shows' README.md Documentation/Prospectus/README.md Documentation/Prospectus/00-prospectus.md Documentation/Plan/000-index.md Documentation/Logs/changes.md` and `grep -rniE '\bunique\b' <same 5 files>` | 0 hits in both greps. |
| V7 | Git status exact file set | `git status --porcelain` | The set of paths is exactly: `README.md`, `Documentation/Prospectus/README.md`, `Documentation/Prospectus/00-prospectus.md`, `Documentation/Plan/000-index.md`, `Documentation/Logs/changes.md` (modified) + `Documentation/Plan/015-readiness-sync.md` (untracked). No deletions, no other modified/added paths. (Compare paths only - strip the two status chars, e.g. `git status --porcelain | awk '{print $2}' | sort`; tolerate `M` or `M ` staging-state differences.) The orchestrator then commits all 6 paths in one commit: `docs(grant): sync readiness status fields and indices (T12)`. |
| V8 | changes.md + index rows present | `grep -E '\| 015 \|$' Documentation/Logs/changes.md`; `grep -c 'Clarifying' <that row>`; `grep -nE '\| 01[45] \|' Documentation/Plan/000-index.md` | Exactly 1 row ending `\| 015 \|` in changes.md, containing `Clarifying` and the verbatim phrase `Relabel to D1 once the 4 blocked tests unblock`; in 000-index.md exactly 2 hits (014 then 015) with consecutive line numbers, row 015 directly after row 014. |

### 3.1 V4 script (run from the repo root)

```python
import pathlib, re
root = pathlib.Path('.')
changed = ['README.md','Documentation/Prospectus/README.md','Documentation/Prospectus/00-prospectus.md','Documentation/Plan/000-index.md','Documentation/Logs/changes.md']
dangling = []
for rel in changed:
    p = root / rel
    text = p.read_text()
    # markdown links ](...) - resolve against the file's dir, fall back to repo root
    for t in re.findall(r'\]\(([^)]+)\)', text):
        t = t.split('#')[0].strip()
        if not t:
            continue
        if not any(c.resolve().exists() for c in (p.parent / t, root / t)):
            dangling.append((rel, 'link', t))
    # backticked root-relative paths (Documentation/..., README.md)
    for t in re.findall(r'`((?:Documentation/|README\.md)[^`]+)`', text):
        if not (root / t).exists():
            dangling.append((rel, 'path', t))
    # backticked local filenames NN-*.md - resolve against the file's own dir,
    # then repo root, then Documentation/Prospectus/ (changes.md rows reference
    # packet files across dirs without a consistent base)
    for t in re.findall(r'`([0-9]{2}-[^`]+\.md)`', text):
        if not any(c.exists() for c in (p.parent / t, root / t, root / 'Documentation/Prospectus' / t)):
            dangling.append((rel, 'local', t))
print('DANGLING:', dangling)
```

### 3.2 V5 script (run from the repo root)

```python
import pathlib, re
files = ['README.md','Documentation/Prospectus/README.md','Documentation/Prospectus/00-prospectus.md','Documentation/Plan/000-index.md','Documentation/Logs/changes.md']
bad = []
for rel in files:
    lines = pathlib.Path(rel).read_text().splitlines()
    i = 0
    while i < len(lines):
        if lines[i].strip().startswith('|'):
            block = []
            while i < len(lines) and lines[i].strip().startswith('|'):
                block.append(lines[i]); i += 1
            # escaped pipes (\|) are content, not column boundaries - exclude them
            if len(block) < 2 or len({l.count('|') - l.count('\\|') for l in block}) != 1:
                bad.append((rel, 'pipe mismatch', block[0] if block else ''))
            if not re.fullmatch(r'\s*\|[\s:|-]+\|', block[1]):
                bad.append((rel, 'no separator row', block[1]))
        else:
            i += 1
print('BAD:', bad)
```

---

## 4. Notes for the executor

1. Read each file fresh at execution time; if a quoted current row differs (line numbers may have shifted), locate by content, never by line number. Change nothing outside the quoted rows.
2. Do NOT touch packet content files (`Prospectus/00-10`, `Refinement/`, `Research/`, `Reference/`), `Logs/instructions.md`, `Logs/research-log.md`.
3. The D1 relabel is DEFERRED, not executed: after this change no file may assert the packet is D1 or Draftable; "framework-complete S0" is the build state, "Not ready" is the readiness.
4. Review run (constitution §11.6): the orchestrator starts the three-reviewer run (comprehension/rubric/evidence) before commit; the changes.md row (F5) is appended only after all three facets pass or a blocked status is recorded - sequence F1-F4 → V1-V6 → review run → F5 → V7-V8 → handoff.
5. The plan index row 015 is written with status `executed`; the orchestrator flips it to `committed` in the single commit (`docs(grant): sync readiness status fields and indices (T12)`).
6. This plan itself (`015-readiness-sync.md`) is part of the version: it was written by the pre-plan agent, is already on disk, and the orchestrator's single commit includes it.