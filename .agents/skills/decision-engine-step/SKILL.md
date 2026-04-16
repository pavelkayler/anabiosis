---
name: decision-engine-step
description: Implement or modify regime, bias, setup, geometry, explanation, or final decision logic while preserving the repository's closed-1m tradeability rule and explanation discipline.
---

You are handling a decision-engine-focused roadmap step.

Mandatory decision rules:

1. Tradeable ENTER is allowed only after closed 1m confirmation.
2. Intrabar states may exist only as preview, watchlist, wait, or invalid style states.
3. Bias alone is insufficient without a valid setup.
4. No tradeable decision without valid:
   - entry zone
   - invalidation
   - target(s)
5. WAIT and INVALID must include a human-readable explanation.
6. Separate spot and linear logic strictly.
7. Preserve normalization, stale budgets, cooldown, expiry, and versioned threshold profiles.
8. Keep trap, failed continuation, and absorption logic distinct.
9. Preserve replay and validation compatibility.

When changing decision logic, always consider:

- eligibility
- regime
- bias
- setup
- geometry
- explanation
- persistence
- outcome validation