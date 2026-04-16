# Repository expectations

## Language rules
- Always respond to the user in Russian unless the user explicitly asks for another language.
- Keep reports, explanations, progress updates, and implementation summaries in Russian.
- Code, filenames, API field names, SQL identifiers, and technical symbols should remain in their technically correct original form unless the user explicitly requests translation.

## Workflow
- Work strictly one roadmap file at a time.
- Never jump ahead.
- Close all unresolved items from the previous report before starting the next file.
- After a roadmap file is fully complete, rename it to `_done`.

## Delivery
- For chat-based delivery, return full updated files only, never diff/patch.
- Always write a report for the current roadmap file.
- Never claim completion if there are unresolved blockers.

## Backend
- TypeScript + Fastify only.
- WebSocket-first, REST only for bootstrap/history/recovery.
- PostgreSQL + TimescaleDB + Drizzle.
- All timestamps must be UTC.
- Separate spot and linear strictly.

## Signal rules
- No tradeable ENTER before closed 1m confirmation.
- No tradeable decision without valid entry/invalidation/targets.
- WAIT and INVALID must always include a human-readable explanation.

## Frontend
- Vite latest + React + TypeScript.
- FSD-like structure: app/pages/features/shared.
- Header must show current phase and current md file.
- UI is read-only in v1.

## Verification
- Use the project bat files for build/test/smoke.
- If checks cannot be run, explicitly say what must be run manually.