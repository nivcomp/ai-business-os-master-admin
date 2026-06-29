# Agent Instructions

These instructions apply to all AI and human agents working in this repository.

## Source of Truth

GitHub is the single source of truth for technical documentation, architecture, coding rules, project instructions, and implementation decisions.

Before making important changes, read the relevant files in `docs/`, especially:

1. `docs/00-START-HERE.md`
2. `docs/PROJECT_CONTEXT.md`
3. `docs/VISION.md`
4. `docs/ROADMAP.md`
5. `docs/ARCHITECTURE.md`
6. `docs/DECISIONS.md`
7. `docs/CODING_RULES.md`
8. `docs/CODEX_INSTRUCTIONS.md`
9. `docs/LOVABLE_SYNC_RULES.md`
10. `docs/NEXT_STEPS.md`

## Required Context Before Work

For architecture work, also read `docs/MASTER_ADMIN.md`, `docs/CLIENT_TEMPLATE.md`, `docs/MODULE_SYSTEM.md`, `docs/PACKAGE_SYSTEM.md`, and `docs/UPDATE_SYSTEM.md`.

For AI work, read `docs/PROMPT_ARCHITECTURE.md`, `docs/AI_EMPLOYEES.md`, `docs/KNOWLEDGE_BASE.md`, `docs/MEMORY.md`, `docs/TOOLS.md`, and `docs/AI_WORKFLOWS.md`.

For product or business work, read `docs/PRODUCT_RULES.md`, `docs/FEATURE_ROADMAP.md`, `docs/PRICING.md`, `docs/ONBOARDING.md`, and `docs/SUPPORT.md`.

## Working Rules

- Do not replace existing documentation when extending it.
- Preserve the two-app architecture: Master Admin and Client Template.
- Keep the Client Template cloneable and free of hard-coded client-specific data.
- Document every important architectural decision.
- Prefer reusable modules, engines, providers, and registries.
- Use clear commit messages and commit logical groups separately.
- Do not introduce dependencies, providers, or workflows without documenting why.
- Favor revenue-supporting work that also strengthens the long-term platform.

## Language Rules

Customer-facing language should use:

- Employees
- Departments
- Office
- Training
- Approval Center
- Performance Review
- Business DNA

Internal technical language may use:

- Agents
- Engines
- Modules
- Providers
- Registries
- Packages
- Update Center

## Architecture Rules

New capabilities should clearly belong to one or more layers from `docs/ARCHITECTURE.md`:

1. Presentation Layer
2. Business Layer
3. AI Layer
4. Integration Layer
5. Data Layer
6. Infrastructure Layer

When a change crosses layers, document the boundary and ownership.

## Documentation Output Rules

Every document should be useful to a future engineer who has no previous conversation context.

Good documentation explains:

- What the system is.
- Why it exists.
- What owns it.
- What depends on it.
- What decisions are settled.
- What decisions remain open.

## Safety Rules

AI-generated work that may affect customers, publishing, billing, data, or brand reputation should require human approval by default.

Secrets, API keys, customer data, and provider credentials must not be committed to the repository.

## When Unsure

If instructions conflict, follow this order:

1. `PROJECT_CONSTITUTION.md`
2. `docs/DECISIONS.md`
3. `docs/ARCHITECTURE.md`
4. `docs/CODING_RULES.md`
5. Existing code patterns
6. The current task request

If the right path is still unclear, document the assumption before implementation.