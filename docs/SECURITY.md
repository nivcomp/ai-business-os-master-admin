# Security

Security protects customer trust, company operations, provider credentials, and AI output safety.

## Core Rules

- Never commit secrets, API keys, credentials, tokens, private customer data, or local environment files.
- Keep customer data isolated by client.
- Require human approval by default for sensitive AI actions.
- Audit support access to customer systems.
- Use provider abstractions to limit credential sprawl.

## Secrets And API Keys

Secrets must not be stored in source code, documentation examples, screenshots, or local files committed to GitHub.

Secrets include:

- AI provider keys.
- Email provider keys.
- WhatsApp provider keys.
- Social publishing tokens.
- Database credentials.
- Storage credentials.
- Payment keys.
- Webhook secrets.

Secrets should be stored in the deployment platform or secret manager appropriate to the environment.

## Provider Credentials

Provider credentials may be platform-owned, client-owned, or hybrid.

Each provider credential should have:

- Owner.
- Scope.
- Environment.
- Rotation process.
- Revocation process.
- Last verification date.
- Access policy.

Client-owned provider credentials should remain scoped to the correct client installation.

## Client Isolation

Client data must be isolated across Business DNA, Knowledge Base, CRM Lite, content history, assets, analytics, provider credentials, users, and package state.

No prompt, tool, log, analytics event, or support workflow should mix data between clients.

## Support Access

Support access should be intentional, permissioned, time-limited where practical, and auditable.

Support users should see the minimum data required to solve the issue.

Master Admin should track who accessed a client, when access started, when it ended, and why access was needed.

## Logs

Logs should help diagnose issues without exposing sensitive data.

Logs should avoid storing raw secrets, full provider tokens, unnecessary customer content, or private CRM data.

When sensitive content must be logged for debugging, access should be restricted and retention should be limited.

## Audit Trail

The system should record audit events for:

- Login and access changes.
- Support access grants.
- Provider credential updates.
- Business DNA changes.
- Prompt package updates.
- Package installation and updates.
- Approval state changes.
- Publishing or external-send actions.

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

## Human Approval

AI employees should not publish, send, bill, delete, overwrite, or expose data without appropriate permissions and approval.

Human approval is required by default for work that affects:

- Public brand communication.
- Customer messages.
- Publishing.
- Billing.
- Data deletion.
- Provider credential changes.
- External systems.

## Incident Handling

Security incidents should be documented with timeline, impact, containment, root cause, customer communication needs, and prevention actions.

## Related Documents

- `MULTI_TENANT.md`
- `TOOLS.md`
- `PROVIDER_LAYER.md`
- `DEPLOYMENT.md`
- `SUPPORT.md`
- `MASTER_ADMIN.md`
- `CLIENT_TEMPLATE.md`
