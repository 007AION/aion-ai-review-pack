# Audit Lobster Minimal Closed-Loop Protocol v0.1

Status: **Draft for review**

## Purpose
Define the smallest workable protocol for introducing a second lobster as a pure audit agent inside AION's current three-role governance model.

## Goal
Do not start with a full audit civilization.
Start with a minimal audit lobster that can:
- receive audit task packets
- decide whether to accept or block
- leave a formal GitHub acknowledgement or blocker
- emit one short Discord fast-loop status
- return a minimal formal audit outcome

## Scope
This protocol is for the first minimal audit lobster only.
It is not yet the full long-term audit system.

## Minimum task packet
The first version requires only these 6 fields:
- `task_id`
- `target_role`
- `audit_scope`
- `write_back_target`
- `risk_level`
- `stop_if_missing`

### Example
```text
task_id: AUDIT-001
target_role: audit-core
audit_scope: closure_legitimacy
write_back_target: github:issue:12
risk_level: high
stop_if_missing:
- execution_trace
- evidence
- boundary
```

## GitHub acknowledgement format
### Accept
```text
[AUDIT-ACK]
task_id: AUDIT-001
scope: closure_legitimacy
status: accepted
```

### Block
```text
[AUDIT-BLOCKER]
task_id: AUDIT-001
missing: evidence
status: blocked
```

## Discord fast-loop status
Discord should retain only one short status for the minimal audit loop:
- accepted
- blocker

### Example
```text
[AUDIT] AUDIT-001 accepted
```

or

```text
[AUDIT] AUDIT-001 blocked: missing evidence
```

## Formal audit outcome states
The minimal audit lobster only needs these output states at first:
- `accepted`
- `blocked`
- `pass`
- `review-incomplete`

## Stop conditions
The audit lobster must stop and block when any of the following is true:
- no boundary
- no write-back target
- no minimum evidence
- risk is high but evidence is insufficient
- audit scope is unclear
- task packet is not directed to audit-core

## Must-have first abilities
The second lobster should first be able to:
1. decide whether to accept the task
2. decide whether evidence is minimally sufficient
3. return a formal minimal audit state

## Why this protocol comes first
This protocol is the best first audit-agent adoption step because it is:
- small
- testable
- governance-compatible
- easy to observe
- easier to harden later than a prematurely large audit system
