# SATF Rings and Operational Capabilities

## Why the Trust Rings Exist

SATF organizes trust controls into three complementary trust rings.

The rings are not maturity levels. The rings are not sequential deployment phases. All three operate continuously throughout the agent lifecycle.

The rings answer three fundamental questions:

```text
Ring 1: Can this agent exist and operate safely?
Ring 2: Should this action occur right now?
Ring 3: Do we still trust the agent, controls, and environment?
```

## Ring 1: Trust Establishment

### Core Question

> Can this agent exist and operate safely?

Ring 1 establishes the initial trust posture before an agent receives credentials, tools, memory access, data access, or delegated authority.

### Why Ring 1 matters

Without trust establishment:

- ownership becomes unclear
- privileges accumulate
- supply chain risk increases
- blast radius expands
- accountability disappears

### Key capabilities

- Human Controllers
- Agent Identity
- Credential Security
- Least Agency
- Runtime Sandboxing
- Supply Chain Integrity
- Memory Integrity
- Lifecycle Governance
- Decommissioning

### SATF principle

```text
Trust cannot be continuously enforced if it was never properly established.
```

## Ring 2: Trust Enforcement

### Core Question

> Should this action occur right now?

Ring 2 is SATF's runtime authorization and policy enforcement layer.

Most significant agent failures are authorization failures, not authentication failures. The agent had valid credentials, but the action should not have occurred under the current context.

### Key capabilities

- Contextual Authorization
- PDP/PEP Controls
- Goal Boundary Enforcement
- Tool Governance
- Data Governance
- Delegation Controls
- Step-Up Review
- Fail-Closed Enforcement

### Contextual authorization model

SATF evaluates:

```text
Identity
Intent
Goal
Context
Risk
Behavior
Delegation Chain
```

### SATF principle

```text
Authentication proves identity.
Enforcement determines whether the action should occur.
```

## Ring 3: Trust Validation

### Core Question

> Do we still trust the agent, controls, and operating environment?

Trust assumptions degrade over time. Goals evolve. Systems change. Dependencies change. Threats change. Ring 3 continuously validates whether trust assumptions remain true.

### Key capabilities

- Goal Integrity Validation
- Reward-Hacking Detection
- Observable Planning
- Agent UEBA
- Rule of Two
- Adversarial Testing
- Containment Trigger Validation
- Assurance Evidence Generation

### Why Ring 3 does not enforce

SATF intentionally separates validation from enforcement.

```text
Validation discovers.
Governance decides.
Enforcement applies.
```

Ring 3 produces evidence. The Cross-Cutting Control Plane converts evidence into policy. Ring 2 enforces policy.

## Goal Integrity

A legitimate goal can still produce unsafe outcomes.

Goal Integrity validates:

- Objective legitimacy
- Objective persistence
- Success constraints
- Goal drift
- Forbidden paths
- Reward hacking

SATF principle:

```text
Goal Approved != Every Action Approved
```

## Delegation Provenance

Modern agent systems increasingly operate using delegation chains.

```text
Human -> Agent A -> Agent B -> Agent C
```

SATF tracks:

- Origin of authority
- Delegation scope
- Delegation expiration
- Delegation constraints
- Lineage back to the human controller or approved workflow

SATF principle:

```text
Delegated Trust Is Not Inherited Trust
```

## Continuous Trust Reassessment

Trust is continuously recalculated based on:

- Telemetry
- Validation findings
- Threat intelligence
- Behavioral drift
- Goal drift
- Delegation changes
- Policy violations
- Assurance evidence

Typical trust decay path:

```text
Allow -> Constrain -> Step-Up Review -> Monitor -> Contain -> Revoke
```

Trust can be re-established through:

- Revalidation
- Remediation
- Credential rotation
- Policy updates
- Human approval
- Assurance testing
