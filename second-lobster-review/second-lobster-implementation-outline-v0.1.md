# Second Lobster Implementation Outline v0.1

Status: **Draft for review**

## Purpose
Describe the minimum implementation path for creating the second lobster as a pure audit agent under the audit-lobster minimal closed-loop protocol.

## Current design assumption
- First lobster (007) acts as controlling / execution civilization
- Second lobster acts as pure audit-core lobster
- GitHub is the formal record center
- Discord is the fast status layer

## Minimum implementation steps
### Step 1: Create isolated audit workspace
Create an isolated folder for the second lobster with:
- identity file
- role charter
- protocol reference
- allowed scope

### Step 2: Define formal packet shape
007 must be able to generate the minimal audit packet with:
- task_id
- target_role
- audit_scope
- write_back_target
- risk_level
- stop_if_missing

### Step 3: Define GitHub response patterns
The second lobster should support at least:
- `[AUDIT-ACK]`
- `[AUDIT-BLOCKER]`
- final minimal state: `pass` / `blocked` / `review-incomplete`

### Step 4: Define Discord fast status pattern
Only emit one short audit fast-loop state:
- accepted
- blocker

### Step 5: Select first pilot issue type
Start with low-risk governance or documentation audit work.
Do not begin with deployment or sales.

## Pilot success criteria
The first pilot is successful if:
1. 007 dispatches a valid audit packet
2. second lobster accepts or blocks correctly
3. GitHub receives formal audit acknowledgement
4. Discord receives one short audit state
5. no human needs to manually reinterpret the result

## Current blocker note
The remaining gap is no longer governance design alone. The next gap is implementation path and runtime communication capability for the second lobster.
