# SATF-C17: Fail-Closed Enforcement

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C17 |
| Control Name | Fail-Closed Enforcement |
| SATF Area | Ring 2 / Runtime Plane |
| Outcome Role | Enforce + Contain |
| Control Family | Trust Enforcement / Runtime Response Controls |
| Status | Draft |

## Purpose

Ensure autonomous agent actions are denied, constrained, paused, or contained when trust cannot be confidently determined.

## Problem Addressed

Autonomous agents may operate under ambiguous evidence, incomplete context, unavailable policy systems, stale trust scores, degraded telemetry, or conflicting authorization signals. If the system fails open, an agent may continue acting despite insufficient trust justification.

## Control Statement

When required trust evidence, policy decisions, identity assurance, or authorization context is unavailable or inconclusive, the system should fail closed by denying, constraining, pausing, or containing the action.

## Implementation Guidance

- Define conditions that require fail-closed behavior.
- Fail closed when identity, context, trust score, policy, delegation provenance, tool status, or evidence cannot be validated.
- Use constrained modes where complete denial is not required but full autonomy is no longer justified.
- Require human review when fail-closed events affect mission continuity.
- Log fail-closed decisions and associated missing evidence.
- Ensure runtime systems can safely pause, block, or rollback agent actions.
- Test fail-closed conditions during assurance and adversarial validation.

## Evidence Artifacts

- Fail-closed policy
- Denial decision log
- Missing evidence record
- Constrained mode record
- Runtime containment record
- Human review record
- Recovery / re-establishment record

## Related SATF Scenarios

- Prompt Injection to Tool Use
- Sandbox Escape
- Unsafe External Action
- Trust Decay
- Lateral Movement
- Credential Misuse

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C05 Contextual Authorization
- SATF-C07 Trust Scoring
- SATF-C13 Tool Access Control
- SATF-C16 Approval Gates

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes

## SATF Principle

```text
When trust cannot be justified, autonomy should be constrained.
```
