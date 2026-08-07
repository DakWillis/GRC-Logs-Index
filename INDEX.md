# GRC Lab Logs — Master Index, Days 1–150

Every daily GRC Lab Log from the DakaraiDoesGRC archive, mapped to its control focus, framework references, and failure mode.

This index exists because 150 individual videos are not a body of work. An indexed, control-mapped, searchable archive is. The archive is governed the same way the controls inside it are: every entry has a verification status, and nothing is asserted as complete when it is not.

## Verification status

| | Status | Meaning | Count |
|---|---|---|---|
| 🟢 | `verified` | Full V2 field set published and confirmed — focus, environment, risk, control, failure mode, evidence, risk score, four-framework mapping | 20 |
| 🟡 | `partial` | Focus and at least one framework reference confirmed; remaining fields pending backfill | 13 |
| ⚪ | `pending` | Slot reserved; content not yet transcribed into the index | 117 |

**Coverage: 33 of 150 entries populated (22%).** Backfill method and provenance: [`docs/PROVENANCE.md`](docs/PROVENANCE.md).

A partially populated index published honestly is more defensible than a complete one populated by inference. See [`docs/PROVENANCE.md`](docs/PROVENANCE.md) for why that decision was made and how to close it.

## Navigation

- **By control domain** — [`domains/`](domains/) — the way most people actually search
- **By framework control** — [`frameworks/CROSSWALK.md`](frameworks/CROSSWALK.md) — ISO 27001, SOC 2, NIST CSF 2.0, CIS v8.1 → day numbers
- **Where to start** — [`START-HERE.md`](START-HERE.md) — the entries that reached the most practitioners
- **Methodology** — [`METHODOLOGY.md`](METHODOLOGY.md) — the control loop every log follows

---

## Full index

