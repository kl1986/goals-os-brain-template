# Goals OS Brain Template

This is the blank, example-populated starting point for a **Brain** — the private repo that holds everything personal in [Goals OS](https://github.com/kl1986/goals-os-engine). Full definition in the Engine's [`CONTEXT.md`](https://github.com/kl1986/goals-os-engine/blob/main/CONTEXT.md#brain) glossary.

Use this template repo to create your own Brain, then clone it locally alongside the [Engine](https://github.com/kl1986/goals-os-engine) — the shared, zero-user-data core that drives protocols against your Brain but never stores anything in it.

## What cloning this gives you

A complete, navigable folder layout — each top level folder has its own README explaining its purpose and what the Engine/Adapters expect to find there:

```
config/            # model routing, autonomy policy, routine state, adapter config
inbox/raw/         # Raw Captures land here first, immutable, per-source subfolders
log/               # the Action Log — daily files, append-only
areas/<area>/      # curated layer: goals, standards, decisions + agent memory
projects/          # active projects with next actions
wiki/              # machine-compiled knowledge, resynthesisable
archive/           # processed raw, completed projects
people/            # person hubs, waiting-for
```

Everything is empty at clone time — folders fill in as the onboarding Protocol runs and you start using the system. (Whether the template should instead ship with a worked example persona for evaluation before commitment is still an open question — see the PRD.)

## Getting started

1. Click **Use this template** to create your own private Brain repo.
2. Clone it locally.
3. Clone the [Engine](https://github.com/kl1986/goals-os-engine) alongside it and follow its onboarding protocol.

## Status

Early scaffold — Phase 1 of the roadmap. Not yet installable.

## Licence

MIT — see [LICENSE](./LICENSE).
