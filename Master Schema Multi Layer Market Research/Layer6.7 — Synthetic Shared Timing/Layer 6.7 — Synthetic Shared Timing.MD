🔹 Shared Timing Types


| **Timing Type** | **Definition** |
| --- | --- |
| **Synchronized Burst Window** | Multiple markets fire synthetic bursts within the same minute |
| **Shared Flick Cluster** | Multiple markets flick within a tight timing window |
| **Cross‑Market Ladder Climb** | Ladder bots climb shelves across markets simultaneously |
| **Synthetic Dump Window** | Multiple markets dump at the same time |
| **Synthetic V‑Recovery Window** | Multiple markets recover in synchronized V‑shape |
| **Ignition Cycle Alignment** | Multi‑hour ignition cycles begin across markets together |
| **Memory Reinforcement Sync** | Synthetic taps occur across markets at the same time |



| **Column** | **Purpose** |
| --- | --- |
| **Timestamp (PDT)** | Exact timing window |
| **Markets Involved** | Markets that fired synthetic events |
| **Synthetic Type** | Burst / Flick / Ladder / Dump / V / Reinforcement |
| **Spike Sizes** | Magnitude per market |
| **Actor Timing** | Actor cluster involvement |
| **Book Behavior** | Thick / thin / hollow per market |
| **Memory Interaction** | Reinforcement / violation |
| **Structure Before** | Engine state before the timing window |
| **Structure After** | Engine state after the timing window |
| **Notes** | Freeform structural notes |



Example Shared Timing Records

JTO + ALLO — Synchronized Synthetic Burst Window

| Field | Value |
| --- | --- |
| Timestamp | 2026‑06‑20 14:32 |
| Markets Involved | JTO, ALLO |
| Synthetic Type | Burst |
| Spike Sizes | JTO: 65 pts, ALLO: 330 pts |
| Actor Timing | High actor presence in both markets |
| Book Behavior | Thin → thick (both) |
| Memory Interaction | Medium tap (both) |
| Structure Before | Tight coil → ladder setup |
| Structure After | Burst → coil reset (both) |
| Notes | Synthetic team fired coordinated bursts across engines |


SYND + JTO + XPL — Shared Flick Cluster


| Field | Value |
| --- | --- |
| Timestamp | 2026‑06‑20 09:15 |
| Markets Involved | SYND, JTO, XPL |
| Synthetic Type | Flick |
| Spike Sizes | 55 pts, 42 pts, 18 pts |
| Actor Timing | Medium cluster |
| Book Behavior | Thin (SYND), thin (JTO), medium (XPL) |
| Memory Interaction | Shallow taps |
| Structure Before | Tight synthetic coil |
| Structure After | Flick → coil reset |
| Notes | Flick cluster repeated twice in 10 minutes across markets |


ALLO + JTO — Synthetic Dump → Synthetic V Window

| Field | Value |
| --- | --- |
| Timestamp | 2026‑06‑21 11:50 |
| Markets Involved | ALLO, JTO |
| Synthetic Type | Dump → V |
| Spike Sizes | ALLO: 330 pts, JTO: 65 pts |
| Actor Timing | High |
| Book Behavior | Hollow → thick |
| Memory Interaction | Medium tap depth |
| Structure Before | Tight coil |
| Structure After | Synthetic V |
| Notes | Synthetic dump triggered across markets simultaneously |

XPL + SYND — Ignition Cycle Alignment

| Field | Value |
| --- | --- |
| Timestamp | 2026‑06‑22 10:00 |
| Markets Involved | XPL, SYND |
| Synthetic Type | Ignition Cycle |
| Spike Sizes | 120 pts, 95 pts |
| Actor Timing | Medium |
| Book Behavior | Medium → thick |
| Memory Interaction | None |
| Structure Before | Loose coil |
| Structure After | Multi‑hour ignition cycle |
| Notes | Ignition cycles aligned across markets; synthetic timing cluster present |


Schema Connections
Upstream:

Layer 6 — Price Spikes

Layer 6.6 — Synthetic Spikes

Layer 4.3 — Actor Registry

Downstream:

Layer 7.1 — Synthetic Market Tracker

Layer 7.2 — Patterns

Layer 6.7 is the synthetic coordination layer that powers cross‑market pattern detection.