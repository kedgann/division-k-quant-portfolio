
includes:

5‑minute spike logs

Spike type classification

Actor involvement

Book behavior

Structural notes

Ladder sequences

Mid‑scale burst patterns


🔹 Navigation
Jump to related layers:

Layer 6 — Price Spikes

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.3 — 15‑Minute Spike Tracker

Layer 6.4 — 1‑Hour Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

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


🔹 Example 5‑Minute Spike Records

JTO — Synthetic Ladder Burst (5‑Minute Window)

| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Time | 14:30–14:35 |
| Spike Size | 68 pts |
| Spike Type | Synthetic Ladder Burst |
| Memory Interaction | Medium tap |
| Structure Before | Tight coil → ladder setup |
| Structure After | Ladder continuation → burst |
| Actor Behavior | High actor presence |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Ladder bot climbed 4 shelves in 5‑minute window |

SYND — Synthetic Multi‑Minute Flick

| Field | Value |
| --- | --- |
| Market | SYND |
| Date | 2026‑06‑20 |
| Time | 09:10–09:15 |
| Spike Size | 72 pts |
| Spike Type | Synthetic Flick |
| Memory Interaction | Shallow tap |
| Structure Before | Tight synthetic coil |
| Structure After | Flick → coil reset |
| Actor Behavior | Medium |
| Book Behavior | Thin |
| Dump Candle Signature | Fast synthetic dump |
| Recovery Signature | Strong synthetic V |
| Notes | Flick triggered by actor cluster; repeated twice in 10 minutes |

ALLO — Synthetic Burst (5‑Minute Expansion)

| Field | Value |
| --- | --- |
| Market | ALLO |
| Date | 2026‑06‑21 |
| Time | 11:45–11:50 |
| Spike Size | 112 pts |
| Spike Type | Synthetic Burst |
| Memory Interaction | Medium tap depth |
| Structure Before | Tight coil |
| Structure After | Burst → coil reset |
| Actor Behavior | High |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Burst triggered by synthetic team; expansion lasted 5 minutes |

XPL — Natural Mid‑Spike

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Time | 10:00–10:05 |
| Spike Size | 45 pts |
| Spike Type | Natural |
| Memory Interaction | None |
| Structure Before | Loose coil |
| Structure After | Slow recovery |
| Actor Behavior | Low |
| Book Behavior | Medium |
| Dump Candle Signature | Natural dump |
| Recovery Signature | Slow |
| Notes | Natural mid‑scale spike, no synthetic involvement |

🔹 Schema Connections
Upstream:

Layer 6 — Price Spikes

Layer 6.1 — 1‑Minute Spike Tracker

Layer 4.3 — Actor Registry

Downstream:

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 7.2 — Patterns

Layer 6.2 is the mid‑scale spike‑tracking layer that bridges microstructure and macrostructure.