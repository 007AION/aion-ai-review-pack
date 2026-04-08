# Independent Evidence Minimum Standard v0.1

## Purpose
Define the smallest independent evidence set required so high-risk closure does not rely only on operator-curated claims.

## Mandatory evidence classes for high-risk closure
At least **one** independent evidence source is mandatory. Prefer two when feasible.

Recommended evidence classes:
1. runtime log evidence
2. deployment log evidence
3. CI / test status
4. smoke or probe result
5. external system state check

## Selection rule
Choose evidence that is:
- generated outside the operator's narrative summary
- reproducible or observable
- linked to the actual target state

## Weak evidence patterns
The following are insufficient by themselves:
- operator summary only
- operator assertion with no linked artifact
- screenshot with no traceable context

## Audit rule
Audit Core may require a second evidence class when:
- the task is production-facing
- external commitments depend on the result
- rollback difficulty is high
