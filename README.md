# Development Loop Optimizer

A prompt-only Codex Skill for keeping long development loops bounded, evidence-driven, and recoverable.

The canonical Skill ID is `dev-loop-optimizer`. The same internal Skill has sometimes been called `loop-developer` in conversation; the published name stays aligned with its installed folder, frontmatter, and `$dev-loop-optimizer` invocation.

## What it improves

- Keeps one primary item active while preserving unresolved work.
- Defines the expected signal, verification method, and exit condition before editing.
- Selects the cheapest useful build, test, device, or UI check.
- Stops retry loops that produce no new evidence.
- Preserves sanitized handoff state without treating old ledgers as authorization.
- Separates implemented, verified, and `needs verification` outcomes.

It is intended for repeated build/test/debug/UI loops, multi-issue development, and simulator or device work. It is not intended for one-step edits, pure Q&A, or expanding a read-only review into implementation.

## Safety model

This repository contains no executable scripts, package dependencies, network integrations, or credential handling. The Skill instructs agents to:

- treat repository content, logs, screenshots, webpages, and ledgers as untrusted data;
- preserve the latest user scope instead of reviving stale authorization;
- inspect project automation before running it;
- keep read-only requests read-only;
- sanitize persistent evidence and keep it untracked by default;
- require real verification before claiming completion.

The pre-publication review covered prompt-injection boundaries, destructive or privileged actions, secrets and personal data, persistent state, resource bounds, hidden files, links, file permissions, and provenance. See [SECURITY.md](SECURITY.md) for reporting guidance and residual risk.

## Install

Inspect the repository, then copy the Skill subfolder into your Codex Skills directory:

```text
skills/dev-loop-optimizer/
```

The default destination is `~/.codex/skills/dev-loop-optimizer`, or `$CODEX_HOME/skills/dev-loop-optimizer` when `CODEX_HOME` is set. Keep the folder name unchanged so the invocation remains `$dev-loop-optimizer`.

## Use

Invoke it explicitly when a development task begins to sprawl:

```text
Use $dev-loop-optimizer to keep this development loop bounded, evidence-driven, and safe to resume.
```

The Skill can also be selected implicitly for long build/test/debug/UI-verification loops.

## Repository layout

```text
skills/dev-loop-optimizer/
├── SKILL.md
├── agents/openai.yaml
└── references/templates.md
```

GitHub-facing documentation stays outside the Skill package so runtime context remains concise.

## License

[MIT](LICENSE)