| | Day | Series | Focus | Framework mapping | Failure mode |
|---|---|---|---|---|---|
| ⚪ | **1** | — | *pending* | — | — |
| ⚪ | **2** | — | *pending* | — | — |
| ⚪ | **3** | — | *pending* | — | — |
| ⚪ | **4** | — | *pending* | — | — |
| ⚪ | **5** | — | *pending* | — | — |
| ⚪ | **6** | — | *pending* | — | — |
| ⚪ | **7** | — | *pending* | — | — |
| ⚪ | **8** | — | *pending* | — | — |
| ⚪ | **9** | — | *pending* | — | — |
| ⚪ | **10** | — | *pending* | — | — |
| ⚪ | **11** | — | *pending* | — | — |
| ⚪ | **12** | — | *pending* | — | — |
| ⚪ | **13** | — | *pending* | — | — |
| ⚪ | **14** | — | *pending* | — | — |
| ⚪ | **15** | — | *pending* | — | — |
| 🟡 | **16** | GRC Log | Shared Account Ownership | NIST PR.AC · CIS 5 | Shared accounts flagged for owner confirmation yet left active without resolution |
| 🟢 | **17** | GRC Log | Asset Inventory — Inactive Equipment Disposition | ISO A.5.9 · SOC 2 CC6.1 · NIST ID.AM · CIS 1 | Review occurs ad hoc — no scheduled cadence, no evidence standard, no ownership assignment |
| ⚪ | **18** | — | *pending* | — | — |
| ⚪ | **19** | — | *pending* | — | — |
| ⚪ | **20** | — | *pending* | — | — |
| ⚪ | **21** | — | *pending* | — | — |
| ⚪ | **22** | — | *pending* | — | — |
| ⚪ | **23** | — | *pending* | — | — |
| 🟡 | **24** | GRC Log | Access Accumulation Over Time | — | Access accrues through role changes without a revocation trigger |
| ⚪ | **25** | — | *pending* | — | — |
| ⚪ | **26** | — | *pending* | — | — |
| 🟢 | **27** | GRC Log | Asset Inventory — Unused Peripheral Disposition | ISO A.5.9 · SOC 2 CC6.1 · NIST ID.AM · CIS 1 | Disposition status recorded generically without specifying whether the asset was reassigned, stored, or destroyed |
| ⚪ | **28** | — | *pending* | — | — |
| 🟡 | **29** | GRC Log | Return of Assets — Verification at Offboarding | ISO A.5.11 | Asset return assumed from the offboarding checklist rather than verified against the register |
| ⚪ | **30** | — | *pending* | — | — |
| ⚪ | **31** | — | *pending* | — | — |
| 🟡 | **32** | GRC Log | Legacy Shared Folder Risk | — | Dormant repositories retain sensitive content and inherited permissions with no review owner |
| ⚪ | **33** | — | *pending* | — | — |
| ⚪ | **34** | — | *pending* | — | — |
| ⚪ | **35** | — | *pending* | — | — |
| ⚪ | **36** | — | *pending* | — | — |
| ⚪ | **37** | — | *pending* | — | — |
| ⚪ | **38** | — | *pending* | — | — |
| ⚪ | **39** | — | *pending* | — | — |
| ⚪ | **40** | — | *pending* | — | — |
| ⚪ | **41** | — | *pending* | — | — |
| ⚪ | **42** | — | *pending* | — | — |
| ⚪ | **43** | — | *pending* | — | — |
| ⚪ | **44** | — | *pending* | — | — |
| ⚪ | **45** | — | *pending* | — | — |
| 🟡 | **46** | GRC Log | Dormant Account Management | — | Dormant accounts identified yet disablement deferred pending manager confirmation that never arrives |
| ⚪ | **47** | — | *pending* | — | — |
| ⚪ | **48** | — | *pending* | — | — |
| ⚪ | **49** | — | *pending* | — | — |
| ⚪ | **50** | — | *pending* | — | — |
| ⚪ | **51** | — | *pending* | — | — |
| 🟢 | **52** | GRC Log | Configuration Management | ISO A.8.9 · SOC 2 CC7.1 · NIST PR.IP · CIS 4 | Baseline defined yet never validated post-deployment — drift accumulates silently |
| 🟢 | **53** | GRC Log | Data Classification | ISO A.5.12 · SOC 2 CC3.2 · NIST PR.DS · CIS 3 | Policy exists yet staff apply labels inconsistently because training never followed the rollout |
| 🟢 | **54** | GRC Log | Network Segmentation | ISO A.8.20 · SOC 2 CC6.6 · NIST PR.AC · CIS 12 | Segmentation implemented at the perimeter yet internal east-west traffic remains unrestricted |
| 🟢 | **55** | GRC Log | Security Awareness Training | ISO A.6.3 · SOC 2 CC2.2 · NIST PR.AT · CIS 14 | Training is completed yet click rates on simulated phishing remain unchanged because content is not targeted |
| 🟢 | **56** | GRC Log | Change Management | ISO A.8.32 · SOC 2 CC8.1 · NIST PR.IP · CIS 4 | Process exists yet emergency changes bypass it routinely, which gradually normalizes the exception |
| 🟢 | **57** | GRC Log | Encryption in Transit | ISO A.8.24 · SOC 2 CC6.7 · NIST PR.DS · CIS 3 | External traffic encrypted yet internal service-to-service communication left unprotected because it feels low risk |
| 🟢 | **58** | GRC Log | Vulnerability Management | ISO A.8.8 · SOC 2 CC7.1 · NIST DE.CM · CIS 7 | Scans run on schedule yet remediation is driven by availability rather than risk, leaving critical findings open |
| 🟢 | **59** | GRC Log | Privileged Access Management | ISO A.5.15 · SOC 2 CC6.2 · NIST PR.AC · CIS 6 | Privileged accounts inventoried yet review cycle is annual, allowing excessive access to persist for most of the year |
| 🟢 | **60** | GRC Log | System Hardening | ISO A.8.9 · SOC 2 CC7.1 · NIST PR.IP · CIS 4 | Hardening applied manually with no post-deployment scan — drift goes undetected after first use |
| 🟢 | **61** | GRC Log | Audit Log Retention & Integrity | ISO A.8.15 · SOC 2 CC7.2 · NIST DE.CM · CIS 8 | Logs collected yet stored locally on endpoints, making them tamper-susceptible and inaccessible post-compromise |
| 🟡 | **62** | GRC Log | Risk Register Management | — | — |
| 🟡 | **63** | GRC Log | MFA Enforcement Validation | — | MFA policy enabled tenant-wide yet enforcement never validated against the actual sign-in log |
| 🟡 | **64** | GRC Log | Access Review — Risk-Based Sampling | — | Review samples selected by convenience rather than risk tier, so the highest-privilege accounts go untested |
| 🟢 | **65** | GRC Log | Asset Inventory — Software Asset Tracking | ISO A.5.9 · SOC 2 CC8.1 · NIST ID.AM · CIS 2 | Asset management treats hardware and software as separate concerns — hardware tracked formally, software managed informally through whoever notices unauthorized installations |
| 🟡 | **66** | GRC Log | Third-Party Risk — Service Provider Management | ISO A.5.19 · SOC 2 CC9.2 · NIST ID.SC · CIS 15 | — |
| 🟢 | **67** | GRC Log | Access Control — Joiner Process | ISO A.5.18 · SOC 2 CC6.1 · NIST PR.AC · CIS 6 | Checklist exists yet managers grant verbal approvals without signing off, leaving no documented authorization trail |
| 🟢 | **68** | Friday Deep Breakdown | Logging Retention & Evidence Integrity | ISO A.8.15 · SOC 2 CC7.2 · NIST DE.CM · CIS 8 | Logs retained on local endpoints where they can be overwritten or deleted before review windows occur, eliminating forensic value |
| ⚪ | **69** | — | *pending* | — | — |
| ⚪ | **70** | — | *pending* | — | — |
| ⚪ | **71** | — | *pending* | — | — |
| 🟡 | **72** | GRC Log | Log Integrity | — | — |
| ⚪ | **73** | — | *pending* | — | — |
| 🟡 | **74** | GRC Log | Access Control — Mover Process | ISO A.5.18 · SOC 2 CC6.1 · NIST PR.AC · CIS 6 | — |
| 🟢 | **75** | Sunday Architecture | Vendor Assurance — Questionnaire vs Independent Testing | ISO A.5.19 · SOC 2 CC9.2 · NIST ID.SC · CIS 15 | Annual questionnaires capture vendor posture at one moment — control degradation between reviews goes undetected |
| 🟢 | **76** | GRC Log | Asset Inventory — Software Licensing | ISO A.5.9 · SOC 2 CC8.1 · NIST ID.AM · CIS 2 | Software discovered during scans yet license status not verified for all installations, leaving compliance gaps undocumented |
| ⚪ | **77** | — | *pending* | — | — |
| 🟡 | **78** | GRC Log | Risk Acceptance & Exception Handling | ISO Clause 6.1 · SOC 2 CC3.2 · NIST ID.RA · CIS 17 | — |
| 🟢 | **79** | GRC Log | Vendor Offboarding | ISO A.5.22 · SOC 2 CC9.2 · NIST ID.SC · CIS 15 | Vendor contracts include termination clauses yet the offboarding checklist is not executed consistently, leaving access revocation dependent on individual memory |
| 🟢 | **80** | Friday Deep Breakdown | Vulnerability Remediation SLA Compliance | ISO A.8.8 · SOC 2 CC7.1 · NIST DE.CM · CIS 7 | High-severity findings ticketed yet remediation driven by engineering sprint cycles rather than risk-based SLAs, allowing critical findings to age past acceptable thresholds |
| ⚪ | **81** | — | *pending* | — | — |
| ⚪ | **82** | — | *pending* | — | — |
| ⚪ | **83** | — | *pending* | — | — |
| ⚪ | **84** | — | *pending* | — | — |
| ⚪ | **85** | — | *pending* | — | — |
| ⚪ | **86** | — | *pending* | — | — |
| ⚪ | **87** | — | *pending* | — | — |
| ⚪ | **88** | — | *pending* | — | — |
| ⚪ | **89** | — | *pending* | — | — |
| ⚪ | **90** | — | *pending* | — | — |
| ⚪ | **91** | — | *pending* | — | — |
| ⚪ | **92** | — | *pending* | — | — |
| ⚪ | **93** | — | *pending* | — | — |
| ⚪ | **94** | — | *pending* | — | — |
| ⚪ | **95** | — | *pending* | — | — |
| ⚪ | **96** | — | *pending* | — | — |
| ⚪ | **97** | — | *pending* | — | — |
| ⚪ | **98** | — | *pending* | — | — |
| ⚪ | **99** | — | *pending* | — | — |
| ⚪ | **100** | — | *pending* | — | — |
| ⚪ | **101** | — | *pending* | — | — |
| ⚪ | **102** | — | *pending* | — | — |
| ⚪ | **103** | — | *pending* | — | — |
| ⚪ | **104** | — | *pending* | — | — |
| ⚪ | **105** | — | *pending* | — | — |
| ⚪ | **106** | — | *pending* | — | — |
| ⚪ | **107** | — | *pending* | — | — |
| ⚪ | **108** | — | *pending* | — | — |
| ⚪ | **109** | — | *pending* | — | — |
| ⚪ | **110** | — | *pending* | — | — |
| ⚪ | **111** | — | *pending* | — | — |
| ⚪ | **112** | — | *pending* | — | — |
| ⚪ | **113** | — | *pending* | — | — |
| ⚪ | **114** | — | *pending* | — | — |
| ⚪ | **115** | — | *pending* | — | — |
| ⚪ | **116** | — | *pending* | — | — |
| ⚪ | **117** | — | *pending* | — | — |
| ⚪ | **118** | — | *pending* | — | — |
| ⚪ | **119** | — | *pending* | — | — |
| 🟡 | **120** | GRC Log | Control Ownership — Independence of Evaluation | SOC 2 CC1.2 · NIST GV.RR · CIS 17 | Control ownership and control execution held by the same role, removing the independence required for objective evaluation |
| 🟢 | **121** | GRC Log | Audit Evidence Requirements by Control Type | ISO A.5.35 · SOC 2 CC4.1 · NIST ID.RA · CIS 17 | Evidence collected reactively during audit preparation rather than defined proactively as part of control design — producing evidence that is sufficient by chance rather than by governance design |
| ⚪ | **122** | — | *pending* | — | — |
| ⚪ | **123** | — | *pending* | — | — |
| ⚪ | **124** | — | *pending* | — | — |
| ⚪ | **125** | — | *pending* | — | — |
| ⚪ | **126** | — | *Continuous Monitoring Architecture* (theme) | — | — |
| ⚪ | **127** | — | *Continuous Monitoring Architecture* (theme) | — | — |
| ⚪ | **128** | — | *Continuous Monitoring Architecture* (theme) | — | — |
| ⚪ | **129** | — | *Continuous Monitoring Architecture* (theme) | — | — |
| ⚪ | **130** | — | *Continuous Monitoring Architecture* (theme) | — | — |
| ⚪ | **131** | — | *Vendor Governance Framework* (theme) | — | — |
| ⚪ | **132** | — | *Vendor Governance Framework* (theme) | — | — |
| ⚪ | **133** | — | *Vendor Governance Framework* (theme) | — | — |
| ⚪ | **134** | — | *Vendor Governance Framework* (theme) | — | — |
| ⚪ | **135** | — | *Vendor Governance Framework* (theme) | — | — |
| ⚪ | **136** | — | *Maturity Modeling & Program Measurement* (theme) | — | — |
| ⚪ | **137** | — | *Maturity Modeling & Program Measurement* (theme) | — | — |
| ⚪ | **138** | — | *Maturity Modeling & Program Measurement* (theme) | — | — |
| ⚪ | **139** | — | *Maturity Modeling & Program Measurement* (theme) | — | — |
| ⚪ | **140** | — | *Maturity Modeling & Program Measurement* (theme) | — | — |
| ⚪ | **141** | — | *Access Governance — Advanced Topics* (theme) | — | — |
| ⚪ | **142** | — | *Access Governance — Advanced Topics* (theme) | — | — |
| ⚪ | **143** | — | *Access Governance — Advanced Topics* (theme) | — | — |
| ⚪ | **144** | — | *Access Governance — Advanced Topics* (theme) | — | — |
| ⚪ | **145** | — | *Access Governance — Advanced Topics* (theme) | — | — |
| ⚪ | **146** | — | *Incident Response Governance & Phase 3 Bridge* (theme) | — | — |
| ⚪ | **147** | — | *Incident Response Governance & Phase 3 Bridge* (theme) | — | — |
| ⚪ | **148** | — | *Incident Response Governance & Phase 3 Bridge* (theme) | — | — |
| ⚪ | **149** | — | *Incident Response Governance & Phase 3 Bridge* (theme) | — | — |
| ⚪ | **150** | — | *Incident Response Governance & Phase 3 Bridge* (theme) | — | — |

---

## Series types

| Series | Cadence | Purpose |
|---|---|---|
| GRC Log | Weekdays | One control scenario in the V2 field structure |
| Friday Deep Breakdown | Friday | Extended treatment — control objective, evidence set, leadership trade-off |
| Saturday Breakdown | Saturday | Real incident analysis cross-mapped across four frameworks |
| Sunday Architecture | Sunday | Program-level design reasoning rather than a single control |

---

*Part of the DakaraiDoesGRC portfolio. Companion repositories: `IT-Inventory-Audit-Template`, `grc-vendor-risk-intake-mini-pack`, `Hands-On-GRC-Starter-Checklist`, `grc-daily-logs-evidence-pack`.*
