# SATF Control Catalog

The SATF Control Catalog translates the Secure Agent Trust Framework into implementable controls.

The catalog is designed to help architects, product security teams, AI platform teams, governance teams, and assurance teams answer:

> What controls should be implemented to establish, enforce, validate, adapt, recover, and re-establish trust for autonomous agents?

## Why this catalog exists

SATF is organized around secure outcomes, the Agent Trust Fabric, trust rings, the Governance, Telemetry, and Assurance Control Plane, and the Runtime and Response Plane.

The Control Catalog connects those concepts to practical implementation guidance.

## How to use this catalog

Each control includes:

- Control ID
- Control name
- SATF area
- Outcome role
- Purpose
- Problem addressed
- Implementation guidance
- Evidence artifacts
- Related SATF scenarios
- Related reference architectures
- Related controls
- Expected outcomes

## Initial control set

The first five controls define the core SATF trust foundation:

| Control ID | Control Name | SATF Area | Outcome Role |
|---|---|---|---|
| SATF-C01 | Agent Identity | Agent Trust Fabric / Ring 1 | Assess + Prevent |
| SATF-C02 | Agent Authentication | Ring 1 / Ring 2 | Prevent + Enforce |
| SATF-C03 | Goal Integrity | Agent Trust Fabric / Ring 2 / Ring 3 | Assess + Enforce + Validate |
| SATF-C04 | Delegation Provenance | Agent Trust Fabric / Ring 2 / Ring 3 | Assess + Enforce + Validate |
| SATF-C05 | Contextual Authorization | Ring 2 | Enforce |

## Control families

The complete catalog will be organized into six families:

1. Agent Trust Fabric Controls
2. Ring 1: Trust Establishment Controls
3. Ring 2: Trust Enforcement Controls
4. Ring 3: Trust Validation Controls
5. Governance, Telemetry, and Assurance Control Plane Controls
6. Runtime and Response Plane Controls

## SATF principle

```text
Secure outcomes are the goal.
Controls exist to continuously establish, enforce, validate, adapt, contain, recover, and re-establish trust.
```
