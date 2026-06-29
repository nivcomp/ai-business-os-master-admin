# Next Steps

This file tracks the next practical actions for AI Business OS Master Admin.

## Current Priority

Build toward the first revenue product: AI Marketing Team.

The goal is not to build the whole long-term platform first. The goal is to create a sellable, cloneable, approval-centered marketing product while laying reusable platform foundations.

## Immediate Steps

1. Confirm repository structure for Master Admin.
2. Confirm or create the separate Client Template repository.
3. Define the minimum AI Marketing Team workflow.
4. Define Business DNA fields required for the first customer.
5. Define the first AI employees and their responsibilities.
6. Define Approval Center states and user actions.
7. Define provider choices and provider abstraction needs.
8. Define the clone setup checklist for a new customer.
9. Document any new architecture decision in `docs/DECISIONS.md`.

## Sprint 1 Documentation Completion

Documentation Sprint 1 is complete when every requested company, vision, architecture, AI, development, product, and business document exists and references related documents.

After Sprint 1, the repository should be understandable by a new engineer without prior conversation.

## Minimum AI Marketing Team Scope

The first revenue product should include:

- Business DNA setup.
- Knowledge base foundation.
- AI Marketing Manager.
- AI Copywriter.
- Content creation workflow.
- Approval Center.
- Landing page workflow.
- CRM Lite foundation.
- Basic analytics.
- Repeatable client clone setup.

## Decisions To Document Next

The next architectural decisions should cover:

- Where client-specific configuration lives.
- How Business DNA is stored and versioned.
- How prompts and employees are packaged.
- How Master Admin publishes updates to Client Template clones.
- Which provider abstractions are needed first.
- Which actions require human approval by default.

## First Build Milestone

A successful first build milestone should let a demo customer:

- Complete Business DNA onboarding.
- Use at least one AI employee to produce marketing content.
- Review and approve output before use.
- Store the approved result.
- See the workflow inside a simple business-friendly interface.

## Engineering Preparation

Before implementation starts, define:

- App shell and navigation structure.
- Data model for Business DNA.
- Approval state machine.
- Prompt configuration format.
- Provider abstraction interface.
- Minimal analytics events.
- Deployment and environment plan.

## Keep In Mind

- Revenue first, platform always.
- Do not weaken cloneability.
- Do not expose technical complexity to customers.
- Document important architecture decisions as they happen.
- Keep GitHub updated after Lovable or external tool changes.

## Related Documents

- `ROADMAP.md`
- `FEATURE_ROADMAP.md`
- `BUSINESS_DNA.md`
- `AI_EMPLOYEES.md`
- `ONBOARDING.md`
