# Second Lobster First Pilot Success Criteria v0.1

Status: **Draft for review**

## Purpose
Define what counts as success for the first real 007 -> second-lobster audit pilot.

## The pilot is successful if all of the following are true
1. 007 creates a valid audit packet
2. the second lobster correctly returns either `[AUDIT-ACK]` or `[AUDIT-BLOCKER]`
3. GitHub contains the formal audit record
4. Discord contains one short audit status
5. the result can be understood without human reinterpretation
6. the audit lobster uses `evidence_sufficiency` as scope
7. the first blocker priority behaves correctly on `missing evidence`

## The pilot is not yet successful if
- audit scope drifts into broad legal or philosophical closure judgment
- Discord becomes the main record store
- humans must manually explain what the audit result meant
- the second lobster silently performs execution instead of audit
