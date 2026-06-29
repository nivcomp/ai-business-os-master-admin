# Decisions

## FD-001: Build a company, not only an app

The project should be treated as the foundation of a software company, not a one-time Lovable app.

## FD-002: First product is AI Marketing Team

The first commercial product will focus on marketing because it is easier to explain, easier to sell and can create revenue faster.

## FD-003: Sell employees, not agents

Customer-facing language should use employees, teams, departments, training, performance and approvals.

Internal technical language can use agents, engines, modules and providers.

## FD-004: Revenue first, platform always

Every early feature should help us get closer to paying customers while still strengthening the long-term platform.

## FD-005: GitHub is the technical source of truth

Google Drive may remain useful for business documents, but GitHub will hold the technical documentation, project brain, architecture and future code.

## FD-006: Two-app architecture

The project is divided into:

- Master Admin: private control system.
- Client Template: cloneable customer system.

## FD-007: Human approval by default

AI can prepare work, but business-sensitive customer-facing actions should require approval unless the user explicitly configures automation.

## FD-008: Documentation is part of the product foundation

The repository must be understandable by a new engineer or AI agent without prior conversation context.

Major concepts should have durable Markdown documentation and links to related documents.

## FD-009: Prefer domain documents over scattered notes

Documentation should be grouped by company, vision, architecture, AI, development, product, and business domains.

Prefer complete documents that explain ownership and decisions over many tiny notes.

## FD-010: Packages are the commercial delivery unit

The company should package modules, employees, prompts, settings, and workflows into sellable and installable offers.

The first package is AI Marketing Team.

## FD-011: Provider abstraction protects the platform

External services should be accessed through provider abstractions where practical so the platform can change vendors without rewriting product workflows.

## FD-012: Approval state is a core workflow concept

Approval is not only a UI feature. It is a business safety model for AI-generated work that affects brand, publishing, customer communication, billing, or external systems.

## FD-013: Support and analytics are platform requirements

Support visibility and analytics should be designed early because they affect trust, retention, pricing, onboarding, and product quality.

Related documents: `ARCHITECTURE.md`, `PRODUCT_RULES.md`, `AI_WORKFLOWS.md`, `SUPPORT.md`, `ANALYTICS.md`.
