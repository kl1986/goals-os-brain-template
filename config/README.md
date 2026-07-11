# config

Machine-readable settings that govern how the Engine and Adapters behave in this Brain. Never contains knowledge content — only policy and state.

**What the Engine/Adapters expect to find here:**

- **Model routing** — which model handles which task type (Capability agent work is model-routed per task, not hard-coded into Protocols).
- **Autonomy policy** — per-action-type review window, graduation thresholds, and the minimum temporal spread across distinct days/sessions required before a type can graduate (ADR-0006). Brain-owned config; the Engine ships defaults, this overrides them.
- **Routine state** — last-run timestamps per Routine, read by the heartbeat due-check at session start (ADR-0007).
- **Adapter config** — per-Runtime settings for whichever Adapter(s) this Brain uses (e.g. Claude Code).

Populated by the onboarding Protocol (Phase 1, ticket 05); empty at template-clone time.
