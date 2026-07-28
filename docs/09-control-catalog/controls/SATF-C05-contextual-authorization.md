# SATF-C05: Contextual Authorization

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C05 |
| Control Name | Contextual Authorization |
| SATF Area | Ring 2 |
| Outcome Role | Enforce |
| Control Family | Trust Enforcement |
| Status | Draft |

## Purpose

Ensure agent actions are authorized based on identity, intent, objective, context, risk, behavior, and delegation state at the time of action.

## Problem Addressed

Traditional authorization often evaluates static identity, permission, and resource access. Autonomous agents require runtime decisions that account for changing goals, dynamic risk, action context, tool use, data sensitivity, delegation, and mission state.

## Control Statement

Every meaningful autonomous agent action should be evaluated through contextual authorization before execution.

## Implementation Guidance

- Evaluate who is acting, what action is requested, why the action is needed, where the action occurs, when it occurs, and what risk is introduced.
- Include goal state, trust score, delegation provenance, data sensitivity, tool risk tier, and behavior history in the decision.
- Use PDP / PEP patterns to separate decision logic from enforcement.
- Support policy decisions such as allow, deny, constrain, step-up review, monitor, contain, or revoke.
- Fail closed when trust cannot be confidently determined.
- Log decisions for auditability and later assurance.

## Evidence Artifacts

- PDP decision log
- PEP enforcement log
- Policy evaluation record
- Context record
- Tool invocation log
- Step-up approval record
- Denial or containment record

## Related SATF Scenarios

- Prompt Injection to Tool Use
- Goal Overreach
- Unsafe External Action
- Credential Misuse
- Lateral Movement
- Trust Decay

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-02 RAG Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture

## Related Controls

- SATF-C01 Agent Identity
- SATF-C03 Goal Integrity
- SATF-C04 Delegation Provenance

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes
