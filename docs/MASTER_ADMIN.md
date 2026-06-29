# Master Admin

Master Admin is the private control center for AI Business OS.

It is used by the company to manage customers, templates, packages, AI employees, prompts, provider settings, update delivery, support access, client health, and operational oversight.

## Responsibilities

Master Admin owns:

- Client registry and installation status.
- Template and package management.
- Employee and prompt governance.
- Provider configuration standards.
- Update publishing and rollout control.
- Support access and diagnostics.
- Client health and usage visibility.
- Internal operational reporting.

## Non-Responsibilities

Master Admin should not become the customer's daily workspace.

It should not own customer-facing marketing workflows, content approval screens, customer CRM records, or customer business data except where needed for support, diagnostics, or controlled administration.

## Users

Primary users are internal operators, founders, support staff, implementation engineers, and authorized AI agents.

Future permission levels should include:

- Owner
- Admin
- Support
- Implementation
- Viewer
- Automation service account

## Data Boundaries

Master Admin may know that a client exists, what version they run, which packages are installed, what support state they are in, and high-level health metrics.

Sensitive customer content should remain in the Client Template unless explicit support access is granted and audited.

## Architecture Decisions

Master Admin is the only place that should coordinate updates across clients.

Package publishing, employee template publishing, provider policy, and version rollout decisions belong here.

## Related Documents

- `ARCHITECTURE.md`
- `CLIENT_TEMPLATE.md`
- `PACKAGE_SYSTEM.md`
- `UPDATE_SYSTEM.md`
- `MULTI_TENANT.md`
- `SUPPORT.md`
