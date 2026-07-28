# SATF-C16: Approval Gates

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C16 |
| Control Name | Approval Gates |
| SATF Area | Ring 2 / Control Plane |
| Outcome Role | Enforce + Govern |
| Control Family | Trust Enforcement / Control Plane Controls |
| Status | Draft |

## Purpose

Require explicit approval before autonomous agents perform high-risk, irreversible, regulated, externally visible, or business-impacting actions.

## Problem Addressed

Autonomous agents may attempt actions that are technically authorized but operationally sensitive. Examples include production changes, external communications, delegated authority expansion, regulated workflow actions, incident response actions, data export, or destructive operations. Without approval gates, an agent may move from recommendation to impact without sufficient oversight.

## Control Statement

The organization should define and enforce approval gates for autonomous agent actions that exceed predefined risk, impact, sensitivity, or autonomy thresholds.

## Implementation Guidance

- Define approval triggers based on risk tier, data sensitivity, tool risk, production impact, regulatory impact, reversibility, and external exposure.
- Require human approval for high-impact or irreversible actions.
- Support step-up review when trust score, evidence confidence, or mission context changes.
- Capture approver identity, approval rationale, approval scope, expiration, and constraints.
- Enforce approval gates through Ring 2 PDP / PEP controls.
- Revalidate approval when mission context, delegated authority, or objective boundaries change.
- Ensure approval gates are auditable and reviewed periodically.

## Evidence Artifacts

- Approval policy
- Approval trigger catalog
- Human approval record
- Step-up review record
- PDP / PEP decision log
- Action execution record
- Approval expiration record
- Exception record

## Related SATF Scenarios

- Goal Overreach
- Unsafe External Action
- Excessive Delegation
- Credential Misuse
- Regulated Workflow Drift
- False-Positive Driven Response

## Related Reference Architectures

- RA-03 Multi-Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C03 Goal Integrity
- SATF-C05 Contextual Authorization
- SATF-C06 Agent Risk Evaluation
- SATF-C15 Objective Boundary Enforcement

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Expected Outcomes
