# SATF-C20: Evidence Validation

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C20 |
| Control Name | Evidence Validation |
| SATF Area | Ring 3 / Control Plane |
| Outcome Role | Validate + Assure |
| Control Family | Trust Validation / Control Plane Controls |
| Status | Draft |

## Purpose

Ensure trust decisions are based on sufficient, current, reliable, and relevant evidence.

## Problem Addressed

Autonomous missions may continue operating based on stale, incomplete, missing, conflicting, or low-quality evidence. If evidence quality degrades, trust decisions become less reliable even when technical systems appear healthy.

## Control Statement

The organization should validate the freshness, completeness, provenance, reliability, and relevance of evidence used to make trust decisions.

## Implementation Guidance

- Define evidence requirements for each mission, agent type, tool risk tier, and data sensitivity level.
- Validate evidence freshness before high-impact decisions.
- Track evidence provenance, source, time, owner, and integrity.
- Detect missing, stale, conflicting, or low-confidence evidence.
- Trigger trust decay or step-up review when evidence confidence is insufficient.
- Maintain evidence packages for regulated, high-impact, or auditable missions.
- Feed evidence validation findings into Control Plane governance and TrustOps metrics.

## Evidence Artifacts

- Evidence requirement specification
- Evidence inventory
- Evidence freshness report
- Evidence provenance record
- Evidence validation finding
- Assurance evidence package
- Trust decision record
- Governance review record

## Related SATF Scenarios

- Trust Decay
- Regulated Workflow Drift
- Goal Overreach
- Unsafe External Action
- Credential Misuse
- Memory Poisoning

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C06 Agent Risk Evaluation
- SATF-C07 Trust Scoring
- SATF-C18 Agent UEBA
- SATF-C19 Adversarial Testing

## Expected Outcomes

- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes

## SATF Principle

```text
Trust decisions require evidence. Stale evidence weakens trust.
```
