# SATF Reference Architectures

This section provides implementation-oriented reference architectures for the Secure Agent Trust Framework.

The reference architectures show where SATF capabilities live, how trust decisions flow, how telemetry and validation evidence are used, and how secure outcomes are achieved.

## Architecture queue

| ID | Architecture | Status | Purpose |
|---|---|---|---|
| RA-00 | Core SATF Reference Architecture | Drafted | Canonical SATF architecture all other patterns inherit from |
| RA-01 | Single Agent Reference Architecture | Drafted | Smallest deployable SATF implementation |
| RA-02 | RAG Agent Reference Architecture | Planned | Knowledge, retrieval, memory, and context security |
| RA-03 | Multi-Agent Reference Architecture | Planned | Delegation provenance, agent-to-agent trust, trust decay |
| RA-04 | Coding Agent Reference Architecture | Planned | Source control, CI/CD, software supply chain |
| RA-05 | Autonomous Security Agent | Planned | Detection, investigation, response, approval gates |
| RA-06 | Agent Marketplace / Registry | Planned | Third-party agent trust, certification, reputation |
| RA-07 | Regulated Healthcare Agent | Planned | Quality systems, risk management, regulatory evidence |
| RA-08 | Manufacturing / OT Agent | Planned | OT safety, digital twins, operational constraints |
| RA-09 | Agent Trust Fabric Architecture | Planned | Trust graph, identity graph, delegation graph, trust propagation |
| RA-10 | Enterprise SATF Architecture | Planned | Multi-domain enterprise trust operations |

## Diagram assets

Diagram source and rendered images live under:

```text
assets/diagrams/reference-architectures/
```

Each architecture should include:

- Markdown explanation
- Mermaid `.mmd` source
- SVG render
- PNG render
