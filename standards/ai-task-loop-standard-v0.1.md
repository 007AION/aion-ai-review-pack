# AI Task Loop Standard v0.1

## Purpose
Define the minimum AI-only loop from issue intake to closure with three roles:
- Monarch
- Operator Core
- Audit Core

## Target behavior
After issue creation, AI should be able to:
- discuss the approach
- shape the plan
- execute the task
- audit the result
- close the task
- preserve work history
- extract reusable lessons

Human intervention should be minimized.

## Loop
### 1. Intake
Issue is created with intake standard.

### 2. Operator discussion
Operator Core creates a short execution discussion note inside the issue or linked record:
- understanding of goal
- proposed path
- expected output
- known risks
- whether scope correction is needed

### 3. State assignment
Task gets one explicit state:
- queued
- acknowledged
- executing
- blocked
- review-ready
- closed

### 4. Execution
Operator Core performs the work and leaves:
- progress note or commit
- blocker note if needed
- evidence package when work is done

### 5. Audit
Audit Core checks:
- boundary fit
- evidence sufficiency
- remaining risk
- closure legitimacy

### 6. Closure
Task is closed only after closure package and audit decision are present.

### 7. Experience extraction
Operator Core or designated memory function writes:
- what worked
- what failed
- what should become reusable pattern

## Record rule
Every loop should preserve:
- plan trace
- execution trace
- blocker trace
- audit trace
- closure trace
- lesson trace
