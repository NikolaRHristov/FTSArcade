# Comprehension Review - 016-review-sweep, unit 03-registers-2-data-dictionary

**Reviewer role:** Comprehension · **Target:** `Documentation/Prospectus/03-registers.md` §2 "Data dictionary" (intro rule paragraph + F-01…F-11 table rows) · **Round:** 1 · **Date:** 2026-10-15
**Method:** section read once, restated and answered from memory without re-reading · **Verdict: PASS**

## Restatement

Section 2 is the packet's data dictionary: one table of eleven figures (F-01 Reach … F-11 Reachable population), each row carrying figure, definition, population, period, source, calculation, and limitation, governed by the rule that every figure has exactly one definition and that "users," "participants," "young people," and "beneficiaries" may not be used interchangeably unless the dictionary declares them identical. Status is S0: most entries are templates pending program decisions, with `[INFORMATION NEEDED]` markers on F-02 (technical owner; analytics or omit), F-09 (budget owner; cost source), and F-11 (program lead; source required), and F-01's population TBD by DR-01. Several rows encode hard measurement rules: F-01 reach is never website use, F-05 outcomes must be pre-registered and immutable after results, F-07 indirect costs are up to 29% of direct costs within the $50M award (not 29% of the total award), F-08 geographic compliance must stay ≤25% outside SF, and only F-06/F-07/F-10 carry E1-grade observed facts (cabinet counts, rules §7, FAQ - retrieved 2026-10-14).

## Answers to the adapted six questions

| # | Question (§11.2, adapted to a reference table) | Answer |
|---|---|---|
| 1 | Who in San Francisco benefits? | The dictionary defines the figures that will measure SF beneficiaries once DR-01 chooses the population: F-01 (people completing enrollment, eligible San Francisco residents, population TBD - DR-01) and F-11 (estimated eligible population, SF residents in the beneficiary definition, program years 1-5). Responsible party: program lead (F-11 source). Evidence basis: recruitment records (F-01); TBD local source (F-11). Limitation: no reachable-population estimate exists yet, and the beneficiary population is undefined until DR-01 closes. |
| 2 | What problem does the project address? | As a dictionary, it addresses unverifiable and conflated measurement: without one definition per figure, claims could silently swap "users" for "participants" or "reach" and figures could not be traced. It fixes per figure a definition, population, period, source, calculation, and limitation, and forbids interchangeable terms unless declared identical. Responsible party: packet authors, with named owners via `[INFORMATION NEEDED]` markers (technical owner, budget owner, program lead). Evidence basis: the dictionary's own columns. Limitation: S0 - most entries are templates pending program decisions, so the dictionary currently defines structure, not settled values. |
| 3 | What does the team actually deliver? | A data dictionary of 11 figures (F-01 Reach, F-02 Website use, F-03 Completion, F-04 Unit cost, F-05 Outcome, F-06 Cabinet count, F-07 Indirect-cost rate, F-08 Geographic compliance, F-09 Award request, F-10 Peer-review load, F-11 Reachable population). Only three rows carry observed facts: F-06 (24 cabinets listed, 15 live, 8 WIP, observed 2026-10-14), F-07 (up to 29% indirect cap per rules §7, retrieved 2026-10-14), F-10 (4 peer reviews, up to 6, ~2.5 h, per FAQ retrieved 2026-10-14). Responsible party: technical owner (F-02 analytics or omit), budget owner (F-09), program lead (F-11). Limitation: the rest are templates with no positive values yet. |
| 4 | Why should that produce the claimed outcomes? | The dictionary produces no outcomes itself; it makes outcome claims honest by construction - F-05 requires a pre-specified result measured by a pre-registered method that may not change after results are seen, and F-01/F-02 exclude website visits and engagement from ever being relabeled as reach or outcomes (consistent with §1 DR-05/DR-07 rules). Responsible party: evidence/measurement owners. Evidence basis: F-01, F-02, F-05 rows. Limitation: no outcome can be measured until DR-01/DR-06/DR-07 are decided (S0), and F-05's follow-up point and population are not yet fixed. |
| 5 | Why is the requested amount justified? | Through the cost figures: F-04 unit cost (eligible costs ÷ completers, excluded overhead stated separately), F-07 indirect-cost rate (up to 29% of direct project/activity costs, within the $50M award limit, explicitly not 29% of the total award), F-09 award request (sum of supported costs across the 4 cost-model layers for the selected scenario, must equal supported costs). Responsible party: budget owner (F-09). Evidence basis: budget model + rules §7 (E1). Limitation: F-09 is ungrounded until `[INFORMATION NEEDED: budget owner; cost source]`; F-04 needs completed participants, which require the program to run. |
| 6 | What remains after funding ends? | The dictionary itself does not define post-grant durability; its only rolling, non-program figure is F-02 (website use, rolling period, anyone with browser access globally, no account required, no program participation implied), which would persist as an artifact but cannot support learning/employment claims. Responsible party: not named in this section. Evidence basis: F-02 row. Limitation: durability as a model is outside this unit's scope; the honest answer is that this section does not address what remains after funding ends. |

