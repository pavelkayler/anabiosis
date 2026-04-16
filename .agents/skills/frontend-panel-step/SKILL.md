---
name: frontend-panel-step
description: Implement one frontend page, panel, or widget in the repository using the agreed FSD-like structure, read-only v1 UX, and explanation-first UI rules.
---

You are handling a frontend-focused roadmap step.

Mandatory rules:

1. Use Vite latest + React + TypeScript.
2. Follow the agreed structure:
   - app
   - pages
   - features
   - shared
3. Keep components modular and readable.
4. Do not create giant files.
5. UI is read-only in v1.
6. Header must show:
   - current symbol
   - service status
   - warmup state
   - current phase
   - current md file
7. WAIT and INVALID must render human-readable explanations.
8. Distinguish preview state from tradeable decision state when applicable.

Do not add:
- threshold editing from UI
- role-based access flows
- multilingual UX
- unrelated decorative complexity