Includes:

1‑hour spike logs

Spike type classification

Actor involvement

Book behavior

Structural notes

Multi‑day ignition cycles

Macro burst patterns

Ceiling migration sequences

🔹 Navigation
Jump to related layers:

Layer 6 — Price Spikes

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.2 — 5‑Minute Spike Tracker

Layer 6.3 — 15‑Minute Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 6.8 — Flat Spike Markets

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


🔹 Example 1‑Hour Spike Records

JTO — Synthetic Multi‑Day Ignition Cycle

| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Time | 14:00–15:00 |
| Spike Size | 210 pts |
| Spike Type | Synthetic Burst Cycle |
| Memory Interaction | Medium tap |
| Structure Before | Tight coil → ladder setup |
| Structure After | Multi‑day ignition → ceiling migration |
| Actor Behavior | High actor presence |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Ignition cycle lasted 6+ hours; ceiling migrated 3 times |


SYND — Synthetic Multi‑Phase Flick Cycle (Macro)

| Field | Value |
| --- | --- |
| Market | SYND |
| Date | 2026‑06‑20 |
| Time | 09:00–10:00 |
| Spike Size | 155 pts |
| Spike Type | Synthetic Flick Cycle |
| Memory Interaction | Shallow tap |
| Structure Before | Tight synthetic coil |
| Structure After | Flick → coil reset → flick → burst |
| Actor Behavior | Medium |
| Book Behavior | Thin |
| Dump Candle Signature | Fast synthetic dump |
| Recovery Signature | Strong synthetic V |
| Notes | Repeated flicks every hour; actor cluster present |

ALLO — Synthetic Burst Expansion (Macro)

| Field | Value |
| --- | --- |
| Market | ALLO |
| Date | 2026‑06‑21 |
| Time | 11:00–12:00 |
| Spike Size | 268 pts |
| Spike Type | Synthetic Burst |
| Memory Interaction | Medium tap depth |
| Structure Before | Tight coil |
| Structure After | Burst → macro expansion |
| Actor Behavior | High |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Burst expanded into a multi‑hour macro cycle |

XPL — Natural Macro Spike

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Time | 10:00–11:00 |
| Spike Size | 120 pts |
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

Layer 6.3 — 15‑Minute Spike Tracker

Layer 4.3 — Actor Registry

Downstream:

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 6.8 — Flat Spike Markets

Layer 7.1 — Synthetic Market Tracker

Layer 7.2 — Patterns

Layer 6.4 is the macro spike‑cycle layer that powers multi‑day synthetic engine analysis.