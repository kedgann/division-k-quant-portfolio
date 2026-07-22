Purpose
Layer 4 defines the engine profile for each market.
It is the first “deep structure” layer in your system — the point where markets stop being tickers and start being engines.

This layer captures:

Engine type (Synthetic / Natural / Hybrid)

Typical spike interval

Typical spike size

Memory tap frequency & depth

Coil behavior

Actor presence

Book behavior

Dump candle signature

Recovery signature

Freeform engine personality notes

Layer 4 is the fingerprint of each market’s engine.


| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which engine this profile belongs to |
| **Engine Type** | Synthetic / Natural / Hybrid |
| **Typical Spike Interval** | Time between spikes (compressed read) |
| **Typical Spike Size** | Average spike magnitude |
| **Memory Tap Frequency** | How often memory bands get tested |
| **Memory Tap Depth** | How deep the retests go |
| **Coil Behavior** | Tight / loose / erratic |
| **Actor Presence** | Low / medium / high |
| **Book Behavior** | Thick / thin / hollow |
| **Dump Candle Signature** | Shape, speed, depth of dumps |
| **Recovery Signature** | V‑shape, slow, synthetic, etc. |
| **Notes** | Freeform engine personality notes |


| Field | Value |
| --- | --- |
| Engine Type | Synthetic |
| Typical Spike Interval | 45–90 sec |
| Typical Spike Size | 40–70 pts |
| Memory Tap Frequency | High |
| Memory Tap Depth | Medium |
| Coil Behavior | Tight → sudden release |
| Actor Presence | High |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Fast synthetic dumps |
| Recovery Signature | Strong synthetic V‑recoveries |
| Notes | Engine feels managed by a team |


| Field | Value |
| --- | --- |
| Engine Type | Synthetic |
| Typical Spike Interval | 45 sec |
| Typical Spike Size | 268–330 pts |
| Memory Tap Frequency | High |
| Memory Tap Depth | Medium |
| Coil Behavior | Tight → 4‑hour windows |
| Actor Presence | High |
| Book Behavior | Thin → thick |
| Dump Candle Signature | Fast synthetic dumps |
| Recovery Signature | Strong synthetic V‑recoveries |
| Notes | 4 ALLO bid stacks clear books well |


| Field | Value |
| --- | --- |
| Engine Type | Synthetic |
| Typical Spike Size | 191 pts |
| Notes | (Fill in additional fields as needed) |


Use Layer 4 to:

Identify engine personality before deeper analysis

Compare synthetic vs natural engines

Predict spike rhythm and memory behavior

Understand actor involvement

Map book thickness and dump/recovery signatures

Build case studies for engine evolution

This layer is the foundation for movement families, actor behavior, memory taps, and spike systems.