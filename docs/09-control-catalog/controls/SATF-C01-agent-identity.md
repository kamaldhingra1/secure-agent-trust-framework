# SATF-C01: Agent Identity

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C01 |
| Control Name | Agent Identity |
| SATF Area | Agent Trust Fabric / Ring 1 |
| Outcome Role | Assess + Prevent |
| Control Family | Agent Trust Fabric / Trust Establishment |
| Status | Draft |

## Purpose

Ensure every autonomous agent has a unique, attributable, lifecycle-managed identity that can be used for trust evaluation, policy enforcement, telemetry correlation, delegation tracking, and auditability.

## Problem Addressed

Autonomous agents can execute actions, invoke tools, access data, delegate tasks, and modify state. Without a unique identity, organizations cannot reliably attribute actions, enforce policy, evaluate trust, revoke access, or investigate failures.

## Control Statement

Every autonomous agent should be assigned a unique identity before receiving credentials, tools, memory access, data access, or delegated authority.

## Implementation Guidance

- Assign each agent a unique identity separate from human users and shared service accounts.
- Bind the identity to an accountable human controller, technical owner, and business owner.
- Track lifecycle state such as proposed, approved, active, constrained, suspended, retired, or revoked.
- Include identity metadata in telemetry, tool calls, memory writes, policy decisions, and delegation records.
- Avoid shared credentials across agents unless explicitly justified and risk accepted.
- Ensure identity can be revoked quickly when trust decays or the agent is decommissioned.

## Evidence Artifacts

- Agent inventory record
- Agent identity record
- Ownership record
- Credential issuance record
- Lifecycle state record
- Revocation record
- Audit logs containing agent identity

## Related SATF Scenarios

- Credential Misuse
- Lateral Movement
- Excessive Delegation
- Trust Decay
- Decommissioning Failure

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-03 Multi-Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C02 Agent Authentication
- SATF-C04 Delegation Provenance
- SATF-C05 Contextual Authorization

## Expected Outcomes

- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes
