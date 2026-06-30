# Template Versioning Model

The Client Template must be cloneable and updateable without losing control of existing clients.

## Version Concepts

### Template Version

The application template version.

Example: `client-template@0.1.0`

### Package Version

The installed product package.

Example: `ai-marketing-team-starter@0.1.0`

### Prompt Package Version

The prompt and employee instruction bundle.

Example: `copywriter-prompts@0.1.0`

### Employee Version

The employee configuration version.

Example: `copywriter@0.1.0`

## MVP Rule

Every client clone should store version values even if update automation is not built yet.

This prevents future clients from becoming untraceable.

## Update Safety

Before updating a client, Master Admin should eventually know:

- Current template version.
- Target template version.
- Installed package version.
- Prompt package version.
- Whether data migration is needed.
- Whether customer approval is needed.
- Rollback notes.

## Clone Registration

When a new client clone is created, it should be registered with:

- Client ID.
- Client name.
- Template ID.
- Template version.
- Package ID.
- Package version.
- Created date.
- Environment.
- Owner.

## Related Documents

- `CONTROL_PLANE_READY_MVP.md`
- `CLIENT_ADMIN_SYNC_CONTRACT.md`
- `UPDATE_SYSTEM.md`
- `PACKAGE_SYSTEM.md`
