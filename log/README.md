# log

The Action Log: the single append-only record every agent action writes to, regardless of which agent took it (ADR-0005). The audit trail, and the substrate the learning loop feeds on.

**What the Engine/Adapters expect to find here:**

- One markdown file per day, named `YYYY-MM-DD.md`, entries appended in chronological order — never edited or deleted, only appended and, for feedback, filled in.
- If concurrent multi-agent writes ever make single-file contention a real problem, the write pattern shards to one file per actor per day (`YYYY-MM-DD-<actor>.md`), merged into the review surface by script — a documented contingency, not the default.
- Entry schema (fields, semantics, worked example) is defined in the Engine's `protocols/action-log-schema.md` — see [`goals-os-engine`](https://github.com/kl1986/goals-os-engine).

This folder starts empty; the first entry is written the first time any agent takes an action in this Brain.
