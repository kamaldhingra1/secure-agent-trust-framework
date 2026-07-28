# SATF-C14: Data Access Control

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C14 |
| Control Name | Data Access Control |
| SATF Area | Ring 2 |
| Outcome Role | Enforce |
| Control Family | Trust Enforcement Controls |
| Status | Draft |

## Purpose

Ensure autonomous agents access only the data required for the approved mission, under appropriate policy, context, sensitivity, and evidence conditions.

## Problem Addressed

Agents may access, combine, summarize, transform, export, or persist data. Excessive or poorly governed data access can lead to leakage, privacy risk, regulatory exposure, unsafe decisions, or unexpected outcomes.

## Control Statement

Agent data access should be governed by contextual authorization, data sensitivity, mission purpose, least agency, and continuous telemetry.

## Implementation Guidance

- Classify data sources by sensitivity, purpose, owner, residency, and regulatory requirements.
- Authorize access based on mission objective and current context.
- Enforce least agency for read, write, export, transform, and retention permissions.
- Require step-up approval for regulated, confidential, safety-critical, or customer-impacting data.
- Restrict data export and external transmission unless explicitly approved.
- Log data access, retrieval, transformation, and output generation.
- Reassess access when trust score changes, mission context changes, or policy is updated.

## Evidence Artifacts

- Data source inventory
- Data classification record
- Data access policy
- Data access log
- Data export log
- PDP / PEP decision log
- Step-up approval record
- Data retention record

## Related SATF Scenarios

- Unsafe External Action
- Memory Poisoning
- Prompt Injection to Tool Use
- Credential Misuse
- Trust Decay

## Related Reference Architectures

- RA-01 Single Agent Reference Architecture
- RA-02 RAG Agent Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C05 Contextual Authorization
- SATF-C09 Least Agency
- SATF-C11 Knowledge Source Approval
- SATF-C10 Memory Integrity

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Expected Outcomes
