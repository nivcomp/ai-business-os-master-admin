# Lovable Repo Connection Guide

Lovable should connect to the Client Template repository when building the customer-facing app.

## Repository To Connect

Use:

```text
nivcomp/ai-business-os-client-template
```

Do not connect Lovable to `nivcomp/ai-business-os-master-admin` when the task is to build the customer app.

## Responsibilities

### GitHub

GitHub defines:

- Product boundaries.
- Architecture.
- Data models.
- Routes.
- Components.
- Documentation.
- Acceptance criteria.

### Codex

Codex should:

- Create code structure.
- Review Lovable changes.
- Keep docs aligned.
- Prevent architecture drift.
- Commit intentional changes.

### Lovable

Lovable should:

- Improve UI.
- Build screens inside existing boundaries.
- Use existing routes and data models.
- Avoid building the wrong app.

Lovable should not decide product architecture.

## Connection Steps

1. Open Lovable.
2. Choose import/connect GitHub repository.
3. Select `nivcomp/ai-business-os-client-template`.
4. Confirm the branch is `main`.
5. Give Lovable the prompt from `LOVABLE_CLIENT_TEMPLATE_PROMPT.md`.
6. Ask Lovable to build only the Client Template first workflow.
7. Review generated changes in GitHub.
8. Use Codex to check the code against the docs.

## Rule

Code-first, Lovable-assisted.

GitHub defines product, architecture, data, and boundaries. Lovable may improve UI and implementation details only inside those boundaries.
