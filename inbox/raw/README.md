# inbox/raw

Every captured input lands here first, as an immutable Raw Capture: markdown with typed frontmatter, stamped on ingestion — by a script wherever possible, not an LLM — so the ground truth is never rewritten.

**What the Engine/Adapters expect to find here:**

- One file per capture, frontmatter-stamped with at minimum a source, a timestamp, and an id.
- Per-source subfolders (e.g. voice, email, meetings, web), created as capture Routines are configured for this Brain — no fixed list is imposed by the Engine.
- Files are **never edited in place** after capture. Triage and synthesis read from here; nothing writes back except the move to `../../archive/` once processed.

The Triage Routine (EA) classifies everything here against structured routing rules and proposes a Triage Plan — a classify-only pass, so nothing captured here can itself trigger an action.
