# SATF-C07: Trust Scoring

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C07 |
| Control Name | Trust Scoring |
| SATF Area | Agent Trust Fabric / Control Plane |
| Outcome Role | Assess + Adapt |
| Control Family | Agent Trust Fabric / Control Plane Controls |
| Status | Draft |

## Purpose

Provide a measurable representation of current trust confidence for an agent, mission, delegation chain, or action context.

## Problem Addressed

Trust is often treated as binary: allowed or denied, approved or rejected. Autonomous systems require more nuanced trust states because confidence changes over time as evidence, behavior, risk, and mission context evolve.

Trust scoring enables proportional responses such as monitoring, constraining, step-up review, containment, revocation, or re-establishment.

## Control Statement

The organization should maintain a dynamic trust score or trust state that reflects current confidence in an agent or autonomous mission based on current evidence and policy context.

## Implementation Guidance

- Define trust scoring inputs, including identity assurance, goal integrity, behavior, telemetry, evidence freshness, delegation provenance, tool risk, and validation findings.
- Support both numeric scores and categorical trust states where appropriate.
- Define trust state thresholds such as normal, elevated, degraded, constrained, contained, revoked, or re-established.
- Use trust scores to inform contextual authorization decisions.
- Decay trust when evidence becomes stale, behavior deviates, delegation expands, or validation fails.
- Increase or re-establish trust only through defined recovery and validation steps.
- Avoid using trust scores as opaque decisions; maintain explainability and auditability.

## Evidence Artifacts

- Trust scoring model
- Trust signal inventory
- Trust state transition log
- Trust decay event record
- Trust re-establishment record
- PDP decision log
- Validation finding
- Assurance review record

## Related SATF Scenarios

- Trust Decay
- Excessive Delegation
- Credential Misuse
- Memory Poisoning
- Lateral Movement
- Sandbox Escape

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-03 Multi-Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C06 Agent Risk Evaluation
- SATF-C05 Contextual Authorization
- SATF-C04 Delegation Provenance
- SATF-C10 Memory Integrity

## Expected Outcomes

- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes

## SATF Principle

```text
Trust is not granted once. Trust decays, adapts, and must be continuously re-established through evidence.
```
