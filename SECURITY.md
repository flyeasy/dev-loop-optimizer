# Security Policy

## Supported version

Security fixes are applied to the latest revision on the default branch.

## Report a vulnerability

Use GitHub private vulnerability reporting when it is available for this repository. If it is unavailable, open a minimal issue asking for a private reporting channel.

Do not post exploit details, credentials, tokens, private repository content, personal data, device identifiers, or sensitive screenshots in a public issue.

Include only the minimum safe information needed to reproduce the behavior:

- affected revision;
- triggering task shape;
- expected safety boundary;
- observed behavior;
- sanitized reproduction steps.

## Security properties and limits

The published Skill is prompt-only and ships no executable scripts, dependencies, binaries, hooks, network calls, or credentials. Its safety rules cover current-scope reconciliation, non-authorizing issue discovery, untrusted repository artifacts, script inspection, read-only boundaries, evidence sanitization, resource fuses, retry limits, and verification truthfulness.

These controls reduce risk but cannot guarantee the behavior of every model, host, project script, external tool, or repository. Review the exact diff and the surrounding task authority before enabling side effects.
