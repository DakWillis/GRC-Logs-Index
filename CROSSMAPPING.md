# Framework crossmapping

Every framework control referenced in the archive, mapped to the day numbers that cover it. Use this to find the scenario behind a control you are being audited against — or studying toward.

Only confirmed mappings appear here. Entries still pending backfill are absent by design rather than by omission; see [`../docs/PROVENANCE.md`](../docs/PROVENANCE.md).

Back to [master index](../INDEX.md).

---

### ISO/IEC 27001:2022

| Control | Days | Count |
|---|---|---|
| `A.5.9` | 17, 27, 65, 76 | 4 |
| `A.5.11` | 29 | 1 |
| `A.5.12` | 53 | 1 |
| `A.5.15` | 59 | 1 |
| `A.5.18` | 67, 74 | 2 |
| `A.5.19` | 66, 75 | 2 |
| `A.5.22` | 79 | 1 |
| `A.5.35` | 121 | 1 |
| `A.6.3` | 55 | 1 |
| `A.8.8` | 58, 80 | 2 |
| `A.8.9` | 52, 60 | 2 |
| `A.8.15` | 61, 68 | 2 |
| `A.8.20` | 54 | 1 |
| `A.8.24` | 57 | 1 |
| `A.8.32` | 56 | 1 |
| `Clause 6.1` | 78 | 1 |

### SOC 2 Trust Services Criteria

| Control | Days | Count |
|---|---|---|
| `CC1.2` | 120 | 1 |
| `CC2.2` | 55 | 1 |
| `CC3.2` | 53, 78 | 2 |
| `CC4.1` | 121 | 1 |
| `CC6.1` | 17, 27, 67, 74 | 4 |
| `CC6.2` | 59 | 1 |
| `CC6.6` | 54 | 1 |
| `CC6.7` | 57 | 1 |
| `CC7.1` | 52, 58, 60, 80 | 4 |
| `CC7.2` | 61, 68 | 2 |
| `CC8.1` | 56, 65, 76 | 3 |
| `CC9.2` | 66, 75, 79 | 3 |

### NIST CSF 2.0

| Control | Days | Count |
|---|---|---|
| `DE.CM` | 58, 61, 68, 80 | 4 |
| `GV.RR` | 120 | 1 |
| `ID.AM` | 17, 27, 65, 76 | 4 |
| `ID.RA` | 78, 121 | 2 |
| `ID.SC` | 66, 75, 79 | 3 |
| `PR.AC` | 16, 54, 59, 67, 74 | 5 |
| `PR.AT` | 55 | 1 |
| `PR.DS` | 53, 57 | 2 |
| `PR.IP` | 52, 56, 60 | 3 |

### CIS Controls v8.1

| Control | Days | Count |
|---|---|---|
| `CIS 1` | 17, 27 | 2 |
| `CIS 2` | 65, 76 | 2 |
| `CIS 3` | 53, 57 | 2 |
| `CIS 4` | 52, 56, 60 | 3 |
| `CIS 5` | 16 | 1 |
| `CIS 6` | 59, 67, 74 | 3 |
| `CIS 7` | 58, 80 | 2 |
| `CIS 8` | 61, 68 | 2 |
| `CIS 12` | 54 | 1 |
| `CIS 14` | 55 | 1 |
| `CIS 15` | 66, 75, 79 | 3 |
| `CIS 17` | 78, 120, 121 | 3 |

---

**A note on the four frameworks.** They are not four separate requirements. They are four dialects describing the same control loop. ISO 27001 states the control objective, SOC 2 states the criterion an auditor tests against, NIST CSF states the outcome category, and CIS states the technical safeguard. An entry mapped across all four is the same scenario translated four ways — which is the actual skill the archive is built to demonstrate.
