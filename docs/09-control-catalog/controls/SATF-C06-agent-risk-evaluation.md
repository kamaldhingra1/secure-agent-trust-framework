# SATF-C06: Agent Risk Evaluation

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C06 |
| Control Name | Agent Risk Evaluation |
| SATF Area | Agent Trust Fabric |
| Outcome Role | Assess |
| Control Family | Agent Trust Fabric Controls |
| Status | Draft |

## Purpose

Continuously evaluate the risk associated with an autonomous agent, mission, action, context, delegation chain, tool invocation, and runtime state.

## Problem Addressed

Autonomous agents operate in dynamic conditions. A request that appears acceptable at mission start may become risky because context changes, delegated authority expands, tools change, evidence becomes stale, or behavior deviates from expected patterns.

Without agent risk evaluation, organizations may continue allowing actions even when trust signals indicate increased uncertainty or risk.

## Control Statement

The organization should continuously evaluate agent risk using identity, intent, goal, context, behavior, delegation provenance, tool risk, data sensitivity, telemetry, and validation evidence.

## Implementation Guidance

- Define risk signals used by the Agent Trust Fabric.
- Include identity, mission objective, current context, delegated authority, data sensitivity, tool risk, and behavior history.
- Evaluate risk before high-impact actions, external actions, sensitive data access, delegation, and memory writes.
- Use validation findings and telemetry to update risk during execution.
- Support risk outcomes such as allow, constrain, step-up review, monitor, contain, revoke, or re-establish trust.
- Document thresholds for acceptable, elevated, degraded, and unacceptable risk states.
- Ensure risk evaluation outputs are available to Ring 2 enforcement and the Control Plane.

## Evidence Artifacts

- Agent risk model
- Risk signal inventory
- Risk score calculation record
- PDP decision log
- Delegation risk record
- Tool risk classification
- Data sensitivity classification
- Validation finding
- Trust state transition record

## Related SATF Scenarios

- Trust Decay
- Goal Overreach
- Excessive Delegation
- Lateral Movement
- Prompt Injection to Tool Use
- Unsafe External Action

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-02 RAG Agent Reference Architecture
- RA-03 Multi-Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C03 Goal Integrity
- SATF-C04 Delegation Provenance
- SATF-C05 Contextual Authorization
- SATF-C07 Trust Scoring

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes
