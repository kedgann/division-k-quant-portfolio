Layer 4.2 — Movement‑Family Behavior
Engine Movement Families, Structural Phases, Geometry Tests & Transition Logic

Purpose
Layer 4.2 defines movement families — the internal “states” an engine cycles through as it moves, tests geometry, breaks structure, or transitions into new behavior.

Movement families describe:

how the engine approaches geometry

how it tests structure

how it resolves movement

how it transitions into new families

how actors and book conditions influence movement

how ceilings, floors, and drift lanes evolve

This layer is the engine state machine.

Movement Family Components

| Component | Description |
| --- | --- |
| **Family Lifespan** | How long the engine stays in a movement family |
| **Branch Structure** | Continuation vs failure paths |
| **Sequence Phases** | Approach → Test → Resolution |
| **Timing Windows** | Duration of each phase |
| **Geometry‑Break Conditions** | What causes structure to fail |
| **Family‑Switch Triggers** | What causes transitions |
| **Anchor Relevance** | When anchors matter or decay |
| **Inversion Turbulence** | Turbulence during inversion attempts |
| **Ceiling Migration** | How ceilings shift during movement |
| **Decay Repair** | How the engine repairs broken geometry |
| **Drift Floor Formation** | How drift floors form or fail |
| **Purge Sweep Logic** | How purge‑style sweeps occur |
| **Actor Requirements** | Actor presence needed for each family |
| **Book Requirements** | Book thickness/hollowness needed |