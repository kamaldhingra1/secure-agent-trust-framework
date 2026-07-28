# TrustOps: Operating Trusted Autonomy

## Positioning

TrustOps is an implementation pattern based on SATF. It is not a replacement for the SATF framework.

SATF defines the trust model, trust lifecycle, trust fabric, trust rings, control plane, runtime plane, and secure outcome expectations.

TrustOps describes how organizations operate SATF in production to continuously manage Mission Trust.

```text
SATF defines what good looks like.
TrustOps describes how to operate it.
```

## Why TrustOps exists

Existing operational disciplines such as SecOps, MLOps, SRE, AIOps, IAM, platform engineering, product security, and GRC provide critical capabilities. However, none of these disciplines is singularly accountable for maintaining trust throughout the execution of an autonomous mission.

A mission may remain technically available, operationally performant, and policy compliant while drifting away from its intended business objective. An agent may use stale knowledge, invoke a tool that has not been sufficiently validated, or delegate authority beyond approved boundaries.

These situations may not begin as cybersecurity incidents, but they directly affect enterprise confidence in the mission.

TrustOps exists to fill that operational gap.

## Definition

TrustOps is the operational discipline responsible for continuously establishing, observing, evaluating, governing, recovering, learning from, and measuring Mission Trust throughout the lifecycle of autonomous missions.

## Relationship to SATF

| SATF Concept | TrustOps Application |
|---|---|
| Secure Outcomes | Defines the objective of trusted autonomy |
| Agent Trust Fabric | Provides trust assessment inputs |
| Ring 1 | Establishes baseline mission trust |
| Ring 2 | Enforces trust decisions |
| Ring 3 | Produces validation evidence |
| Control Plane | Governs and adapts trust policies |
| Runtime Plane | Contains, recovers, and re-establishes trust |

## TrustOps is an integrator

TrustOps does not replace existing operational teams. TrustOps coordinates evidence from those teams into a continuous assessment of Mission Trust.

| Discipline | Evidence Contribution |
|---|---|
| SecOps | Threat intelligence, security events, indicators of compromise |
| MLOps | Model evaluation, drift detection, deployment posture |
| SRE | Service reliability, availability, performance signals |
| IAM | Identity, access, credential, and delegation signals |
| GRC | Policy requirements, exceptions, risk thresholds |
| Platform Engineering | Runtime health, platform telemetry, operational controls |
| Product Security | Threat models, design reviews, secure development evidence |

## Diagram

![TrustOps Operating Model](../../../assets/diagrams/implementation-patterns/trustops-operating-model.png)

Mermaid source:

```text
assets/diagrams/implementation-patterns/trustops-operating-model.mmd
```
