# Evidence Sufficiency Pilot Standard v0.1

Status: **Draft for review**

## Purpose
Define the first audit-lobster pilot scope as `evidence_sufficiency` and specify the minimum rule for pass, review-incomplete, and blocker.

## Pilot scope
The first audit lobster pilot should use:
- `audit_scope: evidence_sufficiency`

## Minimum judgment model
### pass
Grant `pass` only when all three are true:
1. audit scope is clear
2. corresponding minimum evidence exists
3. no clear blocker is found

### review-incomplete
Grant `review-incomplete` when:
1. audit scope is clear
2. available information is insufficient to grant pass
3. no hard blocker is yet confirmed

### blocker
Return `blocked` when:
1. minimum evidence is missing
2. evidence is clearly insufficient for the declared audit scope
3. required stop-if-missing items are absent

## First-priority blocker class
The first audit lobster should prioritize:
- `missing evidence`

## Why this scope comes first
This scope is the best first pilot because it is:
- narrow
- relatively objective
- easier to evaluate than full closure legitimacy
- aligned with anti-self-certification hardening