## Acceptance check - figure rows (and the governing rule paragraph), §11.5 five questions

Units: the intro rule paragraph plus rows F-01…F-11. Q1 = first sentence/cell states the claim; Q2 = claim traceable; Q3 = certainty correctly labeled; Q4 = exactly one new idea; Q5 = deletion removes useful information, not tone.

| Unit | Q1 claim first | Q2 traceable | Q3 certainty labeled | Q4 one new idea | Q5 deletion info, not tone | Result |
|---|---|---|---|---|---|---|
| Rule paragraph | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-01 Reach | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-02 Website use | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-03 Completion | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-04 Unit cost | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-05 Outcome | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-06 Cabinet count | ✅ | ❌ | ✅ | ✅ | ✅ | Pass (one question) |
| F-07 Indirect-cost rate | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-08 Geographic compliance | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-09 Award request | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-10 Peer-review load | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |
| F-11 Reachable population | ✅ | ✅ | ✅ | ✅ | ✅ | Pass |

## Findings

| Paragraph | Finding | Rule violated | Severity |
|---|---|---|---|
| F-06 Cabinet count | The figure's own components do not reconcile: 24 cabinets listed vs 15 live + 8 WIP = 23. Either a 24th cabinet exists in an unstated third state or a count drifted; the limitation ("site labels change; counts may drift") acknowledges drift generally but does not explain the one-cabinet gap. Q2 (traceable) fails. | §11.5(2) | Minor - non-blocking; the claim's source and date are stated, and the row admits drift; the specific gap is a dictionary-completeness nit for the evidence facet or a revision. |

## Verdict

**PASS.**

- Restatement: faithful - captures the unit's nature (one-definition-per-figure dictionary, term-interchangeability rule, S0 template status, the three `[INFORMATION NEEDED]` markers, the hard exclusions in F-01/F-02/F-05/F-07/F-08, and the three E1 observed-fact rows).
- Six answers: all six present, each naming beneficiary/population, action, responsible party (owner or marker), evidence basis (source/calculation column), and limitation without inference; answer 6 honestly states the unit does not address durability.
- Acceptance check: 12 units checked against the five §11.5 questions; 11 pass all five, F-06 fails exactly one (traceable, one-cabinet arithmetic gap). No unit fails more than one acceptance question, satisfying the pass rule.
- Cross-checks from memory hold: F-07's 29% cap and F-08's ≤25% rule match the §1 decision rules and the evidence register's C06 row; F-10's 4-up-to-6 ~2.5 h load matches DR-08; F-01/F-02 exclusions match DR-07's engagement-not-outcome rule; 24 listed vs 15+8 WIP is the only inconsistency found.