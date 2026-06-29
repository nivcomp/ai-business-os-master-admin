# Lovable Sync Rules

These rules define how Lovable work should stay aligned with GitHub.

## Source of Truth

GitHub is the single source of truth for technical documentation, architecture, coding rules, implementation decisions, and project instructions.

Lovable may be used for building and iterating on application screens, but Lovable is not the final authority for architecture or project memory.

## Before Lovable Changes

Before making meaningful Lovable changes, review:

- `PROJECT_CONSTITUTION.md`
- `AGENTS.md`
- `docs/ARCHITECTURE.md`
- `docs/CODING_RULES.md`
- `docs/DECISIONS.md`
- `docs/NEXT_STEPS.md`

## After Lovable Changes

After meaningful Lovable changes, update GitHub with:

- The implementation change, if code is exported or synced.
- Any new architectural decision.
- Any changed feature behavior.
- Any changed product scope.
- Any dependency, provider, or data model change.

## What Must Be Documented

Document changes that affect:

- Master Admin vs Client Template boundaries.
- Client cloneability.
- Business DNA structure.
- AI employee behavior.
- Prompt or agent configuration.
- Approval workflows.
- Integrations and provider choices.
- Data models and storage.
- Package or update logic.

## Sync Direction

GitHub documentation should guide Lovable implementation.

If Lovable produces behavior that conflicts with GitHub documentation, either adjust the Lovable implementation or update GitHub documentation with a clear decision.

## Naming Consistency

Lovable UI should use customer language:

- Employees
- Departments
- Office
- Training
- Approval Center
- Performance
- Business DNA

Internal implementation may use technical language:

- Agents
- Engines
- Modules
- Providers
- Registries
- Packages

## Cloneability Rule

Do not create Lovable features that depend on one specific client, hard-coded client data, or manually edited values that cannot be repeated for new customer clones.

## Commit Rule

Lovable-related sync changes should be committed clearly, for example:

- `docs: add lovable sync rules`
- `feat: add approval center screen`
- `fix: remove hard-coded client settings`
