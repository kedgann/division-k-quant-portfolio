Layer 6.3 — 15‑Minute Candle Tracking
Mid‑Interval Engine Behavior, Geometry Testing & Movement‑Family Transitions

🔹 Purpose
Layer 6.3 tracks spike events at the 15‑minute resolution, giving you a powerful view of:

Multi‑hour ignition cycles

Macro ladder sequences

Synthetic burst windows

Actor‑driven expansions

Vacuum‑driven collapses

Corridor migrations

Drift‑floor failures

Ceiling‑test sequences

Dump → recovery behavior


Example 15‑Minute Spike Records

JTO — Synthetic Multi‑Hour Ignition Cycle

| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Time | 14:15–14:30 |
| Spike Size | 112 pts |
| Spike Type | Synthetic Burst Cycle |
| Memory Interaction | Medium tap |
| Structure Before | Tight coil → ladder setup |
| Structure After | Multi‑hour ignition → ceiling migration |
| Actor Behavior | High actor presence |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Ignition cycle lasted 2.5 hours; ceiling migrated twice |


SYND — Synthetic Multi‑Phase Flick Cycle

| Field | Value |
| --- | --- |
| Market | SYND |
| Date | 2026‑06‑20 |
| Time | 09:00–09:15 |
| Spike Size | 95 pts |
| Spike Type | Synthetic Flick Cycle |
| Memory Interaction | Shallow tap |
| Structure Before | Tight synthetic coil |
| Structure After | Flick → coil reset → flick |
| Actor Behavior | Medium |
| Book Behavior | Thin |
| Dump Candle Signature | Fast synthetic dump |
| Recovery Signature | Strong synthetic V |
| Notes | Repeated flicks every 15 minutes; actor cluster present |

XPL — Natural Macro Spike

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Time | 10:00–10:15 |
| Spike Size | 85 pts |
| Spike Type | Natural |
| Memory Interaction | None |
| Structure Before | Loose coil |
| Structure After | Slow recovery |
| Actor Behavior | Low |
| Book Behavior | Medium |
| Dump Candle Signature | Natural dump |
| Recovery Signature | Slow |
| Notes | Natural macro spike; no synthetic involvement |


🔹 Schema Connections
Upstream:

Layer 6 — Price Spikes

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.2 — 5‑Minute Spike Tracker

Layer 4.3 — Actor Registry

Downstream:

Layer 6.4 — 1‑Hour Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 7.1 — Synthetic Market Tracker

Layer 7.2 — Patterns


🔹 Navigation
Jump to related layers:

Layer 6 — Price Spikes

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.2 — 5‑Minute Spike Tracker

Layer 6.4 — 1‑Hour Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 7.1 — Synthetic Market Tracker

Layer 7.2 — Patterns