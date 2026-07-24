# SATF Control Mapping Matrix

## Introduction

Autonomous agents can fail in ways that traditional security frameworks were never designed to address. Problems such as goal overreach, excessive delegation, memory poisoning, prompt injection, sandbox escape, and autonomous lateral movement are not isolated control failures. They are failures of continuous trust management.

The Secure Agent Trust Framework (SATF) Control Mapping Matrix helps security architects, product security teams, platform engineers, governance teams, and auditors understand how SATF capabilities work together to prevent, detect, validate, contain, recover from, and ultimately re-establish trust following agent failures.

Rather than asking:

> Which security control should I deploy?

SATF asks:

> Which framework capabilities should work together to ensure secure outcomes when autonomous agents encounter risk, uncertainty, or compromise?

---

## How to Read the Control Mapping Diagram

The diagram should be read from top to bottom.

### 1. Failure Scenario

The left column represents common autonomous-agent failure scenarios, including:

- Sandbox Escape
- Goal Overreach
- Excessive Delegation
- Memory Poisoning
- Prompt Injection to Tool Use
- Lateral Movement
- Credential Misuse
- Trust Decay

These scenarios represent real-world failure conditions that organizations may encounter during the operation of autonomous agents.

### 2. SATF Capability Coverage

The heatmap shows how strongly each SATF capability contributes to managing a particular scenario.

#### Legend

- **P** = Primary Control Area
- **M** = Major Supporting Control
- **S** = Supporting / Evidence Control

A scenario often requires multiple SATF capabilities working together. The framework intentionally avoids reliance on a single control point.

### 3. Capability Outcome Roles

The row beneath the capability headers explains the primary role each SATF capability performs within the trust lifecycle.

| SATF Capability | Outcome Role |
|---|---|
| Agent Trust Fabric | Assess |
| Ring 1: Trust Establishment | Prevent |
| Ring 2: Trust Enforcement | Prevent + Enforce |
| Ring 3: Trust Validation | Detect + Validate |
| Governance, Telemetry & Assurance Control Plane | Adapt + Assure |
| Runtime & Response Plane | Contain + Recover + Re-establish |

These outcome roles describe **what each capability contributes**, while the heatmap shows **where each capability applies**.

### 4. SATF Response Loop

```text
Agent Failure Signal
        ↓
Trust Fabric Assesses Risk
        ↓
Ring 2 Enforces Policy
        ↓
Ring 3 Validates Evidence
        ↓
Control Plane Adapts Policy
        ↓
Runtime Plane Contains / Recovers
```

SATF Principle:

```text
Validation discovers.
Governance decides.
Enforcement applies.
```

---

## Mapping Controls to Secure Outcomes

The purpose of the matrix is not simply to catalog controls.

The purpose is to show how SATF capabilities collectively support secure outcomes.

SATF exists to help organizations achieve:

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes

Every capability within SATF contributes to one or more of these outcomes through continuous trust assessment, enforcement, validation, adaptation, containment, recovery, and trust re-establishment.

---

## Key Takeaway

The Control Mapping Matrix should be used as a practical bridge between:

```text
Failure Scenarios
        ↓
SATF Capabilities
        ↓
Outcome Roles
        ↓
Secure Outcomes
```

This enables architects, governance teams, and engineering organizations to understand not only where controls exist, but why they exist and how they contribute to trusted autonomous operations.
