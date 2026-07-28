# SATF-C18: Agent UEBA

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C18 |
| Control Name | Agent UEBA |
| SATF Area | Ring 3 / Control Plane |
| Outcome Role | Detect + Validate |
| Control Family | Trust Validation / Control Plane Controls |
| Status | Draft |

## Purpose

Detect abnormal or risky agent behavior by comparing current activity against expected mission behavior, agent role, tool use, data access, delegation patterns, and historical baselines.

## Problem Addressed

Autonomous agents may drift, become compromised, misuse tools, access unusual data, escalate delegation, or behave inconsistently with their assigned mission. Traditional user behavior analytics may not capture agent-specific patterns such as tool invocation sequences, goal drift, memory influence, delegation lineage, or autonomous action velocity.

## Control Statement

The organization should monitor agent behavior for anomalies using agent-specific UEBA signals and incorporate findings into trust evaluation, enforcement, and response.

## Implementation Guidance

- Define expected behavior profiles for each agent type, mission, tool set, data scope, and autonomy level.
- Monitor tool usage, access patterns, delegation chains, action frequency, data movement, memory writes, and external actions.
- Identify deviations from expected role, goal, context, or historical behavior.
- Correlate UEBA findings with trust score, risk evaluation, and policy decisions.
- Trigger step-up review, constrained mode, containment, or trust decay when anomalies exceed thresholds.
- Review false positives and tune behavioral models.

## Evidence Artifacts

- Agent behavior baseline
- UEBA detection rule or model
- Anomaly alert
- Tool usage profile
- Delegation behavior record
- Trust score update
- Investigation record
- Tuning record

## Related SATF Scenarios

- Lateral Movement
- Trust Decay
- Credential Misuse
- Memory Poisoning
- Excessive Delegation
- Sandbox Escape

## Related Reference Architectures

- RA-03 Multi-Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C06 Agent Risk Evaluation
- SATF-C07 Trust Scoring
- SATF-C04 Delegation Provenance
- SATF-C20 Evidence Validation

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes
