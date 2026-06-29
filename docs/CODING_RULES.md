# Coding Rules

These rules guide implementation in AI Business OS Master Admin and related repositories.

## Core Rules

- Preserve the two-app architecture: Master Admin and Client Template.
- Keep the Client Template cloneable.
- Prefer reusable modules, engines, providers, and registries over one-off code.
- Do not hard-code client-specific data, secrets, API keys, or provider credentials.
- Document important architecture decisions before or alongside implementation.
- Keep GitHub documentation aligned with code behavior.

## Repository Source of Truth

GitHub is the technical source of truth. If implementation and documentation conflict, either update the documentation or document why the implementation is intentionally different.

Relevant documentation should be read before major implementation work:

- `PROJECT_CONSTITUTION.md`
- `AGENTS.md`
- `docs/ARCHITECTURE.md`
- `docs/DECISIONS.md`
- `docs/PRODUCT_RULES.md`
- `docs/PROJECT_CONTEXT.md`

## Code Organization

Code should be organized around product boundaries and reusable capabilities.

Prefer explicit ownership for:

- UI surfaces.
- Business workflows.
- AI employee and prompt logic.
- Integrations and provider adapters.
- Data access and schema rules.
- Infrastructure and deployment behavior.

Avoid mixing provider-specific logic directly into UI or business workflow code.

## Naming Rules

Customer-facing names should follow product language:

- Employee
- Department
- Training
- Approval
- Performance
- Business DNA

Internal technical names may use:

- Agent
- Engine
- Module
- Provider
- Registry
- Package

Do not expose internal technical names to customers unless the surface is explicitly internal.

## Provider Rules

External providers should be accessed through a provider layer when practical.

A provider integration should define:

- Purpose.
- Required credentials.
- Failure behavior.
- Cost or rate-limit concerns.
- Replacement path if the provider changes.

## AI Rules

AI behavior should be explicit, reviewable, and safe.

AI-generated customer-facing work should pass through approval flows unless the user has explicitly configured automation.

Prompt, employee, and agent changes that affect output quality or customer trust should be documented.

## Data Rules

Client data must be isolated per client installation.

Business DNA, knowledge, approvals, campaign data, CRM records, analytics, and package state should have clear ownership.

Avoid storing derived AI output without enough context to audit how it was produced.

## Commit Rules

Commit logical groups separately with clear messages.

Good commit message examples:

- `docs: add project governance instructions`
- `docs: extend architecture and coding rules`
- `feat: add approval workflow foundation`
- `fix: prevent client template hard-coded settings`

## Implementation Checklist

Before merging important work, confirm:

- The change fits the architecture layers.
- Master Admin and Client Template boundaries are preserved.
- Cloneability is not weakened.
- Human approval requirements are clear.
- Relevant documentation is updated.
- Secrets and client-specific values are not committed.
