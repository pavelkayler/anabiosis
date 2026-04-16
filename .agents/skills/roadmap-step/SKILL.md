---
name: roadmap-step
description: Implement exactly one roadmap x.y.md file in strict sequence, close report tails first, stay within scope, update tests, write the report, and rename the roadmap file to _done only when the step is fully complete.
---

You are executing exactly one roadmap step for this repository.

Mandatory workflow:

1. Read `docs/roadmap/0.md`.
2. Read the exact roadmap file requested by the user.
3. Read the latest relevant file in `docs/reports/`.
4. Before doing any new work, close all unresolved tails from the previous report that are still relevant.
5. Implement only the scope of the current roadmap file.
6. Do not jump ahead.
7. Do not perform broad refactors outside the current scope.
8. Keep files modular and readable. Avoid large files and do not create monster files.
9. Update or add tests for the new logic where appropriate.
10. Use the project bat files for verification when available.
11. Write a report in `docs/reports/`.
12. Rename the roadmap file to `_done` only when the step is fully complete.

Repository-specific mandatory rules:

- TypeScript + Fastify for backend.
- Vite latest + React + TypeScript for frontend.
- PostgreSQL + TimescaleDB + Drizzle.
- WebSocket-first, REST only for bootstrap/history/recovery.
- All timestamps must be UTC.
- Separate spot and linear data strictly.
- Tradeable ENTER is allowed only after closed 1m confirmation.
- No tradeable decision without valid entry, invalidation, and targets.
- WAIT and INVALID must always include a human-readable explanation.
- Frontend must show current phase and current md file in the header.
- UI is read-only in v1.

Output discipline:

- Do not claim completion if there are unresolved blockers.
- For chat delivery mode, produce full updated files only, never diff/patch.
- Always state what was not verified.
- Always list which bat files the user should run manually when needed.