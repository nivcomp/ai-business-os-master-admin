# Multi-Tenant and Client Isolation

AI Business OS must support multiple client installations safely and repeatably.

The near-term model may use separate Client Template clones per customer. The long-term platform may evolve toward stronger centralized multi-tenant services where appropriate.

## Core Rule

Client data must be isolated. One customer's data, prompts, credentials, analytics, and Business DNA must not leak into another customer's system.

## Isolation Areas

Isolation must cover:

- Business DNA
- Knowledge base content
- Uploaded assets
- CRM records
- Campaign and content history
- Provider credentials
- Users and permissions
- Analytics events
- Billing and package state

## Master Admin Visibility

Master Admin may view operational metadata and support diagnostics. Access to customer content should be permissioned, auditable, and limited to legitimate support needs.

## Tenant Identity

Every client installation should have a stable client identifier used for package state, updates, analytics, support, and diagnostics.

## Future Decision

A future documented decision should choose the long-term tenancy model: separate deployments, shared multi-tenant service, or hybrid architecture.

## Related Documents

- `MASTER_ADMIN.md`
- `CLIENT_TEMPLATE.md`
- `SECURITY.md`
- `ANALYTICS.md`
- `DEPLOYMENT.md`
