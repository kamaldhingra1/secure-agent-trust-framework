# Secure Agent Trust Framework (SATF) Baseline 1.0
### Safe, Trusted, Compliant, Resilient, and Expected Outcomes

![App Logo](assets/diagrams/satf-baseline-1.0-framework.png)

**End-to-End Enterprise Framework for Autonomous Agent Governance and Contextual Security**

SATF is a vendor-neutral framework for establishing, enforcing, validating, reassessing, adapting, and revoking trust in autonomous agent systems.

## Core idea

Trust is not granted once. Trust is dynamic. Trust is established, consumed, validated, reassessed, adapted, and revoked or re-established when needed.

# Why SATF Exists

Traditional security frameworks focus on securing identities, access, resources, networks, and applications.

Autonomous agents introduce a different challenge.

The fundamental objective is no longer simply protecting access.

The objective is ensuring that autonomous agents consistently produce secure outcomes.

SATF helps organizations achieve:

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
- Expected Outcomes

---

## What Is a Secure Outcome?

A secure outcome is:

- The right action
- Performed by the right agent
- For the right objective
- Using the right authority
- Within approved boundaries
- With continuous validation
- With recoverable trust

SATF continuously evaluates trust throughout the agent lifecycle to ensure that task completion never overrides secure outcomes.

---

# SATF Outcome Model

SATF capabilities exist to achieve secure outcomes.

| SATF Capability | Primary Outcome Role |
|-----------------|----------------------|
| Agent Trust Fabric | Assess |
| Ring 1: Trust Establishment | Prevent |
| Ring 2: Trust Enforcement | Prevent + Enforce |
| Ring 3: Trust Validation | Detect + Validate |
| Governance, Telemetry & Assurance Control Plane | Adapt + Assure |
| Runtime & Response Plane | Contain + Recover + Re-establish |

---

## SATF Core Principle

The controls are not the goal.

**Secure outcomes are the goal.**

> SATF exists to ensure autonomous agents consistently produce safe, trusted, compliant, resilient, and expected outcomes, even when objectives evolve, context changes, authority is delegated, tools expand, threats emerge, and trust must be continuously reassessed.

<div style="display: grid; grid-template-columns: 1fr 1.3fr; gap: 20px; width: 100%; min-width: 0;">
<div style="min-width: 0; overflow: visible;">
  <p><b>Core Principle Pyramid (Objective over Control)</b> </p>

```mermaid

graph TD
    %% --- TOP LAYER: THE GOAL ---
    subgraph APEX["APEX OBJECTIVE"]
        SO["<b>SECURE OUTCOMES</b><br/>Safe • Trusted • Compliant • Resilient • Expected"]
    end

    %% --- MIDDLE LAYER: DYNAMIC ACTIONS ---
    subgraph ACTIONS["DYNAMIC ACTION ENGINE"]
        direction LR
        ACT1["<b>Assess</b><br/>(Trust Fabric)"]
        ACT2["<b>Prevent & Enforce</b><br/>(Ring 1 & Ring 2)"]
        ACT3["<b>Detect & Validate</b><br/>(Ring 3)"]
        ACT4["<b>Adapt & Assure</b><br/>(Control Plane)"]
        ACT5["<b>Contain & Recover</b><br/>(Runtime Plane)"]
    end

    %% --- BASE LAYER: FOUNDATIONAL ARCHITECTURE ---
    subgraph BASE["FOUNDATIONAL CAPABILITIES"]
        direction LR
        ATF["Agent Trust Fabric"]
        TR["Trust Rings (R1-R3)"]
        CP["Control Plane (R4 Overlay)"]
        RP["Runtime & Response Plane"]
    end

    %% RELATIONSHIPS (UPWARD FLOW)
    BASE ==>|Powers| ACTIONS
    ACTIONS ==>|Consistently Delivers| APEX

    %% STYLING
    classDef apex fill:#1b4332,stroke:#52b788,stroke-width:3px,color:#fff;
    classDef action fill:#2d6a4f,stroke:#74c69d,stroke-width:2px,color:#fff;
    classDef base fill:#081c15,stroke:#40916c,stroke-width:1px,color:#d8f3dc;

    class SO apex;
    class ACT1,ACT2,ACT3,ACT4,ACT5 action;
    class ATF,TR,CP,RP base;
```
</div>
<div style="min-width: 0; overflow: visible;">
  <p><b>Comprehensive SATF Outcome Engine Flow</b> </p>

