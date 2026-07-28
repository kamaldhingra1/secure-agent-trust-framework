# SATF-C08: Human Accountability

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C08 |
| Control Name | Human Accountability |
| SATF Area | Ring 1 |
| Outcome Role | Prevent |
| Control Family | Trust Establishment Controls |
| Status | Draft |

## Purpose

Ensure every autonomous agent and autonomous mission has accountable human ownership for business intent, technical operation, risk acceptance, and governance decisions.

## Problem Addressed

Autonomous agents can make decisions, delegate work, invoke tools, and affect business outcomes. Without clearly assigned accountability, organizations may be unable to determine who approved the mission, who owns risk, who can authorize exceptions, or who is responsible for decommissioning or recovery.

## Control Statement

Every autonomous agent and mission should have assigned accountable human ownership before activation.

## Implementation Guidance

- Assign a business owner responsible for mission purpose, expected outcomes, and risk acceptance.
- Assign a technical owner responsible for implementation, runtime posture, telemetry, and operational readiness.
- Assign an accountable sponsor or governance owner where risk or regulatory exposure is significant.
- Record ownership in the agent inventory and mission trust contract.
- Require owner review for high-risk mission changes, new tools, expanded authority, and delegation policy changes.
- Ensure owners can pause, constrain, or retire the agent or mission.
- Review ownership periodically and during organizational changes.

## Evidence Artifacts

- Human controller record
- Business owner record
- Technical owner record
- Mission approval record
- Risk acceptance record
- Exception approval record
- Decommissioning approval record

## Related SATF Scenarios

- Goal Overreach
- Excessive Delegation
- Trust Decay
- Unsafe External Action
- Decommissioning Failure

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-03 Multi-Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C01 Agent Identity
- SATF-C03 Goal Integrity
- SATF-C04 Delegation Provenance
- SATF-C09 Least Agency

## Expected Outcomes

- Trusted Outcomes
- Compliant Outcomes
- Expected Outcomes
