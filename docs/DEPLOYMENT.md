# Deployment

Deployment documentation defines how Master Admin and Client Template installations should move safely from development to production.

## Deployment Principles

- Keep environments explicit.
- Keep secrets outside the repository.
- Make client clone setup repeatable.
- Prefer staged rollout for high-risk updates.
- Track versions for templates, packages, prompts, and employees.

## Environments

Expected environments may include:

- Local development
- Preview
- Staging
- Production
- Client production clone

## Master Admin Deployment

Master Admin deployment should prioritize security, internal access control, operational visibility, and update coordination.

## Client Template Deployment

Client Template deployment should prioritize repeatable onboarding, customer-specific configuration, data isolation, and smoke testing.

## Release Checklist

Before release:

- Confirm documentation is updated.
- Confirm secrets are configured outside GitHub code.
- Run relevant tests.
- Confirm migrations and rollback plan.
- Confirm package and version notes.
- Confirm support visibility.

## Related Documents

- `UPDATE_SYSTEM.md`
- `MULTI_TENANT.md`
- `SECURITY.md`
- `TESTING.md`
- `ONBOARDING.md`
