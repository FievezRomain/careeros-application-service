# CareerOS Application Service â€” service overview

## Responsibility

Track application drafts, approvals, submissions, statuses and audit history.

## Data ownership

Application state machine and immutable audit references.

## Interfaces

- Inputs: User-approved application commands and status updates.
- Outputs: Application lifecycle events.
- Dependencies: identity, job, resume, ATS and communication services.

## Contract rules

- APIs and events are versioned.
- Consumers must be idempotent where retries are possible.
- Correlation identifiers are propagated without logging sensitive payloads.
- Authorization and ownership are checked at the service boundary.

## Non-goals

This service does not absorb responsibilities owned by another CareerOS service. Cross-service workflows are coordinated through explicit contracts rather than shared databases.

## Security and privacy

Persist the minimum data required, record provenance, define retention, redact logs and use synthetic examples in this public repository.