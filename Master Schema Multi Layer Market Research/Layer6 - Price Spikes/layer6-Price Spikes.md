
Includes:

Spike logs

Spike type classification

Memory interaction notes

Actor & book reaction notes

Dump & recovery signatures

Structural notes


Navigation
Jump to related layers:

Layer 4 — Engine Map

Layer 4.3 — Actor Registry

Layer 5 — Memory Taps

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.2 — 5‑Minute Spike Tracker

Layer 6.3 — 15‑Minute Spike Tracker

Layer 6.4 — 1‑Hour Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 6.8 — Flat Spike Markets


| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which engine the spike occurred in |
| **Date** | When the spike happened |
| **Time** | Exact timestamp |
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



Example Spike Records

JTO — Synthetic Spike (Memory Reinforcement)

| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Time | 14:32 |
| Spike Size | 65 pts |
| Spike Type | Synthetic |
| Memory Interaction | Reinforced memory band |
| Structure Before | Tight synthetic coil |
| Structure After | Synthetic V‑recovery |
| Actor Behavior | High actor presence |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Fast synthetic dump |
| Recovery Signature | Strong synthetic V |
| Notes | Synthetic team reinforced memory band |


ALLO — Synthetic Spike (Burst)

| Field | Value |
| --- | --- |
| Market | ALLO |
| Date | 2026‑06‑21 |
| Time | 09:15 |
| Spike Size | 330 pts |
| Spike Type | Synthetic Burst |
| Memory Interaction | Medium tap depth |
| Structure Before | Tight coil |
| Structure After | Burst → coil reset |
| Actor Behavior | High |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Burst triggered by actor cluster |

XPL — Natural Spike

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Time | 11:50 |
| Spike Size | 180 pts |
| Spike Type | Natural |
| Memory Interaction | Shallow tap |
| Structure Before | Loose coil |
| Structure After | Slow recovery |
| Actor Behavior | Low |
| Book Behavior | Medium |
| Dump Candle Signature | Natural dump |
| Recovery Signature | Slow |
| Notes | Natural spike, no synthetic involvement |


Schema Connections
Upstream:

Layer 5 — Memory Taps

Layer 4.3 — Actor Registry

Downstream:

Layer 6.1 — 1‑Minute Spike Tracker

Layer 6.2 — 5‑Minute Spike Tracker

Layer 6.3 — 15‑Minute Spike Tracker

Layer 6.4 — 1‑Hour Spike Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 6.8 — Flat Spike Markets

Layer 7.2 — Patterns

Layer 6 is the core spike‑logic layer that powers all deeper structural analysis.