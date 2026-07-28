# Out-of-Bound Agent

## Definition

An **Out-of-Bound Agent** is an autonomous agent operating outside approved mission, authority, context, tool, identity, trust, evidence, or runtime boundaries.

## Why this term matters

SATF uses **Out-of-Bound Agent** instead of **Rogue Agent** because most boundary failures do not require malicious intent. An agent can become unsafe simply by optimizing too aggressively, inheriting the wrong context, escaping containment, using a risky tool, or continuing execution after evidence becomes stale.

## Boundary types

```text
Mission Boundary
Authority Boundary
Context Boundary
Tool Boundary
Identity Boundary
Trust Boundary
Evidence Boundary
Runtime / Containment Boundary
```

## Related threats

- SATF-T26 Sandbox Escape
- SATF-T27 Autonomous Exploit Chaining
- SATF-T28 Agentic Swarm Escalation
- SATF-T29 Runtime Containment Failure
- SATF-T30 Boundary Policy Evasion
- SATF-T31 Accountability Gap

## Primary controls

- C09 Least Agency
- C17 Fail-Closed Enforcement
- C18 Agent UEBA
- C19 Adversarial Testing
- C20 Evidence Validation
