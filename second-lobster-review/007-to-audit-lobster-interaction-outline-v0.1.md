# 007 to Audit Lobster Interaction Outline v0.1

Status: **Draft for review**

## Purpose
Describe the minimum interaction pattern between 007 and the second lobster in the first audit pilot.

## Flow
1. 007 identifies a formal GitHub issue as audit target.
2. 007 creates the minimal audit packet.
3. 007 dispatches the packet to the audit lobster.
4. Audit lobster checks whether it should accept or block.
5. Audit lobster writes `[AUDIT-ACK]` or `[AUDIT-BLOCKER]` to GitHub.
6. A short Discord status is emitted.
7. Audit lobster later writes `pass` or `review-incomplete`.

## Boundary
The second lobster should not silently become an implementation agent during this first pilot.

## Success test
The interaction is successful if both agents can complete the loop without requiring the Monarch to reinterpret the result manually.
