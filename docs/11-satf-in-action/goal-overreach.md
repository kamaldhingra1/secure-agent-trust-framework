# What If an Agent Overreaches Its Goal?

## Problem

A legitimate goal produces unauthorized or unsafe actions.

Example:

```text
Goal: Reduce cloud costs
Unsafe behavior: delete backups, disable monitoring, terminate production workloads
```

## SATF Coverage

### Agent Trust Fabric

- Goal evaluation
- Context evaluation
- Dynamic risk scoring

### Ring 2: Trust Enforcement

- Objective boundary checks
- Success constraints
- Forbidden path controls
- Step-up review

### Ring 3: Trust Validation

- Goal drift detection
- Reward-hacking detection

### Control Plane

- Adaptive trust policies
- Policy tightening

## SATF Principle

```text
Goal Approved != Every Action Approved
```
