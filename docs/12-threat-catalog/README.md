# SATF Threat Catalog v1.0

The SATF Threat Catalog documents agent-specific threat patterns that can undermine Secure Outcomes in autonomous systems.

SATF Threat Catalog v1.0 contains:

```text
7 threat domains
31 agent-specific threats
```

## Core model

```text
Threat
   ↓
Boundary Violated
   ↓
SATF Controls
   ↓
Reference Architectures
   ↓
Evidence Artifacts
   ↓
Secure Outcomes
```

## Threat domains

1. Mission & Goal Threats
2. Delegation & Authority Threats
3. Memory & Context Boundary Threats
4. Tool & Action Threats
5. Identity & Credential Threats
6. Trust & Evidence Threats
7. Out-of-Bound Agent Threats

## Signature SATF concept

An **Out-of-Bound Agent** is an autonomous agent operating outside approved mission, authority, context, tool, identity, trust, evidence, or runtime boundaries.

## Visual maps

- [Threat Landscape Map](./threat-landscape.md)
- [Threat-to-Control Map](./threat-to-control-map.md)
- [Threat-to-Outcome Map](./threat-to-outcome-map.md)

## Important principle

```text
Identity establishes who an agent is.
Authorization determines what an agent may do.
Context defines when, why, and under what conditions an action remains trustworthy.
```
