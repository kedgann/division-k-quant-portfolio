Layer 6.7 — Synthetic Shared Timing
Cross‑Market Timing Windows, Coordinated Synthetic Behavior & Engine Synchronization

🔹 Purpose
Layer 6.6 is the synthetic spike detection layer — the part of your system that identifies:

synthetic bursts

synthetic flicks

synthetic ladders

synthetic timing clusters

synthetic memory reinforcement

synthetic dump → synthetic V sequences

synthetic ceiling migrations

synthetic coil resets

synthetic pre‑ignition windows

This layer is the core of your synthetic‑engine detection framework.


🔹 Example Synthetic Spike Records

JTO — Synthetic Ladder Burst

| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Time | 14:32 |
| Synthetic Type | Ladder Burst |
| Spike Size | 65 pts |
| Memory Interaction | Medium tap |
| Actor Timing | High actor presence |
| Book Behavior | Thin → thick |
| Structure Before | Tight coil |
| Structure After | Ladder continuation |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Ladder bot climbed 3 shelves; synthetic timing cluster present |

SYND — Synthetic Flick Cluster

| Field | Value |
| --- | --- |
| Market | SYND |
| Date | 2026‑06‑20 |
| Time | 09:15 |
| Synthetic Type | Flick |
| Spike Size | 55 pts |
| Memory Interaction | Shallow tap |
| Actor Timing | Medium |
| Book Behavior | Thin |
| Structure Before | Tight synthetic coil |
| Structure After | Flick → coil reset |
| Dump Candle Signature | Fast synthetic dump |
| Recovery Signature | Strong synthetic V |
| Notes | Flick triggered by actor cluster; repeated twice in 10 minutes |


ALLO — Synthetic Burst Reinforcement

| Field | Value |
| --- | --- |
| Market | ALLO |
| Date | 2026‑06‑21 |
| Time | 11:50 |
| Synthetic Type | Burst |
| Spike Size | 330 pts |
| Memory Interaction | Medium tap depth |
| Actor Timing | High |
| Book Behavior | Thin → thick |
| Structure Before | Tight coil |
| Structure After | Burst → coil reset |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Synthetic team reinforced memory band; burst triggered by actor cluster |

XPL — Synthetic Dump → Synthetic V

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Time | 10:05 |
| Synthetic Type | Dump → V |
| Spike Size | 48 pts |
| Memory Interaction | None |
| Actor Timing | Medium |
| Book Behavior | Hollow → thick |
| Structure Before | Loose coil |
| Structure After | Synthetic V |
| Dump Candle Signature | Synthetic dump |
| Recovery Signature | Synthetic V |
| Notes | Synthetic dump triggered by hollow book; actor cluster present |

🔹 Schema Connections
Upstream:

Layer 6 — Price Spikes

Layer 6.1–6.4 — Candle Spike Trackers

Layer 4.3 — Actor Registry

Downstream:

Layer 6.7 — Synthetic Shared Timing

Layer 7.2 — Patterns

Layer 6.6 is the synthetic‑behavior logic layer that powers timing analysis and pattern formation.


🔹 Navigation
Jump to related layers:

Layer 6 — Price Spikes

Layer 6.1–6.4 — Candle Spike Trackers

Layer 6.5 — Liquidation Events

Layer 6.7 — Synthetic Shared Timing

Layer 4.3 — Actor Registry

Layer 7.2 — Patterns