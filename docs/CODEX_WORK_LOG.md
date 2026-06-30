# Codex Work Log

This file records completed Codex tasks in this repository.

It is factual and concise so a CTO reviewer can understand what changed without reading every file first.

## 2026-06-30 - Document Customer-Owned Telephony Decision

### Task Summary

Added architecture decision `FD-014: Customer-owned telephony by default` to define how future Voice Layer and Voice Receptionist Employee telephony ownership should work.

### Files Changed

- `docs/DECISIONS.md`
- `docs/CODEX_WORK_LOG.md`

### Architecture Decisions Made

- Future voice and telephony providers should be client-owned or client-isolated by default.
- A shared pooled telephony account requires a documented architecture and business decision before use.
- AI Business OS owns orchestration, workflow logic, provider abstraction, Voice Receptionist behavior, call logs, CRM Lite records, and support visibility.
- Application data should store provider references, ownership metadata, phone numbers or extensions, connection status, and provider policy data.
- Provider secrets must not be committed to GitHub or stored directly in normal application tables.

### What Was Intentionally Not Built

- No voice features.
- No telephony integration.
- No provider adapter implementation.
- No secrets storage.
- No Voice Receptionist Employee runtime behavior.

### Known Issues

- Future `VOICE_LAYER.md` does not exist yet in this Master Admin repository.
- Provider-specific telephony account setup, billing, support access, and offboarding flows are not implemented.

### Build/Test Result

- No build was run because this was documentation-only.

### Recommended Next Step

Keep Copywriter v0.1 as the current MVP and document the future Voice Layer before implementing any voice provider adapters.
