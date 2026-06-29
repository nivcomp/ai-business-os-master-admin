# Tools

Tools are controlled capabilities that AI employees may use to complete work.

A tool can read data, transform content, call a provider, create a draft, analyze performance, or prepare an action for approval.

## Tool Categories

Possible tool categories include:

- Content generation.
- Image generation.
- Landing page creation.
- Knowledge retrieval.
- CRM lookup.
- Analytics lookup.
- Email draft preparation.
- WhatsApp draft preparation.
- Social post preparation.
- Publishing actions.

## Tool Permission Model

Tools should be permissioned by employee, workflow, customer, and risk level.

High-risk tools should prepare work for approval rather than execute automatically by default.

## Tool Contract

Each tool should define:

- Purpose.
- Inputs.
- Outputs.
- Required permissions.
- Provider dependencies.
- Failure behavior.
- Logging requirements.
- Approval requirements.

## Safety

Any tool that can publish, send, charge, delete, overwrite, or expose customer data should require explicit permission and audit logging.

## Related Documents

- `AI_EMPLOYEES.md`
- `PROVIDER_LAYER.md`
- `AI_WORKFLOWS.md`
- `SECURITY.md`
- `CODING_RULES.md`
