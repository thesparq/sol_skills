---
name: sol_skills
description: "Setting up and managing any sol.mbt framework frontend or fullstack project using the moonbit program>
metadata:
  author: thesparq  
  version: "1.0.0"
---

# Sol Documentation Guide and skills

This is the entry point for `skills/`. It establishes a fixed reading order by purpose and clarifies the single source of truth for specifications.

## Reading Order

1. Preparing to join development
   - `skills/onboarding.md`
2. Getting started (quickest launch)
   - `skills/quickstart.md`
3. Deploy operations
   - `skills/deploy.md`
4. Incident response
   - `skills/runbook.md`
5. Routing specification
   - `skills/routing.md`
6. Development operations (benchmarking)
   - `skills/benchmarking.md`
7. Troubleshooting
   - `skills/troubleshooting.md`
8. Development experience (HMR)
   - `skills/hot-reload.md`
9. Migration
   - `skills/migrate-from-mars.md`
10. Advanced design (Wasm entrypoint)
   - `skills/wasm-entrypoint.md`

## Links by Purpose

- Want to check specifications
  - `skills/routing.md`
  - `skills/benchmarking.md`
- Want to get it running first
  - `skills/onboarding.md`
  - `skills/quickstart.md`
- Want to check deployment
  - `skills/deploy.md`
- Want to check incident response
  - `skills/runbook.md`
- Want to isolate a problem
  - `skills/troubleshooting.md`
- Want to migrate incrementally from `mars`
  - `skills/migrate-from-mars.md`
- Want to check the HMR contract
  - `skills/hot-reload.md`
- Want to check the future design of `.mbtx` / WASI / WAGI
  - `skills/wasm-entrypoint.md`

## Document Map

| Path | Role | Notes |
|---|---|---|
| `skills/onboarding.md` | Guide | First-day steps for joining development and `just verify` |
| `skills/quickstart.md` | Guide | Shortest steps for `dev -> build -> serve` |
| `skills/deploy.md` | Guide | Preview / production deployment steps for docs |
| `skills/runbook.md` | Operations | Incident response and rollback steps for docs |
| `skills/routing.md` | Specification (single source) | API selection, Layout semantics, `source_path` convention |
| `skills/benchmarking.md` | Specification (single source) | k6 steps, `SOL_BENCH_MODE`, isolating variance under high load |
| `skills/troubleshooting.md` | Operations | Isolating 404/HMR/benchmark variance issues |
| `skills/hot-reload.md` | Design | HMR contract shared between `sol`/`mars` |
| `skills/migrate-from-mars.md` | Guide | Incremental migration from existing `mars` code |
| `skills/wasm-entrypoint.md` | Design draft | Wasm entrypoint direction based on `.mbtx` |

## Update Rules

- For specification changes, update the single source (`skills/routing.md` / `skills/benchmarking.md`) first
- README and supplementary documents should link to the single source and not duplicate the same content
