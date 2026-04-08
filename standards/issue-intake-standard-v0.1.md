# Issue Intake Standard v0.1

## Purpose
Standardize issue creation so AI agents can:
- decide whether a task should exist
- understand the task with minimal reading
- execute under clear boundaries
- leave usable records
- close with evidence

## Core rules
1. Issue titles should be in **Chinese** for fast human scanning.
2. Issue bodies may use **AI-native language** when it improves execution clarity.
3. Every issue should be optimized for **minimum necessary context**, not maximum verbosity.
4. If a task is not worth formal tracking, do not create the issue.

## Pre-issue filter: Musk 5-step adaptation
Before creating or accepting an issue, apply this filter:

### Step 1: Challenge the requirement
- Is this task actually necessary?
- Is the goal real, or is it inherited process noise?
- Can the requirement be simplified or deleted?

### Step 2: Delete unnecessary parts
- What can be removed before planning begins?
- Is there a smaller version that achieves most of the value?

### Step 3: Simplify and optimize
- Is this the simplest task definition that preserves value?
- Can scope, acceptance, or workflow be simplified?

### Step 4: Accelerate cycle time
- Can feedback, verification, or write-back happen sooner?
- Can the task be split to shorten time-to-learning?

### Step 5: Automate last
- Only automate after the task shape is proven useful
- Do not automate broken or unclear process

## Required fields
- Title (Chinese)
- Goal
- Boundary
- Non-goals
- Why now
- Expected output
- Risk level
- Operator owner
- Audit requirement
- Write-back target
- Closure expectation
- Minimal reading pack

## Title rule
Title format recommendation:
- `类型：任务意图简述`

Examples:
- `治理：建立 Issue 最小立项标准 v0.1`
- `运行：修复支付链路回写失败`
- `销售：梳理线索自动分发规则 v0.1`

## Body language rule
- Human-facing brief should stay short
- Execution detail can be AI-native and structured
- Prefer bullets, sections, and machine-diff-friendly text

## Minimal reading pack rule
Each issue should specify only the smallest required reading set.

Preferred pack:
- 1 governing standard
- 1 template
- 1 directly related prior issue or PR
- optional 1 runtime or evidence document

Avoid:
- full-library reading by default
- replaying all governance docs on every task

## Rejection rule
Reject issue creation or return for rewrite if:
- no clear goal
- no clear boundary
- no closure expectation
- no owner
- too much context with no minimal reading pack
- task fails the 5-step filter badly
