# SATF Control Mapping Diagram v3

This version connects SATF capabilities to outcome roles directly in the heatmap header.

## What changed in v3

- Added a **Capability Outcome Role** row beneath the SATF capability headers.
- Removed the disconnected bottom outcome band from v2.
- Clarified how to read the visual:
  - Capability outcome roles explain what each SATF area contributes.
  - Heatmap letters explain how strongly each SATF area applies to each failure scenario.
- Preserved the improved color contrast from v2:
  - P = violet / primary control area
  - M = cyan / major supporting control
  - S = slate gray / supporting evidence control

## SATF Outcome Model

| SATF Capability | Outcome Role |
|---|---|
| Agent Trust Fabric | Assess |
| Ring 1: Trust Establishment | Prevent |
| Ring 2: Trust Enforcement | Prevent + Enforce |
| Ring 3: Trust Validation | Detect + Validate |
| Control Plane | Adapt + Assure |
| Runtime Plane | Contain + Recover + Re-establish |

## Suggested placement

Use this image at the top of `docs/11-satf-in-action/satf-control-mapping-matrix.md` and reference the SATF Outcome Model from the global README.
