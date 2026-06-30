# MVP Build Plan

This document defines the first practical build plan for AI Business OS and AI Marketing Team.

The goal is to build a sellable demo and foundation, not the entire long-term platform.

## MVP Goal

Create a working AI Marketing Team flow that proves:

- A customer can complete Business DNA.
- AI employees can use that profile.
- A Marketing Manager can plan a simple campaign idea.
- A Copywriter can create a marketing draft.
- The customer can review and approve the output.
- The approved output is stored and measured.
- Master Admin can see the client, package, employee, and health state.

## MVP Product

The first package is AI Marketing Team Starter.

Included employees:

- Marketing Manager.
- Copywriter.

Included modules:

- Business DNA.
- Knowledge Base foundation.
- Approval Center.
- Content Workflow.
- Basic Analytics.
- Client Registry in Master Admin.
- Prompt Package Registry in Master Admin.

## Master Admin MVP Screens

1. Dashboard.
2. Clients.
3. Client Detail.
4. Packages.
5. Prompt Packages.
6. AI Employees.
7. Provider Registry placeholder.
8. Client Health.
9. Support Access placeholder.
10. Update Center placeholder.

## Client Template MVP Screens

1. Office Dashboard.
2. Business DNA Onboarding.
3. Employees.
4. Marketing Manager.
5. Copywriter.
6. Content Workflow.
7. Approval Center.
8. Knowledge Base.
9. Basic Analytics.
10. Settings and Provider Keys.

## First Demo Flow

1. Open Client Template demo.
2. Complete Business DNA for a sample business.
3. Open Marketing Manager.
4. Generate one campaign idea.
5. Send task to Copywriter.
6. Copywriter generates social post draft.
7. Draft appears in Approval Center.
8. User approves or requests changes.
9. Approved content is saved.
10. Analytics records first approved output.
11. Master Admin shows client health updated.

## Data Models To Draft First

- Client.
- Package.
- Employee Template.
- Prompt Package.
- Business DNA.
- Content Draft.
- Approval Item.
- Provider Adapter.
- Analytics Event.
- Support Access Grant.

## Build Order

### Phase 1: Static Product Shell

- Master Admin app shell.
- Client Template app shell.
- Navigation and placeholder screens.
- Seed demo data.

### Phase 2: Business DNA And Employees

- Business DNA form and schema.
- Employee catalog data model.
- Marketing Manager and Copywriter screens.
- Prompt package data structure.

### Phase 3: First Workflow

- Create campaign idea.
- Create copy draft.
- Send to Approval Center.
- Approve or request changes.
- Store final output.

### Phase 4: Provider Readiness

- Define provider interfaces.
- Add text provider adapter first.
- Add placeholder image and video provider adapters.
- Add provider key settings model.

### Phase 5: Demo And Sales Readiness

- Add sample business.
- Add first demo script.
- Add pricing package notes.
- Add analytics summary.

## What Not To Build Yet

Do not build yet:

- Full automation autopilot.
- Full employee marketplace.
- Full CRM.
- Full publishing to every channel.
- Full video generation pipeline.
- Enterprise permissions.
- Complex multi-tenant infrastructure.

Build the smallest version that proves the sellable loop.

## Success Criteria

MVP is successful when a prospect can understand and believe:

- This is an AI marketing team.
- The system understands their business.
- It creates useful marketing work.
- They stay in control through approval.
- More employees can be added later.
- The company can package and support this repeatedly.

## Related Documents

- `PROJECT_STATE.md`
- `NEXT_STEPS.md`
- `EMPLOYEE_CATALOG.md`
- `MARKETING_AUTOMATION_ENGINE.md`
- `API_PROVIDER_STRATEGY.md`
- `AGENT_TO_EMPLOYEE_MODEL.md`
- `CLIENT_TEMPLATE.md`
- `MASTER_ADMIN.md`
