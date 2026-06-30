# Client Template Data Contract

This document defines the minimal data contract for the first Client Template build.

The goal is to support Copywriter v0.1 while keeping the app ready for Master Admin control.

## Core Models

### Client

- `id`
- `name`
- `environment`
- `templateId`
- `templateVersion`
- `installedPackageId`
- `installedPackageVersion`
- `createdAt`

### BusinessDNA

- `id`
- `clientId`
- `version`
- `businessName`
- `services`
- `targetAudience`
- `brandVoice`
- `primaryOffer`
- `primaryCTA`
- `languages`
- `restrictions`
- `marketingGoals`
- `updatedAt`

### Employee

- `id`
- `clientId`
- `employeeKey`
- `name`
- `department`
- `version`
- `status`
- `promptPackageVersion`

### ContentRequest

- `id`
- `clientId`
- `employeeId`
- `contentType`
- `userRequest`
- `status`
- `createdAt`

### ContentDraft

- `id`
- `requestId`
- `clientId`
- `employeeId`
- `title`
- `body`
- `cta`
- `channel`
- `tone`
- `businessDNAVersion`
- `promptPackageVersion`
- `createdAt`

### ApprovalItem

- `id`
- `clientId`
- `draftId`
- `status`
- `reviewNotes`
- `approvedAt`
- `createdAt`

### SavedContent

- `id`
- `clientId`
- `approvalItemId`
- `title`
- `body`
- `channel`
- `createdAt`

### ActivityEvent

- `id`
- `clientId`
- `eventType`
- `entityType`
- `entityId`
- `metadata`
- `createdAt`

### ClientHealth

- `clientId`
- `businessDNAStatus`
- `enabledEmployees`
- `lastActivityAt`
- `draftsCreated`
- `approvalPendingCount`
- `approvedContentCount`
- `healthStatus`

## Related Documents

- `CONTROL_PLANE_READY_MVP.md`
- `CLIENT_ADMIN_SYNC_CONTRACT.md`
- `COPYWRITER_V0_SPEC.md`
- `BUSINESS_DNA.md`
- `CLIENT_TEMPLATE.md`
