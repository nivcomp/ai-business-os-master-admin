# Contributing

This repository is the company knowledge base and future Master Admin codebase for AI Business OS.

Contributions should improve the repository as a source of truth for future engineers, AI agents, product work, and implementation.

## Before You Start

Read:

1. `PROJECT_CONSTITUTION.md`
2. `AGENTS.md`
3. `docs/00-START-HERE.md`
4. `docs/ARCHITECTURE.md`
5. `docs/CODING_RULES.md`
6. Any document related to the change.

## Contribution Principles

- Extend documentation instead of replacing it.
- Keep GitHub as the source of truth.
- Group related changes together.
- Document major decisions before or alongside implementation.
- Preserve the two-application architecture.
- Keep the Client Template cloneable.
- Prefer reusable platform capabilities over one-off features.

## Documentation Changes

Documentation should be professional Markdown with clear headings, decision context, related documents, and practical guidance for future engineers.

When adding a new document, link it from a related existing document or from `README.md` in a later documentation pass.

When changing architecture, update `docs/DECISIONS.md` if the change creates a new durable decision.

## Code Changes

Code changes should follow `docs/CODING_RULES.md`, `docs/SECURITY.md`, `docs/TESTING.md`, and `docs/DEPLOYMENT.md`.

Implementation should keep provider-specific logic behind provider boundaries and avoid leaking internal technical language into customer-facing UI.

## Commit Guidelines

Use clear commit messages in this style:

- `docs: add company foundation`
- `docs: add architecture documentation`
- `docs: add AI documentation`
- `docs: add product documentation`
- `docs: add business documentation`
- `feat: add approval workflow foundation`
- `fix: prevent hard-coded client settings`

Do not create one commit per file for documentation sprints. Group related documents by domain.

## Review Checklist

Before finalizing a change, confirm:

- The change supports revenue, platform strength, or operational clarity.
- Relevant documents are updated.
- Architecture boundaries are preserved.
- Cloneability is preserved.
- Human approval requirements are clear.
- No secrets or customer data are committed.
- The change can be understood without prior conversation context.

Related documents: `PROJECT_CONSTITUTION.md`, `AGENTS.md`, `docs/CODING_RULES.md`, `docs/GIT_WORKFLOW.md`.