# Project Constitution

This constitution defines the operating rules for AI Business OS Master Admin.

GitHub is the single source of truth for technical documentation, architecture, coding rules, agent instructions, and implementation decisions. If another tool contains conflicting information, GitHub wins until this repository is updated.

## Project Identity

AI Business OS is the foundation of a software company, not only a one-time application.

The first commercial product is AI Marketing Team, delivered through a two-application architecture:

- Master Admin: private control center for managing clients, templates, prompts, employees, packages, updates, support, and architecture decisions.
- Client Template: cloneable customer system for each client installation.

## Non-Negotiable Principles

- Revenue first, platform always.
- GitHub is the technical source of truth.
- Major architecture decisions must be documented before or alongside implementation.
- Do not break the two-app architecture.
- Keep the Client Template cloneable.
- Build reusable engines, modules, providers, and packages before one-off client features.
- Use customer language externally: employees, departments, training, approval, performance.
- Use technical language internally: agents, engines, modules, providers, registries.
- Human approval is the default for business-sensitive customer-facing actions.

## Company Operating Principles

The company should build for repeatability, not heroics. A feature is not mature until it can be explained, sold, onboarded, supported, measured, and improved.

The first product should be small enough to sell quickly and strong enough to become the foundation of the larger platform.

Every major system should answer:

- How does this help reach paying customers?
- How does this strengthen the long-term platform?
- Can this be reused across client installations?
- Is the customer experience simple?
- Is the internal complexity documented?

## Documentation Rules

Every important architectural decision must be recorded in one of these places:

- `docs/DECISIONS.md` for founder and architecture decisions.
- `docs/ARCHITECTURE.md` for system structure, boundaries, layers, and ownership.
- `docs/CODING_RULES.md` for implementation standards.
- `docs/CODEX_INSTRUCTIONS.md` for Codex work rules.
- `docs/LOVABLE_SYNC_RULES.md` for Lovable and GitHub synchronization.
- `docs/NEXT_STEPS.md` for active execution priorities.

Documentation must be extended, not replaced, unless the old content is explicitly obsolete and the replacement explains why.

## Architecture Authority

The two-application model is foundational:

- Master Admin is private, operational, and internal.
- Client Template is customer-facing, cloneable, and repeatable.

No feature should blur this boundary without a documented decision.

## Change Control

Before adding a major feature, changing architecture, introducing a new provider, or changing clone behavior, update the relevant documentation.

Every logical change should be committed separately with a clear message.

## Product Direction

The project should prioritize a sellable AI Marketing Team product while preserving the long-term AI Business OS platform.

Early work must make progress toward:

- Paying customers.
- Repeatable onboarding.
- Cloneable client deployments.
- Reusable internal platform components.
- Clear support and update workflows.

## Decision Quality Bar

A decision is ready when it states:

- The problem being solved.
- The decision made.
- The alternatives considered, when relevant.
- The expected impact on revenue, architecture, cloneability, safety, and support.
- The documents or code areas affected.

## Authority

This file has priority when project direction is unclear. More specific documentation may refine it, but must not contradict it without an explicit documented decision.

Related documents: `README.md`, `AGENTS.md`, `docs/DECISIONS.md`, `docs/ARCHITECTURE.md`, `docs/PRODUCT_RULES.md`.