# SATF Framework Structure

SATF Baseline 1.0 has three coordinated views.

## 1. Conceptual Trust Plane

The conceptual trust plane defines what must be true for an agent to be trusted.

- Core: Agent Trust Fabric
- Ring 1: Trust Establishment
- Ring 2: Trust Enforcement
- Ring 3: Trust Validation

## 2. Cross-Cutting Control Plane

Governance, Telemetry, and Assurance span Ring 1, Ring 2, and Ring 3.

This plane continuously ingests telemetry, assurance findings, audit results, risk changes, and policy exceptions. It then feeds dynamic machine-enforceable policies into Ring 2 Policy Decision Points.

## 3. Runtime and Response Plane

The runtime plane is where SATF is operationalized.

- Runtime Agent Ecosystem
- Response and Containment
- Trusted Agent Outcomes

Response and containment are not a fourth trust ring. They are operational consequences when trust degrades or fails.
