# SATF-C12: Supply Chain Integrity

## Control Summary

| Field | Value |
|---|---|
| Control ID | SATF-C12 |
| Control Name | Supply Chain Integrity |
| SATF Area | Ring 1 / Control Plane |
| Outcome Role | Prevent + Assure |
| Control Family | Trust Establishment / Control Plane Controls |
| Status | Draft |

## Purpose

Ensure the components used by autonomous agents, including models, prompts, tools, plugins, MCP servers, datasets, containers, dependencies, and knowledge pipelines, are approved, traceable, validated, and monitored for risk.

## Problem Addressed

Agent trust depends on more than the model. A compromised tool, poisoned dataset, malicious plugin, vulnerable container, unsafe prompt package, or untrusted dependency can compromise the mission even if the agent itself appears legitimate.

## Control Statement

The organization should maintain supply chain integrity for agent components and dependencies used across the autonomous mission lifecycle.

## Implementation Guidance

- Maintain an inventory of agent components and dependencies.
- Track provenance for models, prompts, tools, plugins, datasets, retrieval pipelines, and runtime images.
- Require validation before introducing new components into agent workflows.
- Use signed artifacts, version pinning, dependency scanning, and SBOMs where applicable.
- Monitor tool and dependency risk over time.
- Reassess mission trust when dependencies change or vulnerability intelligence emerges.
- Integrate supply chain findings into trust scoring and policy governance.

## Evidence Artifacts

- Agent component inventory
- Model provenance record
- Tool approval record
- SBOM / dependency inventory
- Vulnerability scan results
- Signed artifact record
- Change approval record
- Assurance review record

## Related SATF Scenarios

- Tool Compromise
- Prompt Injection to Tool Use
- Software Supply Chain Compromise
- Trust Decay
- Unsafe External Action

## Related Reference Architectures

- RA-00 Core SATF Reference Architecture
- RA-04 Coding Agent Reference Architecture
- RA-07 Regulated Healthcare Agent Reference Architecture

## Related Controls

- SATF-C01 Agent Identity
- SATF-C05 Contextual Authorization
- SATF-C06 Agent Risk Evaluation
- SATF-C13 Tool Access Control

## Expected Outcomes

- Safe Outcomes
- Trusted Outcomes
- Compliant Outcomes
- Resilient Outcomes
