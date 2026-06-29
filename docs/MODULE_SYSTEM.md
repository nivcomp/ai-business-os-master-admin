# Module System

A module is a reusable product capability that can be enabled, disabled, packaged, upgraded, and reused across client installations.

Modules prevent the product from becoming a collection of one-off screens.

## Module Examples

- Business DNA
- Knowledge Base
- AI Employees
- Content Studio
- Approval Center
- Landing Pages
- CRM Lite
- Analytics
- WhatsApp Integration
- Email Integration

## Module Requirements

Each module should define:

- Purpose.
- Owning application: Master Admin, Client Template, or both.
- Required data models.
- Required providers.
- Permissions.
- Package compatibility.
- Human approval requirements.
- Analytics events.
- Support diagnostics.

## Module Lifecycle

A module may move through these states:

1. Proposed
2. Designed
3. Implemented
4. Packaged
5. Enabled for pilot
6. Available for customers
7. Deprecated

## Architecture Rule

Modules should depend on stable engines and provider abstractions where practical. UI code should not directly own provider-specific behavior.

## Related Documents

- `PACKAGE_SYSTEM.md`
- `FEATURE_ROADMAP.md`
- `ARCHITECTURE.md`
- `CODING_RULES.md`
