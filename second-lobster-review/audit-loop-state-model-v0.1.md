# Audit Loop State Model v0.1

Status: **Draft for review**

## Purpose
Define the minimum state machine for the first 007 -> second-lobster audit loop.

## States
1. `created`
2. `dispatched`
3. `audit-accepted`
4. `audit-blocked`
5. `review-incomplete`
6. `pass`

## State meanings
### created
Formal issue and audit intent exist, but no audit packet has been sent yet.

### dispatched
007 has emitted a valid audit packet to the audit lobster.

### audit-accepted
Audit lobster has acknowledged the audit task.

### audit-blocked
Audit lobster cannot continue because required inputs or conditions are missing.

### review-incomplete
Audit lobster reviewed but cannot grant pass yet.

### pass
Audit lobster considers the requested audit scope sufficiently satisfied.

## Transition rules
- `created` -> `dispatched` only when minimum audit packet exists
- `dispatched` -> `audit-accepted` only when GitHub audit acknowledgement exists
- `dispatched` -> `audit-blocked` when stop conditions are triggered
- `audit-accepted` -> `review-incomplete` when review proceeds but closure conditions remain unsatisfied
- `audit-accepted` -> `pass` when the audit scope is satisfied

## Rule
A state change should be observable either in GitHub formal record or in the minimal Discord fast status layer.