```mermaid

flowchart TD
 
    %% INPUT
    REQ["<b>Agent Execution Request</b><br/>Goal, Tools & Task Scope"] --> FABRIC

    %% LAYER 1: TRUST FABRIC & RINGS
    subgraph CAPABILITIES["1. SATF Capability & Control Engine"]
        FABRIC["<b>Agent Trust Fabric</b><br/><i>[Assess]</i> Real-Time Trust Scoring"]
        
        subgraph RINGS["Trust Rings"]
            R1["<b>Ring 1: Establishment</b><br/><i>[Prevent]</i> Identity & Sandbox"]
            R2["<b>Ring 2: Enforcement</b><br/><i>[Enforce]</i> Contextual PDP/PEP"]
            R3["<b>Ring 3: Validation</b><br/><i>[Detect/Validate]</i> Rule of Two & Red Teaming"]
        end
    end

    %% LAYER 2: OVERLAY & RUNTIME
    subgraph CONTROLS["2. Control & Operational Execution Plane"]
        R4["<b>Governance, Telemetry & Assurance</b><br/><i>[Adapt + Assure]</i> Policy Feeds & Evidence"]
        RRP["<b>Runtime & Response Plane</b><br/><i>[Contain + Recover]</i> Isolation & Rollback"]
    end

    %% PIPELINE CONNECTORS
    FABRIC --> R1 --> R2 --> R3
    R4 -.->|Policy & Observability| CAPABILITIES
    R3 -->|Evaluation Signal| RRP

    %% DECISION GATE
    RRP --> DECISION{"Is Execution & Output Validated?"}

    %% DECISION PATHS
    DECISION -- Yes --> OUTCOME
    DECISION -- No / Drift Detected --> RECOVER["<b>Re-establish Trust / Containment</b><br/>Block, Revoke, Quarantine"]
    RECOVER -.->|Continuous Reassessment| FABRIC

    %% TARGET OBJECTIVE
    subgraph OUTCOME["3. Primary Objective: SECURE OUTCOME"]
        direction LR
        O1["<b>Safe</b>"]
        O2["<b>Trusted</b>"]
        O3["<b>Compliant</b>"]
        O4["<b>Resilient</b>"]
        O5["<b>Expected</b>"]
    end

    %% STYLING
    classDef req fill:#2b2d42,stroke:#8d99ae,color:#fff;
    classDef cap fill:#1a365d,stroke:#2b6cb0,color:#fff;
    classDef ctrl fill:#2c5282,stroke:#4299e1,color:#fff;
    classDef gate fill:#742a2a,stroke:#e53e3e,color:#fff;
    classDef outcome fill:#22543d,stroke:#38a169,stroke-width:2px,color:#fff;

    class REQ req;
    class FABRIC,R1,R2,R3 cap;
    class R4,RRP ctrl;
    class DECISION,RECOVER gate;
    class O1,O2,O3,O4,O5 outcome;

```
</div>
</div>
---

## Control Mapping Matrix

The Secure Agent Trust Framework (SATF) Control Mapping Matrix helps security architects, product security teams, platform engineers, governance teams, and auditors understand how SATF capabilities work together to prevent, detect, validate, contain, recover from, and ultimately re-establish trust following agent failures.

Rather than asking:

> Which security control should I deploy?

SATF asks:

> Which framework capabilities should work together to ensure secure outcomes when autonomous agents encounter risk, uncertainty, or compromise?

- [How to read this diagram](docs/11-satf-in-action/SATF-Control-Mapping-Matrix/satf-control-mapping-matrix-introduction.md)
![Control_Mapping](assets/diagrams/SATF_Control_Mapping_Diagram_v3.png)
---
## Framework structure

SATF Baseline 1.0 uses three coordinated views:

1. **Conceptual Trust Plane**
   - Core: Agent Trust Fabric
   - Ring 1: Trust Establishment
   - Ring 2: Trust Enforcement
   - Ring 3: Trust Validation

2. **Cross-Cutting Control Plane**
   - Governance
   - Telemetry
   - Assurance

3. **Runtime and Response Plane**
   - Runtime Agent Ecosystem
   - Response and Containment
   - Trusted Agent Outcomes

## Quick navigation

- [Why SATF](docs/00-overview/why-satf.md)
- [Trust Lifecycle](docs/00-overview/trust-lifecycle.md)
- [Framework Structure](docs/00-overview/framework-structure.md)
- [Agent Trust Fabric](docs/01-agent-trust-fabric/README.md)
- [Trust Establishment](docs/02-ring-1-trust-establishment/README.md)
- [Trust Enforcement](docs/03-ring-2-trust-enforcement/README.md)
- [Trust Validation](docs/04-ring-3-trust-validation/README.md)
- [Governance, Telemetry, and Assurance](docs/05-cross-cutting-control-plane/README.md)
- [Runtime and Response Plane](docs/06-runtime-response-plane/README.md)
- [Maturity Model](docs/07-maturity-model/README.md)
- [Alignment Mapping](docs/08-alignment-mapping/README.md)
- [Control Catalog](docs/09-control-catalog/README.md)
- [SATF In Action](docs/11-satf-in-action/README.md)
- [FAQ](docs/12-faq/README.md)
- [Pattern Library](docs/12-pattern-library/README.md)
- [Tech Reference](docs/13-technical-reference/README.md)
- [Appendices](docs/10-appendices/README.md)

## Baseline 1.0 status

This repository represents the public/community baseline version of SATF. Internal working versions have been normalized into **Baseline 1.0** for clarity.
