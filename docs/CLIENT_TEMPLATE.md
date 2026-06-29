# Client Template

Client Template is the cloneable customer application for AI Business OS.

Each customer installation should begin from the same template and then receive its own configuration, Business DNA, provider credentials, enabled packages, content, knowledge, approvals, analytics, and users.

## Responsibilities

Client Template owns the customer experience:

- Business DNA onboarding and editing.
- Knowledge base management.
- Customer-facing AI employees.
- Content creation and approval workflows.
- Landing page and campaign workflows.
- CRM Lite records.
- Customer analytics.
- Customer settings and provider credentials.

## Cloneability Rules

The template must not contain hard-coded client-specific data.

A new client clone should be created through a repeatable setup checklist:

1. Create installation.
2. Configure environment and credentials.
3. Load selected package.
4. Complete Business DNA onboarding.
5. Enable employees and workflows.
6. Confirm approval settings.
7. Run smoke tests.
8. Hand off to the customer.

## Customer Language

Customer-facing UI should use employees, departments, office, training, approval center, business profile, and performance.

Avoid exposing agents, prompt blocks, provider adapters, or implementation-specific terms.

## Data Ownership

Customer-specific data should live inside the client installation or customer-owned storage model.

Master Admin may reference metadata, health, package state, and support state, but should not casually duplicate customer data.

## Related Documents

- `MASTER_ADMIN.md`
- `BUSINESS_DNA.md`
- `AI_EMPLOYEES.md`
- `ONBOARDING.md`
- `MULTI_TENANT.md`
