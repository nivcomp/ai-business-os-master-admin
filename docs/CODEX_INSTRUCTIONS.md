# Codex Instructions

These instructions apply when Codex works on this repository.

## First Step

Before making changes, read:

1. `PROJECT_CONSTITUTION.md`
2. `AGENTS.md`
3. `docs/00-START-HERE.md`
4. All relevant files under `docs/`

GitHub is the single source of truth. Do not rely on memory or external planning documents when repository documentation exists.

## Documentation Rule

Do not replace existing documentation unless explicitly asked. Extend it.

Every important architectural decision must be documented in the same change or in a prior documentation change.

## Work Style

- Keep changes focused.
- Commit logical groups separately.
- Use clear commit messages.
- Preserve existing project language and direction.
- Avoid broad refactors unless they are required for the task.
- Prefer small, revenue-supporting work that strengthens the platform.

## Architecture Guardrails

Codex must preserve:

- Master Admin as the private control center.
- Client Template as a cloneable customer application.
- Human approval by default for sensitive AI output.
- Provider abstraction where external services are involved.
- Clear separation between customer-facing language and internal technical language.

## Documentation Updates Required

Update documentation when changing app boundaries, data ownership, provider strategy, AI employee behavior, prompt behavior, approval behavior, package flow, update flow, clone behavior, or revenue-critical product scope.

## Commit Discipline

Each logical group should have its own commit.

Examples:

- Governance documentation.
- Architecture and coding rules.
- AI documentation.
- Product documentation.
- Business documentation.
- Bug fix.

## Verification

Codex should verify changes where possible. Documentation sprints should verify that all requested documents exist in the final GitHub tree.

Implementation work should run relevant tests or explain why tests were not run.

## Safety

Never commit secrets, API keys, credentials, private customer data, or local environment files.

When a requested change conflicts with `PROJECT_CONSTITUTION.md`, `docs/DECISIONS.md`, or `docs/ARCHITECTURE.md`, Codex should stop and document the conflict before proceeding.

Related documents: `AGENTS.md`, `CODING_RULES.md`, `GIT_WORKFLOW.md`, `LOVABLE_SYNC_RULES.md`.