# SATF-C02: Agent Authentication

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C02 |
| Control Name | Agent Authentication |
| SATF Area | Ring 1 / Ring 2 |
| Outcome Role | Prevent + Enforce |
| Control Family | Trust Establishment / Trust Enforcement |
| Status | Draft |

## Purpose

Ensure agents authenticate using approved, verifiable, scoped, and lifecycle-managed credentials before accessing tools, data, memory, APIs, or mission resources.

## Problem Addressed

Unverified or weakly authenticated agents can misuse credentials, impersonate approved agents, access unauthorized resources, or make it difficult to distinguish trusted activity from compromised or rogue activity.

## Control Statement

Autonomous agents should authenticate with strong, scoped, revocable credentials before performing any action that accesses data, tools, APIs, memory, or external systems.

## Implementation Guidance

- Use unique credentials bound to the agent identity.
- Prefer short-lived credentials and just-in-time authorization.
- Scope credentials to agent role, mission context, approved tools, and data boundaries.
- Rotate credentials on schedule and immediately after trust degradation.
- Prevent credential reuse across unrelated agents or missions.
- Capture credential use in telemetry and policy decision logs.
- Require stronger authentication or step-up review for high-risk actions.

## Evidence Artifacts

- Credential issuance log
- Credential rotation log
- Authentication event log
- Token scope record
- Revocation record
- PDP / PEP decision log

## Related SATF Scenarios

- Credential Misuse
- Lateral Movement
- Sandbox Escape
- Trust Decay

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-01 Single Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-05 Autonomous Security Agent Reference Architecture

## Related Controls

- SATF-C01 Agent Identity
- SATF-C05 Contextual Authorization
- SATF-C04 Delegation Provenance

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
