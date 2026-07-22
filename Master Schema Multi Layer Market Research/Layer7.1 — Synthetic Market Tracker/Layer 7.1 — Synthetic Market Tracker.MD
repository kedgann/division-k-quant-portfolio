Synthetic Market Classification

| **Type** | **Definition** |
| --- | --- |
| **Synthetic** | Engine dominated by artificial bursts, flicks, ladders, dumps, V‑recoveries |
| **Natural** | Engine dominated by organic movement, natural spikes, slow recoveries |
| **Hybrid** | Engine shows both synthetic and natural behavior |


| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which market is being tracked |
| **Engine Type** | Synthetic / Natural / Hybrid |
| **Synthetic Activity Level** | None / Low / Medium / High / Extreme |
| **Synthetic Spike Count** | Number of synthetic spikes in the window |
| **Synthetic Burst Count** | Number of synthetic bursts |
| **Synthetic Ladder Count** | Number of ladder climbs |
| **Synthetic Flick Count** | Number of flicks |
| **Synthetic Dump → V Count** | Number of dump → V sequences |
| **Synthetic Memory Reinforcement** | Yes / No |
| **Shared Timing Participation** | Yes / No |
| **Suppression Windows** | Yes / No |
| **Notes** | Freeform structural notes |


Example Synthetic Market Records

JTO — High Synthetic Activity

| Field | Value |
| --- | --- |
| Market | JTO |
| Engine Type | Synthetic |
| Synthetic Activity Level | High |
| Synthetic Spike Count | 14 |
| Synthetic Burst Count | 6 |
| Synthetic Ladder Count | 4 |
| Synthetic Flick Count | 3 |
| Synthetic Dump → V Count | 2 |
| Synthetic Memory Reinforcement | Yes |
| Shared Timing Participation | Yes |
| Suppression Windows | No |
| Notes | Strong synthetic engine; participates in cross‑market timing clusters |


ALLO — Extreme Synthetic Activity

| Field | Value |
| --- | --- |
| Market | ALLO |
| Engine Type | Synthetic |
| Synthetic Activity Level | Extreme |
| Synthetic Spike Count | 22 |
| Synthetic Burst Count | 10 |
| Synthetic Ladder Count | 6 |
| Synthetic Flick Count | 4 |
| Synthetic Dump → V Count | 3 |
| Synthetic Memory Reinforcement | Yes |
| Shared Timing Participation | Yes |
| Suppression Windows | No |
| Notes | ALLO shows extreme synthetic bursts; major synthetic engine |

SYND — Medium Synthetic Activity

| Field | Value |
| --- | --- |
| Market | SYND |
| Engine Type | Hybrid |
| Synthetic Activity Level | Medium |
| Synthetic Spike Count | 8 |
| Synthetic Burst Count | 3 |
| Synthetic Ladder Count | 2 |
| Synthetic Flick Count | 3 |
| Synthetic Dump → V Count | 1 |
| Synthetic Memory Reinforcement | Yes |
| Shared Timing Participation | Yes |
| Suppression Windows | Yes |
| Notes | Hybrid engine; synthetic suppression windows present |

XPL — Natural Engine

| Field | Value |
| --- | --- |
| Market | XPL |
| Engine Type | Natural |
| Synthetic Activity Level | Low |
| Synthetic Spike Count | 1 |
| Synthetic Burst Count | 0 |
| Synthetic Ladder Count | 0 |
| Synthetic Flick Count | 1 |
| Synthetic Dump → V Count | 0 |
| Synthetic Memory Reinforcement | No |
| Shared Timing Participation | No |
| Suppression Windows | No |
| Notes | Natural engine; minimal synthetic behavior |

🔹 Schema Connections
Upstream:

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 6.8 — Flat Spike Markets

Layer 4.3 — Actor Registry

Downstream:

Layer 7.2 — Patterns

Layer 8 — Synthetic Engine Evolution (if you build it later)

Layer 7.1 is the macro synthetic dashboard that powers pattern recognition and engine evolution analysis.