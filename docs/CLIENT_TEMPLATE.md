# Client Template

Client Template is the cloneable customer application for AI Business OS.

Each customer installation should begin from the same template and then receive its own configuration, Business DNA, provider credentials, enabled packages, content, knowledge, approvals, analytics, and users.

## Responsibilities

Client Template owns the customer experience:

- Business DNA onboarding and editing.
- Knowledge Base management.
- Customer-facing AI Employees.
- CRM Lite.
- Approval Center.
- Content workflow.
- Landing page and campaign workflows.
- Customer analytics.
- Customer provider keys and settings.

## Cloneable App Model

The Client Template should be a repeatable application that can be cloned for a new customer without engineering changes.

A clone receives configuration through environment variables, package selection, Business DNA, provider credentials, and customer settings.

The template itself should not include one-off customer content, hard-coded credentials, or manually embedded business rules.

## Core Customer Modules

### Business DNA

The structured client business profile used by AI employees, prompts, analytics, and onboarding.

### Knowledge Base

A customer-owned repository of brand, service, product, FAQ, campaign, and policy information.

### AI Employees

Customer-facing AI workers such as Marketing Manager, Copywriter, SEO Manager, Designer, Campaign Manager, and Analytics Manager.

### CRM Lite

A lightweight customer relationship layer for leads, contacts, simple pipeline state, and marketing follow-up context.

### Approval Center

The review surface for drafts, changes requested, approvals, published items, rejections, and archives.

### Content Workflow

The path from customer request to AI draft, review, approval, storage, publishing, or export.

### Analytics

Customer-facing and internal signals for onboarding, usage, approvals, publishing, performance, and value.

### Provider Keys

Customer-specific credentials for AI, email, WhatsApp, social publishing, analytics, storage, or other external services.

## Cloneability Rules

The template must not contain hard-coded client-specific data.

A new client clone should be created through a repeatable setup checklist:

1. Create installation.
2. Configure environment and credentials.
3. Load selected package.
4. Complete Business DNA onboarding.
5. Enable employees and workflows.
6. Confirm approval settings.
7. Run smoke tests.
8. Hand off to the customer.

## Customer Language

Customer-facing UI should use employees, departments, office, training, approval center, business profile, and performance.

Avoid exposing agents, prompt blocks, provider adapters, or implementation-specific terms.

## Data Ownership

Customer-specific data should live inside the client installation or customer-owned storage model.

Master Admin may reference metadata, health, package state, and support state, but should not casually duplicate customer data.

## First Build Screens

The first Client Template build should prioritize:

- Business DNA onboarding.
- Dashboard or office home.
- Employees list.
- Employee detail or task screen.
- Knowledge Base.
- Approval Center.
- Content workflow.
- CRM Lite foundation.
- Analytics summary.
- Settings for provider keys and business profile.

## Related Documents

- `MASTER_ADMIN.md`
- `BUSINESS_DNA.md`
- `AI_EMPLOYEES.md`
- `KNOWLEDGE_BASE.md`
- `ONBOARDING.md`
- `MULTI_TENANT.md`
- `SECURITY.md`
