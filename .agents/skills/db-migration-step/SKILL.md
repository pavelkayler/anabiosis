---
name: db-migration-step
description: Execute a database-focused roadmap step using PostgreSQL, TimescaleDB, and Drizzle while preserving schema discipline, retention rules, and versioned configuration.
---

You are handling a database and migration scoped step.

Mandatory rules:

1. Respect PostgreSQL + TimescaleDB + Drizzle architecture.
2. Use Drizzle for normal schema work.
3. Use raw SQL where Timescale-specific behavior is required.
4. Preserve UTC timestamps everywhere.
5. Do not introduce JSONL-first persistence.
6. Do not store full raw orderbook history as the main storage strategy.
7. Preserve retention, compression, and replay/validation requirements.
8. Keep rule versioning and threshold profile versioning intact.
9. Ensure schema remains ready for BTC first, then ETH and SOL later.

Always consider:

- hypertables
- continuous aggregates
- retention policies
- rule_versions
- threshold_profiles
- replay/validation storage
- signal decision history