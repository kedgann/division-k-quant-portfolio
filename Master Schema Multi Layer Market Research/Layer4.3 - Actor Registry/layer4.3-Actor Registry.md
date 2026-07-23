
Purpose
Layer 4.3 defines the actors that drive engine behavior.

Actors are the “micro‑agents” inside your synthetic or natural engines.
They create bursts, cascades, drift floors, vacuum spikes, ceiling tests, compression phases, purges, repairs, anchors, and migrations.

This layer documents:

Actor types

What each actor does

Where each actor operates (lane scope)

Required spacing

Conditions for activation

Which movement families each actor belongs to


🔹 Actor Registry Table
This is the full structured registry — the strongest part of Layer 4.3.

| **Actor Type** | **Purpose** | **Lane Scope** | **Spacing** | **Conditions** | **Families** |
| --- | --- | --- | --- | --- | --- |
| **Burst** | Sudden expansion bursts | B‑C‑D‑Ceiling | +5–10 | Needs intact geometry, mid‑book thickness | Expansion, Cascade, Ceiling‑Test |
| **Cascade** | Multi‑lane inheritance | C‑D‑Ceiling | +10–20 | Needs intact geometry, actor presence | Cascade, Expansion, Ceiling‑Test |
| **Drift** | Maintains drift floors | Drift‑A | 1–3 | Needs stable drift corridor | Drift, Expansion |
| **Vacuum** | Hollow‑book displacement | C→A / B→D | +15–40 | Needs hollow zones, missing shelves | Inversion, Purge |
| **Ceiling‑Test** | Tests ceiling boundary | D‑Ceiling | +5–12 | Needs intact ceiling geometry | Ceiling‑Test, Expansion, Migration |
| **Compression** | Tightens lane spacing | A‑B | 1–4 | Needs stable lower geometry | Drift, Expansion |
| **Purge** | Clears stacked highs/lows | A‑Drift / C‑D | −10–25 | Needs congestion, stale geometry | Purge, Decay‑Repair |
| **Weaver** | Maintains corridor spacing | A‑B‑C (D optional) | 5‑spacing | Needs intact corridor structure | Weaver, Drift, Expansion |
| **Inversion** | Chaotic spacing | A‑Drift / C‑D | +10 to −20 | Needs broken geometry, hollow zones | Inversion, Purge |
| **Repair** | Controlled descent | B‑A‑Drift | −5–12 | Needs unstable geometry, actor presence | Decay‑Repair, Ceiling‑Test |
| **Anchor** | Defines meaningful highs/lows | A‑Drift‑C / D‑Ceiling | Stable | Needs stable geometry, repeated taps | Drift, Expansion, Cascade |
| **Migration** | Moves ceiling/floor | Ceiling‑D / Drift‑A | +8–15 | Needs boundary instability | Migration, Ceiling‑Test |


Schema Connections
Upstream:

Layer 4 — Engine Map

Layer 4.2 — Movement‑Family Behavior

Downstream:

Layer 5 — Memory Taps

Layer 6 — Spike System

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 7.2 — Patterns

Layer 4.3 is the actor‑logic layer that powers all deeper structural analysis.

Navigation
Jump to related layers:

Layer 4 — Engine Map

Layer 4.2 — Movement‑Family Behavior

Layer 5 — Memory Taps

Layer 6 — Spike System

Layer 7.2 — Patterns