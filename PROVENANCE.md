# Provenance and coverage

This document states exactly how complete this index is, where each populated entry came from, and what remains open. It is here because an archive that cannot account for its own completeness has the same problem as a control register that cannot account for its own evidence.

Back to [master index](../INDEX.md).

---

## Current coverage

| Status | Count | Share of 150 |
|---|---|---|
| 🟢 Verified — full field set confirmed | 20 | 13% |
| 🟡 Partial — focus and/or mapping confirmed | 13 | 9% |
| ⚪ Pending — slot reserved, content not yet transcribed | 117 | 78% |
| **Populated total** | **33** | **22%** |

## Verification definitions

**🟢 Verified.** The complete published field set was located in the source content calendars: focus, environment, risk, control, failure mode, evidence list, risk score, and all four framework references. Nothing in a verified row is inferred.

**🟡 Partial.** The focus area and at least one framework reference were located, and the remaining fields are pending transcription. Where a failure mode appears in a partial row, it is either recovered directly or clearly noted as reconstructed. Partial rows should be treated as accurate on what they state and incomplete on what they omit.

**⚪ Pending.** The day number is reserved and, where a weekly theme was confirmed, the theme is recorded. No focus, mapping, or failure mode is claimed.

## Why this published at 22% rather than 100%

The complete day-by-day content exists in the source content calendars — the monthly build files where each day's post was drafted. Those files were not available at compilation time. What was available was the subset quoted, revised, or referenced across project history.

The alternative to partial publication was to generate the missing 117 entries by inference from the confirmed pattern. That was rejected. Generated entries would be indistinguishable from real ones to a reader, and every one would be a fabricated record of a post that was never published — in a repository whose entire premise is that evidence must be defensible. A viewer who cross-checked one invented entry against the actual video would have found a genuine integrity failure, and would have been right to.

Partial coverage published honestly is a defensible artifact. Complete coverage populated by inference is a fabricated evidence set. The archive spends 150 entries making that distinction; it would be a poor place to abandon it.

## Open conflicts found during compilation

Two genuine inconsistencies surfaced in the source material. Both need a decision before this repository is presented as authoritative.

### Conflict 1 — Day numbering scheme changed mid-run

The earlier content calendars assign day numbers to weekend posts. Day 75 is a Sunday Architecture post. Day 68 and Day 80 are Friday Deep Breakdowns.

The July calendar assigns day numbers to weekdays only. Days 126–150 span Monday 29 June through Friday 31 July — twenty-five numbers across five Monday-to-Friday weeks, with no weekend numbers issued.

Consequence: the day number does not map to a consistent calendar offset across the full run, so Day 150 does not sit 150 days after Day 1. This is worth resolving explicitly rather than leaving a reader to discover it.

**Options:** keep the historical numbers as published and document the scheme change at the point it occurred, or renumber to a single scheme and publish a mapping table from old to new. The first option is strongly preferred — the numbers are already public in 150 video titles, and renumbering would break every existing reference. Documenting the change is the honest fix; rewriting history is not.

### Conflict 2 — Two topics assigned to the same day numbers

| Day | Topic A | Topic B |
|---|---|---|
| 63 | MFA Enforcement Validation | Asset inventory drift |
| 65 | Asset Inventory — Software Asset Tracking | Control Testing / Evidence Sampling |

These almost certainly reflect a draft revised after the calendar was rebuilt, with one version published and the other superseded. The published version is the authoritative one. Confirm against the actual posts and correct the index rows.

## Source of populated entries

| Range | Source | Confidence |
|---|---|---|
| 16, 24, 29, 32, 46 | Analytics reach reporting — post titles and hooks | Focus confirmed; framework mapping mostly pending |
| 17, 27 | Format rebuild drafts with complete field sets | High |
| 52–68 | Content calendar excerpts, continuous block | High |
| 72–80 | Content calendar excerpts | High for 75, 76, 79, 80; partial for 72, 74, 78 |
| 120–121 | Content calendar excerpts | High for 121; ISO reference pending for 120 |
| 126–150 | July calendar — weekly themes and date bands confirmed | Themes confirmed; individual days pending |

### July arc — confirmed structure

| Days | Theme | Date band |
|---|---|---|
| 126–130 | Continuous Monitoring Architecture | Mon 29 Jun – Fri 3 Jul |
| 131–135 | Vendor Governance Framework | Mon 6 Jul – Fri 10 Jul |
| 136–140 | Maturity Modeling & Program Measurement | Mon 13 Jul – Fri 17 Jul |
| 141–145 | Access Governance — Advanced Topics | Mon 20 Jul – Fri 24 Jul |
| 146–150 | Incident Response Governance & Phase 3 Bridge | Mon 27 Jul – Fri 31 Jul |

August follows as the mock audit simulation capstone month.

## Editorial note on wording

Failure mode text in this index follows the archive's current convention of using *yet* in place of *but*. Several source posts predate that convention and used *but* in the original caption. The index applies the current convention for internal consistency; if verbatim fidelity to the original captions is preferred, revert those strings in the generator data.

## How to close the gap

The index is generated from a single data structure, so backfilling is a data-entry task rather than a document-editing task.

1. Open `build_index.py`. Every entry is one `d(...)` call in the `DAYS` list.
2. For each day, fill `focus`, `domain`, `iso`, `soc2`, `nist`, `cis`, `failure`, and set `status="verified"` once the full field set is confirmed against the published post.
3. Re-run `python3 build_index.py`. `INDEX.md`, every file in `domains/`, and `frameworks/CROSSWALK.md` regenerate together, and the coverage counts update automatically.
4. Commit. Log the coverage change in [`../CHANGELOG.md`](../CHANGELOG.md).

Suggested pace: one month of the archive per session, roughly twenty to twenty-five entries. Five sessions closes it. Update the coverage number in the changelog each time so the progression is visible in the commit history — which is itself the evidence that the archive is maintained rather than dumped.

Recommended order: complete the ranges already partially populated first (52–80, then 120–121), because context is freshest and the domain files fill out fastest. Then work backward from Day 51 to Day 1, then forward through 81–150.
