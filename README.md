# CareerOS Application Service

Track application drafts, approvals, submissions, statuses and audit history.

## Scope

- **Owns:** Application state machine and immutable audit references.
- **Inputs:** User-approved application commands and status updates.
- **Outputs:** Application lifecycle events.
- **Dependencies:** identity, job, resume, ATS and communication services.

## Safety baseline

This public repository must never contain secrets, real resumes, real applications or personal data. External communication and application submission always require explicit user approval.

## Documentation

See [docs/overview.md](docs/overview.md) and the central [CareerOS workspace](https://github.com/FievezRomain/careeros-workspace).

## Status

Architecture and security baseline. Functional implementation will be added incrementally with tests and versioned contracts.

## License

Apache-2.0.