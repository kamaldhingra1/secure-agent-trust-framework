# Context Boundary

## Definition

A **Context Boundary** defines what information an agent may see, inherit, retain, transfer, trust, and act upon during an autonomous mission.

## Why context boundaries matter

An agent may be correctly identified, authenticated, and authorized, yet still become unsafe if it operates on inappropriate, poisoned, stale, inherited, cross-tenant, or unapproved context.

## SATF principle

```text
Identity establishes who an agent is.
Authorization determines what an agent may do.
Context defines when, why, and under what conditions an action remains trustworthy.
```

## Related threat

- SATF-T13 Context Boundary Violation

## Primary controls

- C05 Contextual Authorization
- C10 Memory Integrity
- C11 Knowledge Source Approval
- C14 Data Access Control
- C20 Evidence Validation
