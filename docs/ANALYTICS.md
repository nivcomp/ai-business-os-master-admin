# Analytics

Analytics should show whether AI Business OS creates customer value and whether the platform is healthy.

## Product Analytics Goals

Track whether customers:

- Complete onboarding.
- Fill Business DNA.
- Use AI employees.
- Create drafts.
- Approve or reject output.
- Publish or use approved work.
- Return after first use.
- Need support.

## First Events

Suggested initial events:

- `business_dna_started`
- `business_dna_completed`
- `employee_opened`
- `workflow_started`
- `draft_created`
- `draft_approved`
- `changes_requested`
- `content_published`
- `support_requested`
- `package_enabled`

## Master Admin Analytics

Master Admin should monitor:

- Client health.
- Installed package version.
- Update status.
- Workflow usage.
- Approval bottlenecks.
- Provider errors.
- Support load.

## Business Analytics

Business analytics should support pricing, retention, onboarding, and product decisions.

Useful metrics include activation rate, time to first approved output, approval rate, repeat usage, support tickets, and churn risk.

## Privacy

Analytics must respect client isolation and avoid storing sensitive content unless clearly required and permissioned.

## Related Documents

- `AI_WORKFLOWS.md`
- `CUSTOMER_LIFECYCLE.md`
- `PRICING.md`
- `SUPPORT.md`
- `MULTI_TENANT.md`
