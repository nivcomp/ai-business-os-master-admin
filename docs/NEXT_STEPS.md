# Next Steps

This file tracks the next practical actions for AI Business OS Master Admin.

## Current Priority

Move from documentation foundation to the first build phase for AI Marketing Team.

The next build phase should create enough working product structure to prove the Master Admin and Client Template model without overbuilding the full platform.

## Sprint 2 Documentation Status

Sprint 2 deepened:

- `PROJECT_STATE.md`
- `BUSINESS_DNA.md`
- `PROMPT_ARCHITECTURE.md`
- `MASTER_ADMIN.md`
- `CLIENT_TEMPLATE.md`
- `SECURITY.md`

This gives the next build phase clearer requirements for current status, client profiles, prompt packages, Master Admin controls, cloneable client app scope, and security boundaries.

## Next Build Phase Task List

### 1. Repository And App Structure

- Confirm whether this repository will contain the Master Admin app code or documentation first with code added later.
- Confirm whether `ai-business-os-client-template` exists.
- If the Client Template repository does not exist, create it with matching documentation references.
- Define the basic folder structure for Master Admin implementation.

### 2. Master Admin Shell

- Build the Master Admin app shell.
- Add navigation for Dashboard, Clients, Templates, Packages, Prompt Packages, AI Employees, Update Center, Support, and Settings.
- Create placeholder screens that match `MASTER_ADMIN.md`.
- Keep the UI internal, operational, and dense enough for repeated admin work.

### 3. Client Registry

- Define the client record model.
- Track client name, status, package, version, environment, health, support state, and last activity.
- Build Clients list and Client detail placeholders.

### 4. Business DNA Schema

- Convert `BUSINESS_DNA.md` into an implementation schema.
- Start with required fields: business name, services or products, target audience, brand voice, primary offer, primary CTA, languages, restrictions, and marketing goals.
- Add validation rules and version metadata.

### 5. Prompt Package Format

- Define Global Prompt, Client Prompt, and Task Prompt structure.
- Define Prompt Blocks.
- Define Prompt Package metadata.
- Add version, tests, approval status, and rollout status.

### 6. AI Employee Registry

- Define employee template structure.
- Start with Marketing Manager and Copywriter.
- Map employees to prompt packages, tools, approval rules, and workflows.

### 7. Client Template Scope

- Define first Client Template screens: Business DNA onboarding, Office dashboard, Employees, Knowledge Base, Approval Center, Content Workflow, CRM Lite, Analytics, Settings.
- Confirm how provider keys are configured per client.
- Confirm smoke tests for clone readiness.

### 8. Security Foundation

- Define where secrets and provider credentials live.
- Define support access model.
- Define audit events for Business DNA changes, prompt package updates, provider credential updates, support access, approval changes, and publishing actions.

### 9. First Workflow

- Build or prototype the first AI Marketing Team workflow: create marketing content draft from Business DNA, review it, approve it, and store it.
- Track prompt version, Business DNA version, employee, approval state, and user feedback.

### 10. Testing And Verification

- Add tests for required Business DNA fields.
- Add tests for prompt package metadata.
- Add tests for approval states.
- Add smoke checklist for client clone setup.

## Build Phase Success Criteria

The next build phase is successful when:

- Master Admin has a working shell and core registry placeholders.
- Business DNA has a defined implementation schema.
- Prompt packages have a defined format.
- The first AI employees are modeled.
- The first customer workflow path is clear.
- Security decisions for secrets, support access, and audit trails are documented or implemented.

## Keep In Mind

- Revenue first, platform always.
- Do not weaken cloneability.
- Do not expose technical complexity to customers.
- Document important architecture decisions as they happen.
- Keep GitHub updated after Lovable or external tool changes.

## Related Documents

- `PROJECT_STATE.md`
- `ROADMAP.md`
- `FEATURE_ROADMAP.md`
- `BUSINESS_DNA.md`
- `PROMPT_ARCHITECTURE.md`
- `MASTER_ADMIN.md`
- `CLIENT_TEMPLATE.md`
- `SECURITY.md`
