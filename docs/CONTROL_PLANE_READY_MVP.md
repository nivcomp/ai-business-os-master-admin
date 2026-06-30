# Control Plane Ready MVP

The first working product should be small, but it must be built with the future control plane in mind.

The goal is to launch the first real employee, Copywriter v0.1, inside the Client Template while preparing the data shape that lets Master Admin manage hundreds of future client clones.

## Principle

Do not build a huge platform first.

Do build the first client app as if it will later be registered, monitored, updated, and supported by Master Admin.

## What This Means

Every Client Template clone should have:

- `clientId`
- `templateId`
- `templateVersion`
- `installedPackageId`
- `installedPackageVersion`
- `promptPackageVersion`
- `enabledEmployees`
- `businessDNA`
- `approvalItems`
- `activityEvents`
- `clientHealth`

The first UI can still be simple, but the data should not be a dead-end demo.

## First Real Employee

The first real employee is Copywriter v0.1.

Copywriter v0.1 must:

- Read Business DNA.
- Generate marketing copy.
- Produce multiple draft options.
- Send selected draft to Approval Center.
- Save approved output.
- Record Activity Events.
- Contribute to Client Health.

## Minimal Master Admin Relationship

At MVP stage, Master Admin does not need full update automation.

It does need to understand:

- Which client exists.
- Which template version the client runs.
- Which package version is installed.
- Whether Business DNA is complete.
- Whether Copywriter has been used.
- Whether content has been approved.
- Whether the client has health risks.

## Not In MVP

Do not build yet:

- Full multi-tenant infrastructure.
- Full billing.
- Full employee marketplace.
- Automatic update rollout.
- Full provider marketplace.
- Full media generation stack.

## Related Documents

- `CLIENT_ADMIN_SYNC_CONTRACT.md`
- `CLIENT_TEMPLATE_DATA_CONTRACT.md`
- `COPYWRITER_V0_SPEC.md`
- `TEMPLATE_VERSIONING_MODEL.md`
- `MVP_BUILD_PLAN.md`
