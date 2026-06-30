# Lovable Client Template Prompt

Use this prompt when connecting Lovable to the Client Template repository.

```text
You are building the AI Business OS Client Template, not the Master Admin.

GitHub is the source of truth.

Repository role:
- This repo is the cloneable customer-facing Client Template.
- Do not build Master Admin screens here.
- Master Admin belongs in nivcomp/ai-business-os-master-admin.

Build goal:
Create the first working client app for AI Marketing Team Starter with Copywriter v0.1.

Core principle:
Build one real employee workflow end-to-end. Do not build a fake all-in-one AI marketing platform.

Build these screens:
1. Client Office dashboard
2. Business DNA onboarding/edit screen
3. Employees screen
4. Copywriter employee screen
5. Content request and draft options
6. Approval Center
7. Saved Content
8. Client Settings / Provider Keys placeholder

Do not build yet:
- Master Admin
- Employee marketplace
- Image generation
- Video generation
- Auto publishing
- Full analytics
- Billing
- Enterprise permissions

Data model:
Use local/mock data that follows these concepts:
- Client
- BusinessDNA
- Employee
- ContentRequest
- ContentDraft
- ApprovalItem
- SavedContent
- ActivityEvent
- ClientHealth

Workflow:
1. User completes Business DNA.
2. User opens Copywriter.
3. User requests marketing copy.
4. App creates three draft options using mock AI logic.
5. User selects a draft.
6. User sends it to Approval Center.
7. User approves it.
8. Approved content appears in Saved Content.
9. Activity events update Client Health.

UI language:
Use customer-facing business language:
- Employees
- Business DNA
- Approval Center
- Saved Content
- Office

Avoid technical language in customer UI:
- Agents
- Prompt chains
- Provider adapters
- Embeddings
- Internal registries

Design style:
This is an operational SaaS client workspace. It should feel clear, trustworthy, modern, and useful. Avoid marketing landing-page layouts. Prioritize workflow clarity.

Acceptance criteria:
- Business DNA can be completed.
- Copywriter can create three drafts.
- A draft can be sent to Approval Center.
- A draft can be approved.
- Approved content is saved.
- Activity/health state changes after the workflow.
- No Master Admin screens exist in this repo.
- No hard-coded single-client assumptions beyond seed demo data.
```

## Related Documents

- `CONTROL_PLANE_READY_MVP.md`
- `COPYWRITER_V0_SPEC.md`
- `CLIENT_TEMPLATE_DATA_CONTRACT.md`
- `CLIENT_ADMIN_SYNC_CONTRACT.md`
