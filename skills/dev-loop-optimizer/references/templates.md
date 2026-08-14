# Templates

Use only the minimum template required. Persist it only when project writes are authorized and repository conventions allow it. Use a task-specific, non-overwriting path and keep it untracked by default. Remove credentials, account data, personal information, device identifiers, raw environment values, and host-specific absolute paths; prefer sanitized excerpts and repository-relative evidence paths.

## Contents

- [Task Contract](#task-contract)
- [Iteration Summary](#iteration-summary)
- [Backlog Ledger](#backlog-ledger)
- [Completion Challenge](#completion-challenge)
- [Verification Note](#verification-note)
- [Context-Restart Handoff](#context-restart-handoff)
- [UI Verification](#ui-verification)
- [Retry Cutoff](#retry-cutoff)

## Task Contract

```markdown
# Task Contract

- Target:
- Current request and authority:
- Authorized side effects:
- Approval gates:
- Out of scope:
- Expected signal:
- Verification method:
- Exit condition:
```

## Iteration Summary

```markdown
# Iteration Summary

- Target:
- Files changed:
- Validation:
- Result:
- Backlog touched:
- Status changes:
- Remaining risk:
- Next step:
```

## Backlog Ledger

```markdown
# Work Ledger

- Active:
- Needs verification:
- Queued:
- Blocked:
- Cancelled:
- Done this round:

## Scope notes
- Current request:
- Item sources:
- Reprioritization reason:
- Side effects requiring fresh approval:
```

## Completion Challenge

```markdown
# Completion Challenge

- What evidence could still prove this unfinished?
- Which earlier user-reported items remain open or cancelled?
- Was the result verified on the real target path?
- Did the work stay within the current request?
- Should this be `done` or only `needs verification`?
```

## Verification Note

```markdown
# Verification Note

- Item:
- Expected result:
- Verification method:
- Sanitized repository-relative evidence path:
- Actual result:
- Remaining risk:
```

## Context-Restart Handoff

```markdown
# Context-Restart Handoff

- Latest user request to reconcile:
- Active item:
- Last verified result:
- Open or cancelled backlog:
- Sanitized evidence paths:
- Side effects requiring re-authorization:
- Next best read-only action:
```

## UI Verification

```markdown
# UI Check

- Target form factor:
- Screen or flow:
- Verified states:
- Layout, icon, or interaction issues:
- Sanitization performed:
- Remaining risk:
```

## Retry Cutoff

```markdown
# Retry Cutoff

- Problem:
- Attempts tried:
- New evidence gained:
- Why this path is stalled:
- Budget or approval gate reached:
- Best next branch:
```
