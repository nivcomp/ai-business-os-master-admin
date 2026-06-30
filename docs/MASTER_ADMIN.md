# Master Admin

Master Admin is the private control center for AI Business OS.

It is used by the company to manage customers, templates, packages, AI employees, prompts, provider settings, update delivery, support access, client health, and operational oversight.

## Core Responsibilities

Master Admin owns:

- Client registry and installation status.
- Template registry and clone readiness.
- Package registry.
- Prompt package registry.
- AI employee registry.
- Provider policy and configuration standards.
- Update Center.
- Support access and diagnostics.
- Client health and usage visibility.
- Internal operational reporting.

## What Master Admin Controls

### Clients

Master Admin should track each client installation, including client name, status, package, version, environment, health, support state, and last activity.

### Templates

Master Admin should track Client Template versions, clone readiness, required environment variables, required setup steps, and compatibility with packages.

### Prompt Packages

Master Admin should own prompt package creation, versioning, testing status, approval status, rollout status, and rollback notes.

### AI Employees

Master Admin should define reusable employee templates, responsibilities, tools, prompt package compatibility, default approval rules, and package availability.

### Update Center

Master Admin should coordinate package, prompt, employee, module, template, and security updates across client installations.

### Support Access

Master Admin should grant limited, auditable support access to client installations when needed.

Support access should be time-limited where practical and should avoid exposing customer content unless required.

### Package Registry

Master Admin should maintain the list of installable packages, including AI Marketing Team, package versions, included modules, employee templates, prompt packages, setup steps, and provider requirements.

### Client Health

Master Admin should show health indicators such as onboarding completion, Business DNA status, package version, approval activity, provider errors, support tickets, and usage activity.

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

## First Build Screens

The first Master Admin build should prioritize:

- Dashboard.
- Clients list.
- Client detail.
- Template registry.
- Package registry.
- Prompt package registry.
- AI employee registry.
- Update Center placeholder.
- Support access controls.
- Client health summary.

## Architecture Decisions

Master Admin is the only place that should coordinate updates across clients.

Package publishing, employee template publishing, provider policy, prompt package publishing, and version rollout decisions belong here.

## Related Documents

- `ARCHITECTURE.md`
- `CLIENT_TEMPLATE.md`
- `PACKAGE_SYSTEM.md`
- `PROMPT_ARCHITECTURE.md`
- `UPDATE_SYSTEM.md`
- `MULTI_TENANT.md`
- `SUPPORT.md`
- `SECURITY.md`
