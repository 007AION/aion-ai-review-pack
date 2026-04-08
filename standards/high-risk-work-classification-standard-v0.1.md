# High-Risk Work Classification Standard v0.1

## Purpose
Define which tasks count as high-risk in the three-role AI-only model, so stronger control gates apply consistently.

## High-risk by default
The following categories are high-risk by default:
- production deployment
- payment, credits, or ledger logic
- credentials, tokens, secrets, or auth changes
- database migration or destructive data operation
- external commitments affecting delivery, SLA, price, or scope
- policy or constitutional rule change
- changes that can materially impact multiple projects at once

## Medium-risk examples
- internal workflow standard updates
- non-production deployment rehearsal
- reporting automation touching shared records

## Low-risk examples
- formatting
- document cleanup
- non-authoritative summary generation
- private draft preparation

## Escalation rule
If uncertainty exists, classify upward, not downward.
