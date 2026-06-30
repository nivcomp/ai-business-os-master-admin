# Capability Validation

AI Business OS must not sell or present a capability as real until that capability has passed a clear validation gate.

This document prevents the product from becoming a beautiful dashboard where the employees sound powerful but only work in theory.

## Core Rule

An employee is not considered real because it has a name, avatar, prompt, or screen.

An employee becomes real only when at least one complete workflow works from input to approved output.

## Capability Definition

A capability is a specific repeatable thing an AI employee can do.

Examples:

- Copywriter creates a social post draft.
- Designer creates three approved image concepts.
- Video Creator creates a script and storyboard.
- Campaign Manager schedules an approved post.
- Analytics Manager summarizes campaign results.

## Validation Levels

### Level 0: Idea

The capability is only a product idea.

It may appear in docs, roadmap, or sales planning, but should not be sold as available.

### Level 1: Designed

The workflow is documented.

Required:

- Inputs defined.
- Outputs defined.
- Employee owner defined.
- Provider needs defined.
- Approval rule defined.

### Level 2: Prototype

The workflow can run manually or with mock providers.

Required:

- Demo data.
- Example input.
- Example output.
- Known limitations.

### Level 3: Working Demo

The workflow works end-to-end in a demo environment.

Required:

- Uses Business DNA.
- Uses the correct employee.
- Produces a useful draft.
- Sends output to Approval Center.
- Stores approved result.
- Records analytics event.

### Level 4: Pilot Ready

The workflow can be used with an early customer under supervision.

Required:

- Real provider adapter or stable manual fallback.
- Error handling.
- Support notes.
- Security review.
- Human approval.
- Basic tests.

### Level 5: Sellable

The capability can be sold as part of a package.

Required:

- Repeatable onboarding.
- Documented limits.
- Pricing assumptions.
- Support process.
- Measured success criteria.
- Rollback or fallback plan.

## Capability Validation Table

Every capability should answer:

| Field | Question |
| --- | --- |
| Capability name | What exact thing can the employee do? |
| Employee owner | Which employee owns it? |
| Media type | Text, image, video, landing page, publishing, analytics, automation, or other? |
| Input | What does the user or workflow provide? |
| Business DNA usage | Which Business DNA fields are required? |
| Provider | Which API or provider adapter is used? |
| Output | What is produced? |
| Approval | Does a human approve it before external use? |
| Test | How do we verify it works? |
| Limitation | What can it not do yet? |
| Sales status | Idea, designed, prototype, demo, pilot, or sellable? |

## Employee Validation Rule

An employee can be displayed in a product demo when it has at least one Level 3 capability.

An employee can be sold when it has at least one Level 5 capability and all advertised capabilities are clearly marked by status.

## Package Validation Rule

A package can be sold only when its core promise is backed by validated capabilities.

For AI Marketing Team Starter, the minimum sellable promise should be:

- Business DNA onboarding works.
- Copywriter can create approved marketing copy.
- Approval Center works.
- Approved content is stored.
- Master Admin can see client health.

## Anti-Fake-MVP Rules

- Do not list a capability as available if it only exists in a prompt.
- Do not sell full automation while approval is still manual-only.
- Do not imply image or video generation works until provider output is tested.
- Do not claim publishing works until channel-specific constraints are handled.
- Do not call an employee complete when only one hidden action works.

## Related Documents

- `MEDIA_BY_MEDIA_ROLLOUT.md`
- `EMPLOYEE_CATALOG.md`
- `MVP_BUILD_PLAN.md`
- `MARKETING_AUTOMATION_ENGINE.md`
- `AI_WORKFLOWS.md`
- `TESTING.md`
