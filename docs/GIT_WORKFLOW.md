# Git Workflow

GitHub is the single source of truth for AI Business OS technical documentation, decisions, and future code.

## Branching

Use `main` as the source of truth.

For larger implementation work, prefer feature branches and pull requests. For documentation sprints using trusted automation, grouped direct commits are acceptable when requested.

## Commit Grouping

Do not create one commit per file during documentation sprints.

Group commits by purpose:

- Company foundation
- Vision and roadmap
- Architecture documentation
- AI documentation
- Development documentation
- Product documentation
- Business documentation

## Commit Messages

Use clear messages:

- `docs: add company foundation`
- `docs: add architecture documentation`
- `docs: add AI documentation`
- `docs: add product documentation`
- `docs: add business documentation`
- `feat: add approval workflow foundation`
- `fix: prevent hard-coded client settings`

## Pull Requests

A pull request should explain:

- What changed.
- Why it changed.
- What documents or decisions are affected.
- How it was tested.
- Risks or follow-up work.

## Protected Behaviors

Do not rewrite history on shared branches unless explicitly approved.

Do not force-push `main`.

Do not commit secrets, environment files, customer data, or local tool output.

## Related Documents

- `CONTRIBUTING.md`
- `CODING_RULES.md`
- `SECURITY.md`
- `TESTING.md`
