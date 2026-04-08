# High-Risk Category × Required Evidence Matrix v0.1

## Purpose
Bind high-risk task categories to minimum mandatory evidence classes, so closure legitimacy depends on category-sensitive proof rather than generic operator narrative.

## Core rule
For high-risk work, closure is valid only when the task's category-specific evidence floor is satisfied.

## Matrix
### 1. Production deployment
Required evidence:
- smoke or probe result
- deployment log **or** observable environment state evidence

### 2. Payment / credits / ledger logic
Required evidence:
- test or validation result tied to changed logic
- observable post-change state check or rollback validation note

### 3. Credentials / tokens / auth changes
Required evidence:
- formal change record
- observed post-change validation result

### 4. Database migration or destructive data operation
Required evidence:
- migration / operation record
- post-change validation or integrity check
- rollback or restoration readiness note

### 5. External commitments affecting delivery / SLA / scope
Required evidence:
- formal write-back record
- capability validation link **or** explicit dependent-risk note

### 6. Policy or constitutional rule change
Required evidence:
- formal proposal/change record
- audit trace
- approval or adoption record

### 7. Multi-project-impacting shared change
Required evidence:
- formal change record
- one observable post-change verification artifact

### 8. Routing / automation / workflow rule changes affecting multiple tasks or approval paths
Required evidence:
- formal change record
- one execution-path validation artifact
- one write-back path verification artifact

## Escalation rule
Audit Core may require an additional evidence class when:
- rollback cost is high
- cross-project blast radius is high
- external commitments depend on the outcome
- production impact is difficult to observe directly

## Weak closure prohibition
No high-risk category may close on operator summary alone, even if the summary is structured and detailed.
