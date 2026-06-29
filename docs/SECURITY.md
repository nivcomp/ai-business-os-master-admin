# Security

Security protects customer trust, company operations, provider credentials, and AI output safety.

## Core Rules

- Never commit secrets, API keys, credentials, tokens, private customer data, or local environment files.
- Keep customer data isolated by client.
- Require human approval by default for sensitive AI actions.
- Audit support access to customer systems.
- Use provider abstractions to limit credential sprawl.

## Sensitive Data

Sensitive data includes:

- Provider credentials.
- Customer Business DNA when private.
- Knowledge base records.
- CRM records.
- User account data.
- Billing data.
- Drafts and approved customer content.
- Analytics tied to a customer.

## Access Control

Master Admin should use explicit roles and permissions.

Support access should be limited, intentional, and auditable. Customer content should not be broadly visible in Master Admin without a documented support purpose.

## AI Safety

AI employees should not publish, send, bill, delete, or expose data without appropriate permissions and approval.

Prompt and tool changes that affect external actions should be reviewed.

## Incident Handling

Security incidents should be documented with timeline, impact, containment, root cause, customer communication needs, and prevention actions.

## Related Documents

- `MULTI_TENANT.md`
- `TOOLS.md`
- `PROVIDER_LAYER.md`
- `DEPLOYMENT.md`
- `SUPPORT.md`
