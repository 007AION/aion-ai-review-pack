# Multi-Project Routing Standard v0.1

## Purpose
Allow three-role AI organization to run multiple projects in parallel without context contamination.

## Routing rules
1. Each project has its own formal record lane.
2. Each task belongs to exactly one project lane.
3. Cross-project work must name a primary project owner.
4. Shared infrastructure tasks must declare all affected projects.

## Task selection rule
Before taking a task, Operator Core should ask:
- Is this the highest-value current task?
- Is this blocked by a more upstream task?
- Is this redundant with an existing issue?
- Does it survive the 5-step filter?

## Priority stack
Default priority order:
1. blockers on active main line
2. high-risk runtime or deployment work
3. high-leverage automation work
4. sales tasks directly tied to delivery reality
5. optimization and polish

## Anti-sprawl rule
Do not open too many issues at once.
Favor fewer, better-shaped issues over broad noisy intake.
