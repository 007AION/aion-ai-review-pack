# First Audit Pilot Selection Rule v0.1

Status: **Draft for review**

## Purpose
Choose the first issue type for the second lobster pilot so the audit loop is testable without exposing the system to unnecessary risk.

## Good first pilot issue characteristics
- low-risk
- governance or documentation related
- clear boundary
- visible evidence exists
- easy to tell accepted vs blocked
- does not require production deployment
- does not require external commitment

## Avoid for first pilot
- deployment execution
- sales commitment review
- auth / token changes
- payment or ledger logic
- destructive data work

## Recommended pilot types
- closure legitimacy check on a governance issue
- evidence sufficiency check on a documentation update issue
- boundary check on a low-risk standards change

## Goal
The first pilot should test the audit loop itself, not the most dangerous part of the civilization.
