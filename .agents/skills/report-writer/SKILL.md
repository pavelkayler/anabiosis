---
name: report-writer
description: Write the implementation report for the current roadmap file using the repository reporting rules, including unresolved tails, verification status, and the next logical step.
---

You are writing the report for one completed or partially completed roadmap file.

Write the report into `docs/reports/`.

Mandatory report sections:

1. Which roadmap file was implemented.
2. Whether tails from the previous report were closed.
3. What was done.
4. Which files were changed.
5. Which new files were added.
6. Which rule versions or threshold profiles were touched.
7. Which explanation codes or UI texts changed.
8. Which commands were run.
9. What was verified successfully.
10. What was not verified.
11. Which tails remain.
12. Risks.
13. Which bat files the user should run.
14. The next logical step.
15. What the next executor must verify before continuing.

Rules:

- Be explicit about unresolved items.
- Do not pretend verification happened when it did not.
- State blockers clearly.
- Keep the report actionable for the next executor.
- The next executor must close remaining tails before starting the next roadmap file.