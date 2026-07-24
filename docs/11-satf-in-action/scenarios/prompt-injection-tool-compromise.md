# What If Prompt Injection Reaches a Tool?

## Problem

Untrusted content causes an agent to invoke a tool or action in an unsafe way.

Example flow:

```text
Malicious document -> Prompt injection -> Tool invocation -> Sensitive action
```

## SATF Coverage

### Ring 2: Trust Enforcement

- Contextual authorization
- Tool governance
- Risk-based enforcement
- Step-up review
- Fail-closed enforcement

### Ring 3: Trust Validation

- Threat validation
- Adversarial testing
- Behavioral monitoring

### Runtime and Response Plane

- Containment
- Tool disablement
- Trust re-establishment
