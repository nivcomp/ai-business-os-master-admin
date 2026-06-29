# Architecture Overview

## Core Principle

The platform is built around a two-application architecture.

- Master Admin: internal control center.
- Client Template: cloneable customer application.

## Layers

1. Presentation Layer (UI)
2. Business Layer
3. AI Layer
4. Integration Layer
5. Data Layer
6. Infrastructure Layer

## Shared Concepts

- Business DNA
- Prompt Engine
- Employee Engine
- Knowledge Engine
- Package System
- Update Center
- Provider Layer

All new components should be reusable across client installations.

## Application Boundaries

### Master Admin

Master Admin is the private control center. It owns internal management workflows, client oversight, package/version management, prompt and employee governance, support access, update publishing, and operational visibility.

Master Admin must not become a customer-facing product surface. Customer-facing experience belongs in the Client Template.

### Client Template

Client Template is the cloneable customer application. It owns the customer's Business DNA, knowledge base, enabled employees, approvals, content workflow, CRM Lite, analytics, and customer-specific provider settings.

Client Template must remain cloneable. No feature should depend on hard-coded client data, one-off credentials, or assumptions that prevent repeatable customer setup.

## Layer Responsibilities

### Presentation Layer

Owns user-facing screens, navigation, forms, dashboards, approvals, and human review flows.

Customer-facing surfaces should use business language: employees, departments, training, approval, office, and performance.

### Business Layer

Owns product workflows, rules, permissions, approval states, package eligibility, onboarding flow, and revenue-facing product behavior.

### AI Layer

Owns employees, agents, prompt composition, model interaction, memory rules, AI output quality, and safety controls.

AI-generated work that can affect customers, publishing, brand, billing, or external communication requires human approval by default.

### Integration Layer

Owns external services such as AI providers, email, WhatsApp, social publishing, analytics, CRM, storage, and payment services.

Integrations should go through provider abstractions where possible so the platform does not depend permanently on one vendor.

### Data Layer

Owns schemas, data access, tenant separation, Business DNA, knowledge records, content assets, approvals, metrics, and package state.

Client-specific data must stay isolated per client installation.

### Infrastructure Layer

Owns deployment, environments, secrets, logging, monitoring, backups, versioning, and update delivery.

Secrets and credentials must never be committed to the repository.

## Architectural Decision Rules

Every important architectural decision must be documented in `docs/DECISIONS.md` or this file.

Document a decision when it affects:

- Master Admin vs Client Template boundaries.
- Cloneability.
- Data ownership or tenant separation.
- Provider choices or provider abstraction.
- AI employee behavior, permissions, or approval rules.
- Package, update, or deployment flow.
- Revenue-critical product scope.

## Core Architecture Documents

- `MASTER_ADMIN.md` defines the private control center.
- `CLIENT_TEMPLATE.md` defines the cloneable customer system.
- `MODULE_SYSTEM.md` defines installable product capability units.
- `PACKAGE_SYSTEM.md` defines bundles of modules, employees, prompts, and settings.
- `BUSINESS_DNA.md` defines the structured business identity model.
- `AI_EMPLOYEES.md` defines the customer-facing employee model.
- `PROVIDER_LAYER.md` defines external service abstraction.
- `UPDATE_SYSTEM.md` defines controlled distribution to client clones.
- `MULTI_TENANT.md` defines isolation and tenancy rules.

## Reuse Rules

Prefer reusable engines and modules over one-off screens or client-specific features.

A reusable component should declare:

- What layer owns it.
- Whether it belongs to Master Admin, Client Template, or both.
- What data it reads or writes.
- What provider dependencies it has.
- What human approval step is required, if any.

## Current Architecture Direction

The near-term architecture should support the first revenue product, AI Marketing Team, while preserving the long-term AI Business OS platform.

Priority architecture capabilities:

- Business DNA setup and editing.
- Knowledge ingestion and retrieval.
- AI employee configuration.
- Approval Center.
- Content creation workflow.
- Landing page workflow.
- CRM Lite.
- Basic analytics.
- Package and update foundation.
