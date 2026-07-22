Includes:

15‑minute spike logs

Spike type classification

Actor involvement

Book behavior

Structural notes

Multi‑hour ignition cycles

Macro burst patterns


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

| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which market the spike occurred in |
| **Date** | When the spike happened |
| **Time (PDT)** | Exact timestamp |
| **Spike Size** | Magnitude of the spike |
| **Spike Type** | Natural / Synthetic / Actor‑Forced / Vacuum |
| **Memory Interaction** | Whether the spike interacted with a memory band |
| **Structure Before** | Engine state before the spike |
| **Structure After** | Engine state after the spike |
| **Actor Behavior** | Actor involvement |
| **Book Behavior** | Thick / thin / hollow |
| **Dump Candle Signature** | Shape & speed of dumps |
| **Recovery Signature** | V‑shape / slow / synthetic |
| **Notes** | Freeform structural notes |


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

Layer 6.3 is the macro‑micro bridge that powers multi‑hour engine analysis.