# Deployment and Sales Minimum Hard Control Standard v0.1

## Purpose
Add minimum hard control gates for deployment and sales before production-like use.

# 1. Deployment minimum controls
## Required before deploy
- deploy authority named
- target environment named
- stop conditions defined
- rollback owner named
- pre-deploy checklist completed
- write-back target defined

## Required after deploy
- post-deploy smoke check
- deployment result record
- incident linkage if deploy fails or degrades service

## Weak patterns to reject
- deployment with no rollback owner
- deployment with no smoke verification
- deployment success declared from intent rather than observed state

# 2. Sales minimum controls
## Required before non-template commitment
- commitment authority named
- commitment category identified
- prohibited categories checked
- boundary language for delivery / SLA / scope applied
- formal write-back target defined

## Prohibited without Monarch approval
- guaranteed delivery promises outside validated capability
- SLA promises outside approved boundary
- pricing or scope commitments outside approved template

## Required after external non-template commitment
- formal write-back record
- owner for follow-through
- risk note if promise depends on unfinished delivery capability
