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

## FD-014: Customer-owned telephony by default

Voice and telephony providers such as Twilio, SIP providers, PBX systems, or future call providers should be treated as client-owned or client-isolated provider accounts by default.

For the first voice products, the preferred model is:

- The client owns the telephony account, phone number, billing, and provider relationship; or
- The platform uses an isolated provider subaccount per client when central management is required.

AI Business OS owns orchestration, workflow logic, provider abstraction, Voice Receptionist Employee behavior, call logs, CRM Lite records, and support visibility.

AI Business OS should not casually pool all clients through one shared telephony account unless there is a documented architecture and business decision explaining why.

The application should store only provider connection references, client ownership metadata, phone numbers or extensions, connection status, and provider policy data.

Actual provider secrets must not be committed to GitHub or stored directly in normal application tables.

This decision protects:

- Billing separation.
- Client data isolation.
- Easier client offboarding.
- Reduced misuse risk across clients.
- Cleaner support boundaries.
- Provider replacement through adapters.
- Client Template cloneability.

Customer-facing language:

- "Connect your phone system"
- "Connect your Voice Receptionist"
- "Your business phone provider"

Internal technical language:

- Telephony provider adapter.
- Voice provider reference.
- Client-owned provider account.
- Client-isolated provider subaccount.

This decision belongs to the future Voice Layer and Voice Receptionist Employee architecture, but it affects provider, billing, support, security, and multi-tenant design now.

Copywriter v0.1 remains the current MVP. Voice features must not be implemented until a future voice build phase is explicitly approved.

Related documents: `PROVIDER_LAYER.md`, `SECURITY.md`, `MULTI_TENANT.md`, `CLIENT_TEMPLATE.md`, `MASTER_ADMIN.md`, future `VOICE_LAYER.md`.
