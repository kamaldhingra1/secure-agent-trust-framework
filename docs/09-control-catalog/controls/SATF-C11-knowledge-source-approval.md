# SATF-C11: Knowledge Source Approval

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C11 |
| Control Name | Knowledge Source Approval |
| SATF Area | Ring 1 / Ring 2 |
| Outcome Role | Prevent + Enforce |
| Control Family | Trust Establishment / Trust Enforcement Controls |
| Status | Draft |

## Purpose

Ensure autonomous agents only use approved, governed, current, and context-appropriate knowledge sources during mission execution.

## Problem Addressed

Agents that rely on unapproved, stale, poisoned, incomplete, or unauthorized knowledge sources may produce unsafe, noncompliant, or unexpected outcomes. In RAG and knowledge-driven workflows, source quality and authorization directly affect mission trust.

## Control Statement

The organization should approve, classify, govern, and continuously validate knowledge sources used by autonomous agents.

## Implementation Guidance

- Maintain an inventory of approved knowledge sources for agent use.
- Classify sources by sensitivity, authority, freshness, ownership, and mission applicability.
- Define retrieval policies for regulated, confidential, public, and untrusted sources.
- Require approval before connecting new sources to an agent or retrieval system.
- Track source provenance, version, update time, and owner.
- Prevent agents from using untrusted or unapproved sources for high-impact decisions.
- Use contextual authorization to enforce source access at runtime.
- Monitor evidence freshness and trigger trust decay when source confidence declines.

## Evidence Artifacts

- Approved knowledge source inventory
- Source owner record
- Source classification record
- Retrieval policy
- Source approval record
- Source freshness report
- Retrieval trace
- PDP / PEP decision log

## Related SATF Scenarios

- Memory Poisoning
- Retrieval Poisoning
- Context Poisoning
- Goal Overreach
- Trust Decay

## Related Reference Architectures

- RA-02 RAG Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture
- TrustOps Implementation Pattern

## Related Controls

- SATF-C10 Memory Integrity
- SATF-C05 Contextual Authorization
- SATF-C06 Agent Risk Evaluation
- SATF-C14 Data Access Control

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Expected Outcomes
