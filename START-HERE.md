# Where to start

150 entries is too many to read in order. This page routes you by what you are trying to do.

The sequencing below is not arbitrary. It is ordered by which scenarios actually reached and held the most practitioners across the archive's run, and by the search terms people were using when they found the content in the first place. Reach data is used to order this page; it is not published as a metric, because view counts describe an algorithm's behavior rather than a control's quality.

Back to [master index](INDEX.md).

---

## The five entries that resonated most

If you read nothing else, read these. Each one addresses a control that organizations believe is closed and usually is not.

| Day | Focus | Why it landed |
|---|---|---|
| [29](domains/asset-management.md) | Return of Assets — verification at offboarding | Asset return is assumed from a completed checklist rather than verified against the register. Nearly every offboarding process has this gap. |
| [32](domains/data-protection-classification.md) | Legacy shared folder risk | Dormant repositories keep their sensitive contents and their inherited permissions. Nobody owns a folder nobody talks about. |
| [16](domains/access-governance-identity.md) | Shared account ownership | An account flagged for owner confirmation and left active is an unmanaged identity with a paper trail proving you knew. |
| [24](domains/access-governance-identity.md) | Access accumulation over time | Entitlement drift is not an event. It is the absence of a revocation trigger across many small, individually reasonable approvals. |
| [46](domains/access-governance-identity.md) | Dormant account management | Dormant accounts expand attack surface silently, and disablement is usually deferred pending a confirmation that never arrives. |

Four of those five sit in access governance and asset management. That is not a content preference — it is where the findings are.

---

## Routes by intent

### I am studying for a certification

Start at [`frameworks/CROSSWALK.md`](frameworks/CROSSWALK.md). Find your control, read every scenario mapped to it. The highest-density mappings in the archive are:

- **ISO A.5.9** (inventory of information and associated assets) — asset lifecycle from acquisition through disposition
- **ISO A.5.18 / A.5.15** (access rights, privileged access) — joiner, mover, leaver and privilege review
- **ISO A.8.9** (configuration management) — baselines and drift
- **ISO A.8.15** (logging) — retention and evidence integrity
- **ISO A.5.19–A.5.22** (supplier relationships) — the full third-party lifecycle

### I am building or fixing a program

Take one domain end to end from [`domains/`](domains/). Recommended order, because each domain's failures depend on the previous one being solved:

1. [Asset Management](domains/asset-management.md) — you cannot govern an inventory you do not have
2. [Access Governance & Identity](domains/access-governance-identity.md) — the largest finding source in most programs
3. [Configuration & Hardening](domains/configuration-hardening.md) — baselines, and validating them after deployment
4. [Logging & Monitoring](domains/logging-monitoring.md) — whether your evidence survives to the investigation window
5. [Third-Party & Vendor Risk](domains/third-party-vendor-risk.md) — intake through offboarding
6. [Risk Management & Governance](domains/risk-management-governance.md) — register, acceptance, ownership, maturity
7. [Audit, Evidence & Control Testing](domains/audit-evidence-control-testing.md) — what makes a conclusion defensible

### I found this by searching for something specific

The terms people most often arrived on, and where they lead:

| If you searched | Go to |
|---|---|
| ISO/IEC 27001, ISO 27001 controls | [`frameworks/CROSSWALK.md`](frameworks/CROSSWALK.md) |
| ISO 27001 certification | [Audit, Evidence & Control Testing](domains/audit-evidence-control-testing.md) — what an auditor actually tests |
| GRC, GRC analyst | [`METHODOLOGY.md`](METHODOLOGY.md) — the control loop the whole role runs on |
| Endpoint security | [Configuration & Hardening](domains/configuration-hardening.md) |
| Technical background moving into GRC | [`METHODOLOGY.md`](METHODOLOGY.md), then [Logging & Monitoring](domains/logging-monitoring.md) — the closest bridge from an operations skill set |

### I am new to this entirely

Read [`METHODOLOGY.md`](METHODOLOGY.md) first, then Days 17, 27, and 65 in [Asset Management](domains/asset-management.md). Asset management is the cleanest entry point into GRC because the control is intuitive and the failure modes are still surprising.

---

## The pattern worth noticing

Read enough of these and the same structure appears in every domain. The control is almost never missing. It is defined, documented, approved, and reported as operating. What fails is one of four things:

1. **The control was defined and never validated after deployment.** Baselines, hardening, MFA policy.
2. **The evidence exists yet cannot survive to when it is needed.** Local log storage, retention gaps.
3. **The review cadence is slower than the rate of change.** Annual privilege reviews in an environment that changes weekly.
4. **The exception became the process.** Emergency changes, verbal approvals.

Those four are the whole archive compressed. Everything else is which control domain you are standing in when it happens.
