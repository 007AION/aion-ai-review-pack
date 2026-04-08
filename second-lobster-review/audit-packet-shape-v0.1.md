# Audit Packet Shape v0.1

Status: **Draft for review**

## Purpose
Standardize the smallest audit task packet 007 can send to the second lobster.

## Required fields
- `task_id`
- `target_role`
- `audit_scope`
- `write_back_target`
- `risk_level`
- `stop_if_missing`

## Field meanings
### task_id
Unique audit task identifier.

### target_role
Should be `audit-core` for the second lobster.

### audit_scope
The specific audit question, for example:
- `closure_legitimacy`
- `evidence_sufficiency`
- `boundary_check`

### write_back_target
The GitHub issue or comment target for acknowledgement and result.

### risk_level
- low
- medium
- high

### stop_if_missing
List of missing items that should force block instead of continuation.

## Example
```yaml
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
