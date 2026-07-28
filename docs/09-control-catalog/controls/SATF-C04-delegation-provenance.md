# SATF-C04: Delegation Provenance

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C04 |
| Control Name | Delegation Provenance |
| SATF Area | Agent Trust Fabric / Ring 2 / Ring 3 |
| Outcome Role | Assess + Enforce + Validate |
| Control Family | Agent Trust Fabric / Trust Enforcement / Trust Validation |
| Status | Draft |

## Purpose

Ensure delegated authority across agents remains traceable, scoped, time-bound, revocable, and continuously validated.

## Problem Addressed

Multi-agent systems can create opaque delegation chains where authority expands beyond approved scope. Without delegation provenance, organizations may lose visibility into who delegated authority, what was delegated, for how long, and under what constraints.

## Control Statement

All agent-to-agent delegation should preserve provenance, scope, expiration, authority lineage, and policy constraints throughout the mission lifecycle.

## Implementation Guidance

- Record the origin of delegated authority.
- Capture delegating agent, receiving agent, delegated scope, constraints, and TTL.
- Apply scope attenuation so delegated authority does not exceed the delegator's approved authority.
- Enforce maximum delegation depth where appropriate.
- Require step-up approval for high-risk delegation.
- Validate delegation chains continuously for anomalies, expired authority, or scope creep.
- Revoke delegated authority when trust decays or mission state changes.

## Evidence Artifacts

- Delegation chain record
- Delegation TTL record
- Delegation scope record
- Delegation approval record
- Trust graph update
- Delegation anomaly finding
- Delegation revocation record

## Related SATF Scenarios

- Excessive Delegation
- Delegation Escalation
- Lateral Movement
- Credential Misuse
- Trust Decay

## Related Reference Architectures

- RA-03 Multi-Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C01 Agent Identity
- SATF-C02 Agent Authentication
- SATF-C05 Contextual Authorization

## Expected Outcomes

- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes

## SATF Principle

```text
Delegated Trust Is Not Inherited Trust
```
