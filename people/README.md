# people

One hub per person the user works or lives with — the source of truth for what's being waited on from them and the running context of the relationship.

**What the Engine/Adapters expect to find here:**

- One note per person, holding `#waiting-for` items (things delegated to that human, awaiting their reply or deliverable), plus whatever context helps prep a conversation with them.
- Any cross-hub "waiting for" roll-up (e.g. a dashboard view) is a read-only derivation over this folder, never a second place to log a delegation.

Empty at template-clone time.
