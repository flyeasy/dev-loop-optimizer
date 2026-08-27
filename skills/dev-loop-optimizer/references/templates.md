# Templates

Use only the minimum template needed. Persist it only when project writes are authorized and repository conventions allow it. Use a task-specific, non-overwriting path and keep it untracked by default. Remove credentials, account data, personal information, device identifiers, raw environment values, and host-specific absolute paths; prefer sanitized excerpts and repository-relative evidence paths.

## Goal Lock

```markdown
# Goal Lock

- Requested outcome:
- Acceptance signal:
- Allowed surface:
- Authorized side effects:
- Approval gates:
- Out of scope:
- Verification lane and gates:
- Resource budget:
- Stop line:
```

## Iteration Delta

```markdown
# Iteration Delta

- Hypothesis:
- Coherent batch:
- Files or surfaces changed:
- Invalidated gate:
- Validation result:
- User-visible delta:
- Status: done | needs verification | blocked | failed
```

## Bounded Work Ledger

```markdown
# Bounded Work Ledger

- Active now and authority source:
- User-selected next:
- Needs verification:
- Decision pool requiring user selection:
- Blocked:
- Cancelled:
- Done this round:

## Scope lock
- Latest request:
- Allowed surface:
- Stop line:
- Side effects requiring fresh authority:
```

Do not promote a candidate merely because `active now` is complete.

## Decision Candidate

```markdown
# Decision Candidate — User Selection Required

- Observed behavior:
- Reproduction or evidence:
- User impact:
- Product-direction impact:
- Confidence:
- Affected journey:
- Reversibility or lock-in risk:
- Decision urgency or deadline:
- Estimated effort and risk:
- Recommendation:
- Why it is not completion-critical:
- No implementation performed:
```

## Acceptance Probe

```markdown
# Acceptance Probe

- Locked user journey and target:
- Primary task result:
- One interruption, empty/error, or recovery path checked:
- State truthfulness and feedback:
- Layout or interaction evidence:
- Completion-critical result:
- Up to three new non-blocking candidates added to the decision pool:
- Probe stop line reached:
```

## Resource Checkpoint

```markdown
# Resource Checkpoint

- Locked outcome:
- Elapsed time or tool-call proxy:
- User-visible delta so far:
- Hypotheses attempted:
- New evidence gained:
- Why the current pattern is no longer efficient:
- Narrower or alternative branch:
- Work stopped pending replanning or user decision:
```

## Context-Restart Handoff

```markdown
# Context-Restart Handoff

- Latest user request:
- Goal lock and stop line:
- Current status:
- Last verified delta:
- Remaining completion-critical work:
- Deduplicated decision pool requiring user selection:
- Sanitized evidence paths:
- Side effects requiring fresh authority:
- Safest next read-only action:
```

## Read-only Completion Challenge

```markdown
# Completion Challenge

- Does the requested acceptance path pass?
- Did an in-scope user requirement disappear?
- Is each remaining issue completion-critical, a decision gate before lock-in, or only a decision candidate?
- Is the evidence current and from the required target?
- Did the work remain inside the goal lock and resource budget?
- Final status and stop reason:
```
