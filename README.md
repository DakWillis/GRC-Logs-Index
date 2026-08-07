# GRC Lab Logs — Index

**A control-mapped, searchable index of the DakaraiDoesGRC daily GRC Lab Log archive, Days 1–150.**

Every entry is a real control scenario documented in a fixed structure: what the environment looked like, what the risk actually was, what control addresses it, how that control fails in practice, what evidence proves it operated, and how it maps across ISO/IEC 27001:2022, SOC 2, NIST CSF 2.0, and CIS Controls v8.1.

**→ [Open the master index](INDEX.md)**
**→ [Browse by control domain](domains/)**
**→ [Look up a framework control](frameworks/CROSSWALK.md)**
**→ [Where to start](START-HERE.md)**

---

## Why this exists

Someone asked where the archive lived. There wasn't one — 150 individual posts with no index is a discoverability failure, and a governance program that cannot produce its own record on request has a problem it would flag in anyone else.

So this repository is the record. It is also, deliberately, governed the way the controls inside it are governed: every entry carries a verification status, coverage is stated as a number rather than implied, and nothing is asserted as complete when it is not.

## What this is not

This is not a framework summary, a certification cram sheet, or a list of control text you can read in the standard itself. The value is in the **failure mode** field — the specific way each control breaks in a real environment after it has been implemented, documented, and signed off. That is the part standards do not tell you and the part audits find.

## How to use it

**If you are studying for a certification** — go to [`frameworks/CROSSWALK.md`](frameworks/CROSSWALK.md), find the control you are working on, and read the scenarios mapped to it. Framework text tells you what a control requires. These entries show you what it looks like when the requirement is met on paper and missed in practice.

**If you are building a program** — go to [`domains/`](domains/) and take a domain end to end. The entries within a domain are sequenced so the failure modes compound, which is how they compound in a real environment.

**If you are hiring or evaluating** — [`METHODOLOGY.md`](METHODOLOGY.md) is the fastest read. It sets out the control loop every entry follows and the reasoning behind the field structure.

## Entry structure

Each log follows the same fields, in this order:

| Field | What it captures |
|---|---|
| Focus | The control area under examination |
| Environment | The specific organizational condition — not a generic scenario |
| Risk | What is actually exposed, stated as consequence rather than category |
| Control | The control that addresses it, stated as an operating activity |
| Failure Mode | How the control breaks after implementation |
| Evidence | The artifacts that prove the control operated, not that it exists |
| Risk Score | Likelihood / Impact → Residual |
| Mapping | ISO 27001 · SOC 2 · NIST CSF 2.0 · CIS Controls |

## Companion repositories

| Repository | Domain |
|---|---|
| `IT-Inventory-Audit-Template` | Asset management — audit SOP, discrepancy workflow, evidence naming |
| `grc-vendor-risk-intake-mini-pack` | Third-party risk — intake, tiering, scorecard, decision log |
| `Hands-On-GRC-Starter-Checklist` | Methodology and onboarding for new practitioners |
| `grc-daily-logs-evidence-pack` | Closed-loop case files from live execution |

## Coverage and honesty

This index is published at partial coverage on purpose. See [`docs/PROVENANCE.md`](docs/PROVENANCE.md) for exactly what is verified, what is pending, what source each entry came from, and the two numbering conflicts found in the source calendars during compilation.

An index that claims 150 complete entries while inferring most of them would be a fabricated evidence set. That is the precise failure mode this archive spends 150 days warning about, so it is not one worth committing here.

---

## License

MIT — see [`LICENSE`](LICENSE). Attribution appreciated.

## Disclaimer

All scenarios are sanitized and generalized. No real organization names, staff names, system identifiers, network details, or vendor contracts appear anywhere in this repository. See [`DISCLAIMER.md`](DISCLAIMER.md) and [`SECURITY.md`](SECURITY.md).
