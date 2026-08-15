<!--
Copyright © 2026 CrypticNews LLC. All rights reserved.
This provenance header does not replace the repository's applicable license.
-->

# Canonical Convergence Review Checklist

## Repository integrity

- [ ] Repository is genuinely part of the Living System project corpus.
- [ ] External forks are labeled as external.
- [ ] Repository visibility is recorded.
- [ ] Default branch is recorded.
- [ ] Existing history is preserved.
- [ ] No destructive rewrite is required.

## Artifact provenance

- [ ] Every imported artifact has a source.
- [ ] Source commit/revision is recorded when available.
- [ ] Artifact type and sector are assigned.
- [ ] Duplicate artifacts are linked rather than silently duplicated.
- [ ] Generated artifacts are labeled.

## Security

- [ ] Secrets scanned before publication.
- [ ] API keys excluded.
- [ ] OAuth tokens excluded.
- [ ] Private keys excluded.
- [ ] Passwords/recovery codes excluded.
- [ ] Sensitive personal information excluded or redacted.
- [ ] Credentials are referenced by variable name or capability, never by value.

## Licensing

- [ ] Repository license inspected.
- [ ] External research licenses recorded.
- [ ] Generated documentation does not falsely claim third-party work as original.
- [ ] Copyright/provenance notices are consistent with the repository license.

## Architecture

- [ ] Module declares identity.
- [ ] Module declares capabilities.
- [ ] Module declares communication interface.
- [ ] Persistence behavior documented.
- [ ] Telemetry behavior documented.
- [ ] Governance/review boundary documented.
- [ ] Protocol contract exists before implementation is promoted.

## Runtime quality

- [ ] Build is reproducible.
- [ ] Tests exist for critical paths.
- [ ] Error handling is explicit.
- [ ] Watchdog/recovery behavior is bounded.
- [ ] No uncontrolled self-modification is enabled.
- [ ] Human release approval remains required.

## Public review quality

- [ ] README explains the project's purpose.
- [ ] Architecture diagram is current.
- [ ] Repository topology is documented.
- [ ] Installation path is documented.
- [ ] Security model is documented.
- [ ] Research references are reproducible.
- [ ] Changelog/release notes are maintained.
- [ ] Reviewers can distinguish canonical work from historical/prototype work.

## Convergence acceptance

A repository or artifact is accepted into the canonical convergence graph only when:

```text
Provenance ✓
Security ✓
License ✓
Architecture ✓
Tests ✓
Review ✓
```

Acceptance does not require every prototype to become production code. Historical artifacts remain valuable as lineage evidence.
