# Client Admin Sync Contract

This contract defines the minimal information a Client Template clone should expose or report so Master Admin can manage it.

The MVP may use mock data or manual registration, but the data contract should be designed from the beginning.

## Sync Direction

Client Template reports operational state.

Master Admin tracks, supports, and eventually updates client installations.

## Client Identity

Each Client Template clone must have:

- `clientId`
- `clientName`
- `environment`
- `templateId`
- `templateVersion`
- `installedPackageId`
- `installedPackageVersion`

## Health Fields

Client health should include:

- Business DNA completion status.
- Enabled employees.
- Last employee activity.
- Drafts created.
- Approval items pending.
- Approved content count.
- Provider configuration status.
- Last sync time.
- Error status.

## Activity Events

Client Template should record events such as:

- `business_dna_completed`
- `employee_opened`
- `copywriter_request_created`
- `content_draft_created`
- `approval_item_created`
- `content_approved`
- `content_saved`
- `provider_error`

## Master Admin MVP View

The first Master Admin can show a simple client health table:

| Field | Meaning |
| --- | --- |
| Client | Customer name |
| Template Version | Which template clone version runs |
| Package | Installed package |
| Business DNA | Complete or incomplete |
| Active Employee | Last employee used |
| Approved Content | Count of approved assets |
| Health | Healthy, needs setup, warning, or error |

## Future Sync

Later versions may support:

- Webhook reporting.
- Pull-based health checks.
- Update eligibility checks.
- Package update recommendations.
- Support access sessions.

## Related Documents

- `CONTROL_PLANE_READY_MVP.md`
- `CLIENT_TEMPLATE_DATA_CONTRACT.md`
- `MASTER_ADMIN.md`
- `CLIENT_TEMPLATE.md`
- `UPDATE_SYSTEM.md`
