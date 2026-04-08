# Anti-Self-Certification Hardening Standard v0.1

## Purpose
Reduce hidden self-certification risk inside the three-role model, especially where Operator Core internal duty compression makes closure appear independent while still relying on operator-curated evidence.

## Core law
No high-risk or non-trivial task should be considered formally closed when its legitimacy depends only on operator-prepared interpretation.

## 1. Internal duty lanes inside Operator Core
Without adding a fourth top-level role, Operator Core should distinguish the following internal duty lanes:
- build / implementation
- runtime / ops
- deployment
- sales-support
- knowledge upkeep

This is a control distinction, not yet a top-level organizational split.

## 2. High-risk closure gate
For high-risk work, closure requires all of the following:
1. explicit owner
2. explicit boundary and non-goals
3. formal write-back target
4. execution trace
5. audit trace
6. at least one independent evidence source
7. remaining risk statement

If any of the above is missing, the task may be marked blocked or review-incomplete, but not fully closed.

## 3. Independent evidence rule
For high-risk work, operator-self-curated summary alone is insufficient.

At least one independent evidence source is required, such as:
- runtime logs
- deployment logs
- CI or test status
- environment probe or smoke result
- external system state check

## 4. Audit raw-evidence right
Audit Core has the right to request and inspect raw evidence, not only operator-compressed summaries.

## 5. Lesson extraction rule
A task cannot be considered fully closed unless one of the following exists:
- lesson extraction record
- explicit `lesson deferred` record with reason

## 6. Prohibited weak closure patterns
- operator says “done” with no independent evidence
- operator-prepared summary is treated as sufficient proof in high-risk work
- no audit trace but task marked closed
- no boundary / non-goals but execution proceeded anyway
