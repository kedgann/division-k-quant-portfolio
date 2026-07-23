Layer 6.5 — Liquidation Events
Forced Exits, Cascade Behavior, Synthetic Liquidation Triggers & Structural Impact

Includes:

Full liquidation logs

Macro cycle windows

Cascade depth notes

Actor & book reaction notes

Spike interactions

Recovery signatures

Structural notes



Example Liquidation Event Records


JTO — Synthetic Long Liquidation Cascade

| Field | Value |
| --- | --- |
| Market | JTO |
| Long/Short Liquidation | Long |
| Liquidation Size | Medium |
| Cluster Density | High |
| Event Count | 4 |
| Cascade Depth | Deep (3‑lane inheritance) |
| Engine Reaction | Synthetic dump → synthetic V |
| Actor Reaction | High actor presence |
| Book Reaction | Hollow → thin → thick |
| Spike Interaction | Synthetic burst → synthetic ladder |
| Recovery Time | Fast (synthetic V) |
| Follow‑Through Strength | Strong |
| Notes | Forced long liquidation triggered by synthetic timing cluster |


STG — Synthetic Short Liquidation Chain

| Field | Value |
| --- | --- |
| Market | STG |
| Long/Short Liquidation | Short |
| Liquidation Size | Large |
| Cluster Density | Medium |
| Event Count | 3 |
| Cascade Depth | Medium |
| Engine Reaction | Synthetic dump → coil reset |
| Actor Reaction | Medium |
| Book Reaction | Thin |
| Spike Interaction | Synthetic flick |
| Recovery Time | Medium |
| Follow‑Through Strength | Medium |
| Notes | Synthetic short liquidation triggered by actor cluster imbalance |

XPL — Natural Long Liquidation

| Field | Value |
| --- | --- |
| Market | XPL |
| Long/Short Liquidation | Long |
| Liquidation Size | Small |
| Cluster Density | Low |
| Event Count | 1 |
| Cascade Depth | Shallow |
| Engine Reaction | Natural dump → slow recovery |
| Actor Reaction | Low |
| Book Reaction | Medium |
| Spike Interaction | Natural spike |
| Recovery Time | Slow |
| Follow‑Through Strength | Weak |
| Notes | Natural liquidation; no synthetic involvement |

🔹 Schema Connections
Upstream:

Layer 6 — Price Spikes

Layer 6.1–6.4 — Candle Spike Trackers

Layer 4.3 — Actor Registry

Downstream:

Layer 7.2 — Patterns

Layer 4.2 — Movement‑Family Behavior

Layer 6.5 is the forced‑move logic layer that powers macro‑cycle analysis and pattern formation.


🔹 Navigation
Jump to related layers:

Layer 6 — Price Spikes

Layer 6.1–6.4 — Candle Spike Trackers

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 4.2 — Movement‑Family Behavior

Layer 7.2 — Patterns