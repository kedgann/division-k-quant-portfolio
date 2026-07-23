
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


Example Engine Profiles

JTO — Synthetic Engine

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

ALLO — Synthetic Engine

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


TIA‑USD — Synthetic Engine

| Field | Value |
| --- | --- |
| Engine Type | Synthetic |
| Typical Spike Size | ~191 pts |
| Memory Tap Frequency | Medium |
| Memory Tap Depth | Medium |
| Coil Behavior | Tight |
| Actor Presence | Medium |
| Book Behavior | Thin |
| Dump Candle Signature | Synthetic dump → fast recovery |
| Recovery Signature | Synthetic V‑shape |
| Notes | Engine shows consistent synthetic spike rhythm |

Schema Connections
Upstream
Layer 1 — Markets

Layer 2 — Daily Logs

Downstream
Layer 4.2 — Movement‑Family Behavior

Layer 4.3 — Actor Registry

Layer 5 — Memory Taps

Layer 6 — Spike System

Layer 7 — Synthetic Market Tracker

Layer 8 — Engine Evolution