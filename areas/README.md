# areas

The curated layer: one subfolder per life area, each holding the goals, standards, and decisions the user has made for that area, plus that area's Area agent memory. Human-authored — the machine reads this layer, only the user writes it. Boundary test: did the user *decide* it (→ here) or *learn* it (→ `../wiki/`)?

**What the Engine/Adapters expect to find here:**

- One `<area>/` subfolder per Area agent, instantiated by the onboarding Protocol (name, tone, and area chosen by the user — the Engine ships a generic Area CEO charter, not fixed area names).
- Inside each area: a standard (what "good enough" looks like), current goals, and an `_memory` note the Area agent reads for continuity.
- Area agents plan against this layer plus the Wiki; they direct Capability agents, never execute directly.

Empty at template-clone time — populated area by area during onboarding (Phase 1, ticket 05).
