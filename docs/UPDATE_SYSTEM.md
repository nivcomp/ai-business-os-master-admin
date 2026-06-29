# Update System

The Update System defines how Master Admin publishes improvements to Client Template installations.

It is critical because the company must support multiple clients without manually rebuilding each one from scratch.

## Responsibilities

The Update System should manage:

- Template versions.
- Package versions.
- Module updates.
- Prompt and employee updates.
- Migration notes.
- Rollout status.
- Rollback guidance.
- Client compatibility checks.

## Ownership

Master Admin owns update publishing, rollout policy, and visibility.

Client Template owns installed version state, local configuration, and execution of safe updates.

## Update Types

- Documentation update
- Prompt update
- Employee behavior update
- Module update
- Package update
- Security update
- Data migration
- Provider configuration update

## Safety Rules

Updates that can change customer-facing output quality, publishing behavior, data structure, or provider cost should be documented and reviewable.

High-risk updates should support staged rollout.

## Related Documents

- `PACKAGE_SYSTEM.md`
- `MODULE_SYSTEM.md`
- `CLIENT_TEMPLATE.md`
- `DEPLOYMENT.md`
- `SECURITY.md`
