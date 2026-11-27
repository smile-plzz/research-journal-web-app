# TrailLink

**Community-powered trekking intelligence and destination information platform** (web-first, bilingual Bangla & English PWA), starting in Bandarban, Bangladesh.

## Why TrailLink Exists

Remote trekkers and expedition organisers lack a single, trustworthy place to check whether destinations are currently accessible, whether clearance is required, where para accommodation is available, and how trails look on the ground. TrailLink separates **community observations** from **officially verified access notices** so popularity never overrides safety.

## Core Principles & Guardrails

- **Official beats popular:** Vote counts and provider statements never set official access status (L4 verifiers only).
- **Label everything:** Community data always carries source type, observation date (`observed_at`), and verification status.
- **A route is not permission:** Mapped routes never imply legal or current access.
- **No security operations data:** Troop movements, patrol schedules, and tactical checkpoint details are withheld.
- **Offline-first PWA:** Saved destinations, routes, and cached notices (clearly stamped with `last_synced_at` and never labelled live) work without signal.
- **Bilingual (Bangla & English):** Supported from day one across UI, destination names, and transliteration search.

## Repository Layout

```text
/apps/web          Next.js PWA (explore, map, routes, posts, voting, providers, notices, offline, i18n, admin)
/contracts         OpenAPI spec, event and sync contracts (owner: A2)
/db                PostgreSQL + PostGIS migrations, RLS policies, seed data (owner: A3)
/design            Design tokens, flows, screen specs (owner: A6)
/tests             Unit, integration, end-to-end tests (owner: A16)
/infra             CI/CD, environments, monitoring (owner: A18)
/docs/prd          FR register, user stories, PRD v0.2 (owner: A1)
/docs/architecture Architecture & ADRs (owner: A2)
/docs/policy       Trust and moderation policy (owner: A12)
/docs/security     Threat model, security reviews (owner: A17)
/docs/plan         Task board, wave status, branch rules (owner: A0)
/docs/dev          Developer docs & runbooks (owner: A18)
/docs/handoffs     Task handoff notes (<task-id>.md)
```

## Development Status

- **Current Phase:** Wave 0 (Setup) & Wave 1 (Contracts) toward **Gate G1**.
- See [task-board.md](docs/plan/task-board.md) and [dev-log.md](dev-log.md) for live progress.
