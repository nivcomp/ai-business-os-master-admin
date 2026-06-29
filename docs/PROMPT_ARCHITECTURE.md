# Prompt Architecture

Prompt Architecture defines how AI Business OS turns business context, employee role, workflow state, tools, memory, and safety rules into reliable AI output.

## Purpose

Prompts should be reusable, inspectable, versioned, and connected to Business DNA.

The goal is not to write clever one-off prompts. The goal is to build a prompt system that improves over time and can be packaged across customers.

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

## Versioning

Prompt changes can affect quality, cost, and customer trust. Important prompt templates should be versioned.

A prompt version should record:

- Purpose.
- Owner.
- Supported employee or workflow.
- Required inputs.
- Expected outputs.
- Change notes.

## Safety

Prompts must not encourage bypassing approval for sensitive work. Customer-facing output should clearly support review and editing.

## Related Documents

- `BUSINESS_DNA.md`
- `AI_EMPLOYEES.md`
- `KNOWLEDGE_BASE.md`
- `MEMORY.md`
- `AI_WORKFLOWS.md`
