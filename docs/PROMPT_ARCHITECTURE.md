# Prompt Architecture

Prompt Architecture defines how AI Business OS turns business context, employee role, workflow state, tools, memory, and safety rules into reliable AI output.

## Purpose

Prompts should be reusable, inspectable, versioned, testable, and connected to Business DNA.

The goal is not to write clever one-off prompts. The goal is to build a prompt system that improves over time and can be packaged across customers.

## Prompt Layers

### Global Prompt

The Global Prompt defines platform-wide behavior.

It should include:

- AI Business OS identity.
- Safety rules.
- Human approval requirements.
- Customer language rules.
- Output quality expectations.
- Prohibited behavior.
- Tool use boundaries.

The Global Prompt should be managed by Master Admin and versioned carefully because it can affect all clients and all employees.

### Client Prompt

The Client Prompt adapts the system to one customer's Business DNA.

It should include:

- Business profile summary.
- Brand voice.
- Offers and services.
- Target audience.
- Languages.
- Restrictions.
- CTAs.
- Channel preferences.

The Client Prompt should be generated from Business DNA, not hand-written as a hidden one-off prompt.

### Task Prompt

The Task Prompt defines the immediate job.

It should include:

- User request.
- Workflow stage.
- Employee role.
- Required output format.
- Relevant knowledge records.
- Tool instructions.
- Approval or review requirements.

## Prompt Inputs

A production prompt may combine:

- Employee role and responsibilities.
- Business DNA.
- Relevant knowledge base records.
- Workflow stage.
- User request.
- Output format.
- Brand voice.
- Channel constraints.
- Approval and safety rules.
- Tool availability.

## Prompt Blocks

Prompts should be composed from reusable blocks where practical:

- System policy block.
- Employee role block.
- Business DNA block.
- Knowledge context block.
- Task instruction block.
- Output format block.
- Safety and approval block.
- Channel constraint block.
- Tool use block.
- Localization block.

## Prompt Packages

A Prompt Package is a versioned bundle of prompt blocks, employee instructions, required Business DNA fields, workflow settings, output schemas, and tests.

Prompt packages should define:

- Package name.
- Version.
- Supported employees.
- Supported workflows.
- Required Business DNA fields.
- Required tools.
- Output formats.
- Approval requirements.
- Test scenarios.
- Rollback notes.

Prompt Packages belong to the Master Admin package and prompt registries.

## Versioning

Prompt changes can affect quality, cost, and customer trust. Important prompt templates should be versioned.

A prompt version should record:

- Purpose.
- Owner.
- Supported employee or workflow.
- Required inputs.
- Expected outputs.
- Change notes.
- Test results.
- Approval status.
- Rollout status.

## Testing

Prompt testing should include:

- Scenario tests for common customer requests.
- Business DNA variation tests.
- Language tests.
- Restriction and safety tests.
- Output format tests.
- Regression tests for previously approved examples.
- Cost and latency checks when provider behavior matters.

No major prompt package should be rolled out without at least a small set of documented test scenarios.

## Approvals

Prompt changes that affect customer-facing output, publishing behavior, compliance, regulated claims, or external tools should require review before rollout.

Approval records should include who approved the prompt package, what was tested, and which clients or packages are affected.

## Safety

Prompts must not encourage bypassing approval for sensitive work. Customer-facing output should clearly support review and editing.

## Related Documents

- `BUSINESS_DNA.md`
- `AI_EMPLOYEES.md`
- `KNOWLEDGE_BASE.md`
- `MEMORY.md`
- `AI_WORKFLOWS.md`
- `MASTER_ADMIN.md`
- `PACKAGE_SYSTEM.md`
