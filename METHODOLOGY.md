# Methodology — the control loop

Every entry in this archive is one station on a single loop. The loop is what GRC actually is; the frameworks are dialects describing it.

Back to [master index](INDEX.md).

---

## The loop

```
Context → Risk → Control → Evidence → Test → Finding
                                                 ↓
        Monitoring ← Remediation ← Communication
                 ↓
              (back to Context)
```

| Station | The question it answers |
|---|---|
| **Context** | What is this environment actually like — size, tooling, ownership, constraints? |
| **Risk** | What is exposed, stated as a consequence rather than a category? |
| **Control** | What activity, performed by whom and how often, addresses it? |
| **Evidence** | What artifact proves the activity happened, not that a policy exists? |
| **Test** | How would an independent party confirm the control operated as described? |
| **Finding** | What did the test reveal, stated in a way a decision-maker can act on? |
| **Communication** | How is it framed so the trade-off is visible to whoever must approve it? |
| **Remediation** | What changed, who owned it, when did it close? |
| **Monitoring** | What detects recurrence without waiting for the next audit? |

## Why the loop matters more than the frameworks

ISO 27001 states the control objective. SOC 2 states the criterion an auditor tests against. NIST CSF 2.0 states the outcome category. CIS Controls state the technical safeguard. All four are describing the same loop from different vantage points, which is why every entry here maps to all four rather than picking one.

Learning four frameworks separately means learning the same thing four times. Learning the loop means the frameworks become translation, and translation is fast.

## Why the archive emphasizes failure mode

Most control documentation stops at the Control station. The control is written, approved, and reported as operating — and the report is accurate. The control genuinely exists.

The failure happens between **Control** and **Evidence**, or between **Test** and **Finding**. Specifically:

- A control is defined and never validated after deployment, so drift is invisible
- Evidence is generated in a form that cannot survive to the moment it is needed
- The review cadence is slower than the environment's rate of change
- An exception path is used often enough that it silently becomes the process
- The person evaluating the control is the person operating it, so independence is absent

None of those are visible in a control register. All of them are visible in a failure mode field. That is why the field exists.

## Where automation is going, and what it does not touch

Evidence collection, control testing, and monitoring are being absorbed by tooling, and that absorption will continue. It is a good thing — those stations are mechanical and benefit from being mechanized.

What stays human is the rest of the loop. **Context** requires knowing why this organization operates the way it does. **Finding** requires judgment about materiality. **Communication** requires understanding what a leadership team is actually trading off. **Remediation** requires negotiating change with people who have competing priorities.

A practitioner who can only run the mechanical stations is automating themselves. A practitioner who can close the loop between written policy and technical reality — verifying controls rather than accepting attestations — is doing the part that compounds.

## The V2 field structure

The field structure used across the archive maps directly onto the loop:

| Field | Loop station |
|---|---|
| Environment | Context |
| Risk | Risk |
| Control | Control |
| Evidence | Evidence + Test |
| Failure Mode | Finding (anticipated) |
| Risk Score | Communication — the trade-off made legible |

Risk Score is written as `Likelihood / Impact → Residual`. The arrow is the point: it states what the control is expected to achieve, which makes the control testable rather than decorative.
