# Marketing Automation Engine

The Marketing Automation Engine is the system that helps AI Marketing Team plan, create, approve, publish, measure, and improve marketing work.

It should automate execution while preserving human control.

## Purpose

The engine turns Business DNA, knowledge, employees, prompts, providers, approval rules, and analytics into repeatable marketing workflows.

The first version should support guided automation, not uncontrolled autopilot.

## Core Loop

1. Understand the business through Business DNA.
2. Plan campaign or content work.
3. Create draft assets.
4. Send drafts to Approval Center.
5. Apply requested changes.
6. Publish or export only after approval.
7. Measure performance.
8. Recommend improvements.
9. Feed learnings into the next cycle.

## Main Capabilities

### Marketing Plan

The Marketing Manager creates a plan based on business goals, offers, target audience, channels, seasonality, past performance, and available employees.

### Content Calendar

The engine should maintain a simple content calendar with:

- Topic.
- Channel.
- Owner employee.
- Draft status.
- Approval status.
- Scheduled date.
- Publish status.
- Performance notes.

### Content Creation

The engine should coordinate employees such as Copywriter, Designer, and Video Creator.

Each draft should record:

- Employee.
- Prompt package version.
- Business DNA version.
- Knowledge used.
- Provider used.
- Approval state.

### Approval Center

Approval is central. Drafts should move through states:

- Draft.
- Needs Review.
- Changes Requested.
- Approved.
- Scheduled.
- Published.
- Rejected.
- Archived.

### Publishing And Distribution

Publishing should be provider-based and approval-first.

The engine may prepare posts, emails, landing pages, WhatsApp campaigns, or ads, but final external action requires explicit approval unless automation is later configured by the user.

### Analytics And Improvement

The Analytics Manager should summarize:

- What was created.
- What was approved.
- What was published.
- What performed well.
- What should improve next.

## Automation Levels

### Level 1: Assisted Drafting

AI creates drafts. Human approves everything.

### Level 2: Guided Scheduling

AI creates a plan and schedule. Human approves the calendar and each external action.

### Level 3: Approved Automation

User explicitly authorizes limited automatic publishing under defined rules.

### Level 4: Managed Autopilot

Future state. The system runs approved campaigns within policy and escalates exceptions.

The MVP should start at Level 1 and limited Level 2.

## MVP Workflow

1. Customer completes Business DNA.
2. Marketing Manager creates a campaign idea.
3. Copywriter creates a social post draft.
4. Customer reviews in Approval Center.
5. Customer approves or requests changes.
6. Approved draft is saved.
7. Analytics event records first value.

## Related Documents

- `EMPLOYEE_CATALOG.md`
- `AI_WORKFLOWS.md`
- `PROMPT_ARCHITECTURE.md`
- `API_PROVIDER_STRATEGY.md`
- `ANALYTICS.md`
- `MVP_BUILD_PLAN.md`
