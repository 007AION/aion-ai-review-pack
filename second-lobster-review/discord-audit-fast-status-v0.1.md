# Discord Audit Fast Status v0.1

Status: **Draft for review**

## Purpose
Define the smallest Discord status pattern for the audit lobster so Discord remains a fast coordination layer, not a record dump.

## Allowed statuses
- accepted
- blocker

## Examples
```text
[AUDIT] AUDIT-001 accepted
```

```text
[AUDIT] AUDIT-001 blocked: missing evidence
```

## Rule
If more detail is needed, put it in GitHub and only summarize the state in Discord.
