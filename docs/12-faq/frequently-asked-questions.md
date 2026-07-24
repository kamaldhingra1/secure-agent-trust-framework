# SATF Frequently Asked Questions

## What Exactly Is the Agent Trust Fabric?

The **Agent Trust Fabric** is the decision engine at the center of SATF. It continuously evaluates Identity, Intent, Task Context, Goal, Dynamic Risk Score, Behavior, and Delegation Provenance to determine whether an agent should be allowed, constrained, monitored, contained, revoked, or re-established.

Short version:

```text
Agent Trust Fabric = dynamic trust evaluation engine for autonomous agents.
```

## How Is SATF Different From Zero Trust?

Zero Trust protects access. SATF protects autonomous decisions.

Zero Trust is foundational to SATF, but autonomous agents require additional controls around goal integrity, delegation provenance, trust lifecycle, trust decay, adaptive trust policies, continuous reassessment, and trust recovery.

Short version:

```text
Zero Trust asks: should this identity access this resource?
SATF asks: should this agent perform this action, for this goal, in this context, right now?
```

## How Is SATF Different From ATF?

ATF focuses primarily on governance domains such as Identity, Behavior, Data Governance, Segmentation, Incident Response, and autonomy maturity.

SATF adds a continuous trust operating model: Agent Trust Fabric, Trust Lifecycle, Goal Integrity, Delegation Provenance, Trust Decay, Continuous Trust Reassessment, Adaptive Trust Policies, Runtime Trust Operations, and re-establishment after containment.

Short version:

```text
ATF is governance-oriented.
SATF is continuous-trust-operations-oriented.
```

## Why Does Goal Integrity Matter?

A legitimate goal can still produce unsafe outcomes. For example, an agent asked to reduce cloud cost might delete backups, disable monitoring, or terminate critical production assets if goal boundaries are not enforced.

Goal Integrity ensures objectives remain valid, bounded, and pursued through approved paths.

SATF Principle:

```text
Goal Approved != Every Action Approved
```

## Why Is Delegation Provenance Needed?

Modern agent systems frequently delegate tasks across agents.

```text
Human -> Agent A -> Agent B -> Agent C -> Action
```

Delegation Provenance ensures authority remains traceable, scoped, time-bound, revocable, and continuously validated.

SATF Principle:

```text
Delegated Trust Is Not Inherited Trust
```

## Why Does Ring 3 Not Perform Enforcement?

Ring 3 validates trust assumptions and produces evidence. It does not directly enforce runtime policy.

SATF separates responsibilities:

```text
Validation discovers.
Governance decides.
Enforcement applies.
```

Ring 3 produces evidence, the Cross-Cutting Control Plane converts evidence into adaptive policy, and Ring 2 enforces that policy through PDP/PEP controls.

## How Does Trust Decay and Get Re-Established?

Trust can decay due to goal drift, excessive delegation, unsafe tool usage, memory poisoning, policy violations, behavioral anomalies, threat intelligence, or failed assurance tests.

Typical SATF progression:

```text
Allow -> Constrain -> Step-Up Review -> Monitor -> Contain -> Revoke
```

Trust can later be re-established through revalidation, recovery actions, credential rotation, policy updates, remediation, assurance testing, and human approval.

## One-Line Summary

SATF is a continuous trust operating model that establishes, enforces, validates, reassesses, adapts, contains, and re-establishes trust for autonomous agents.
