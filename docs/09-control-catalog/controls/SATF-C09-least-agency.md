# SATF-C09: Least Agency

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C09 |
| Control Name | Least Agency |
| SATF Area | Ring 1 / Ring 2 |
| Outcome Role | Prevent + Enforce |
| Control Family | Trust Establishment / Trust Enforcement Controls |
| Status | Draft |

## Purpose

Limit the autonomous decision-making power, action scope, tool access, data access, and delegation authority of agents to the minimum necessary for the approved mission.

## Problem Addressed

Traditional least privilege focuses on what an identity can access. Autonomous agents require a broader control because risk is also driven by what the agent can decide, perform, optimize, modify, invoke, delegate, and persist.

Without least agency, agents may accumulate excessive autonomy, expand blast radius, overreach goals, or delegate authority beyond intended boundaries.

## Control Statement

The organization should constrain each agent's autonomy, actions, tools, data, memory, and delegation authority to the minimum required for the approved mission.

## Implementation Guidance

- Define the approved autonomy level for each agent or mission.
- Limit tools, data sources, write permissions, external actions, and delegation authority.
- Separate read, write, execute, delegate, and external action permissions.
- Require step-up approval for actions outside normal autonomy boundaries.
- Apply scoped credentials and just-in-time access where possible.
- Review autonomy scope when mission objectives, tools, or environments change.
- Continuously monitor for autonomy expansion or scope drift.

## Evidence Artifacts

- Agent autonomy classification
- Tool access policy
- Data access policy
- Delegation policy
- Credential scope record
- Approval gate record
- Autonomy review record
- Scope drift finding

## Related SATF Scenarios

- Goal Overreach
- Sandbox Escape
- Lateral Movement
- Excessive Delegation
- Unsafe External Action
- Credential Misuse

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-03 Multi-Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C01 Agent Identity
- SATF-C02 Agent Authentication
- SATF-C04 Delegation Provenance
- SATF-C05 Contextual Authorization

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes

## SATF Principle

```text
Least privilege limits access. Least agency limits autonomous power.
```
