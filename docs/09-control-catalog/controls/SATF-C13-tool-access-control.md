# SATF-C13: Tool Access Control

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C13 |
| Control Name | Tool Access Control |
| SATF Area | Ring 2 |
| Outcome Role | Enforce |
| Control Family | Trust Enforcement Controls |
| Status | Draft |

## Purpose

Ensure autonomous agents can only invoke approved tools under authorized mission context, defined risk thresholds, and appropriate supervision levels.

## Problem Addressed

Tools expand agent capability. A tool-enabled agent may browse, execute code, call APIs, modify repositories, access databases, trigger workflows, or perform external actions. Without tool access controls, a prompt injection or goal overreach condition can become a high-impact operational event.

## Control Statement

Agent tool access should be explicitly approved, risk-classified, policy-enforced, logged, and continuously governed throughout mission execution.

## Implementation Guidance

- Maintain an approved tool inventory for agent use.
- Classify tools by risk tier, action type, data sensitivity, and reversibility.
- Require contextual authorization before tool invocation.
- Enforce least agency for tool use, including read, write, execute, delegate, and external action scopes.
- Require approval gates for high-impact or irreversible tools.
- Log tool invocations, parameters, outputs, and decision context.
- Disable or constrain tools when trust decays or anomalies are detected.

## Evidence Artifacts

- Approved tool inventory
- Tool risk classification
- Tool access policy
- Tool invocation log
- PDP / PEP decision log
- Approval record
- Tool disablement record
- Tool assurance review

## Related SATF Scenarios

- Prompt Injection to Tool Use
- Goal Overreach
- Unsafe External Action
- Sandbox Escape
- Lateral Movement
- Trust Decay

## Related Reference Architectures

- RA-01 Single Agent Reference Architecture
- RA-02 RAG Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C05 Contextual Authorization
- SATF-C09 Least Agency
- SATF-C12 Supply Chain Integrity
- SATF-C15 Objective Boundary Enforcement

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Resilient Outcomes
- Expected Outcomes
