🔹 Pattern Types

| Pattern | Definition |
| --- | --- |
| **Burst → Coil → Burst** | Synthetic burst followed by coil reset and another burst |
| **Dump → V → Ladder** | Synthetic dump → synthetic V → ladder climb |
| **Synthetic Flick Loop** | Repeated flicks in tight timing windows |
| **Synthetic Memory Reinforcement Cycle** | Synthetic taps reinforcing memory bands |
| **Synthetic Ignition Cycle** | Multi‑hour synthetic ignition sequence |
| **Synthetic Ceiling Migration** | Synthetic movement of ceiling boundary |


Natural Patterns

| Pattern | Definition |
| --- | --- |
| **Natural Drift Corridor** | Slow, organic drift with low actor presence |
| **Natural Spike → Slow Recovery** | Natural spike followed by slow recovery |
| **Natural Compression → Expansion** | Natural compression leading to organic expansion |
| **Natural Coil → Natural Burst** | Natural coil followed by natural burst |


Hybrid Patterns

| Pattern | Definition |
| --- | --- |
| **Synthetic Burst → Natural Drift** | Synthetic burst followed by natural drift |
| **Natural Spike → Synthetic V** | Natural spike followed by synthetic recovery |
| **Synthetic Ladder → Natural Compression** | Synthetic ladder followed by natural compression |
| **Natural Drift → Synthetic Ignition** | Natural drift corridor leading into synthetic ignition |


| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which market the pattern occurred in |
| **Pattern Type** | Synthetic / Natural / Hybrid |
| **Pattern Name** | Name of the pattern |
| **Start Time (PDT)** | When the pattern began |
| **End Time (PDT)** | When the pattern ended |
| **Duration** | Length of the pattern |
| **Actor Behavior** | Actor involvement |
| **Book Behavior** | Thick / thin / hollow |
| **Memory Interaction** | Reinforcement / violation / none |
| **Spike Interaction** | Burst / flick / ladder / dump / V |
| **Structure Before** | Engine state before the pattern |
| **Structure After** | Engine state after the pattern |
| **Notes** | Freeform structural notes |


🔹 Example Pattern Records


JTO — Synthetic Burst → Coil → Burst

| Field | Value |
| --- | --- |
| Market | JTO |
| Pattern Type | Synthetic |
| Pattern Name | Burst → Coil → Burst |
| Start Time | 14:20 |
| End Time | 14:45 |
| Duration | 25 min |
| Actor Behavior | High |
| Book Behavior | Thin → thick |
| Memory Interaction | Medium tap |
| Spike Interaction | Burst → coil → burst |
| Structure Before | Tight coil |
| Structure After | Ladder continuation |
| Notes | Classic synthetic burst cycle; actor cluster present |


ALLO — Synthetic Dump → V → Ladder


| Field | Value |
| --- | --- |
| Market | ALLO |
| Pattern Type | Synthetic |
| Pattern Name | Dump → V → Ladder |
| Start Time | 11:45 |
| End Time | 12:10 |
| Duration | 25 min |
| Actor Behavior | High |
| Book Behavior | Hollow → thick |
| Memory Interaction | Medium tap depth |
| Spike Interaction | Dump → V → ladder |
| Structure Before | Tight coil |
| Structure After | Ladder climb |
| Notes | Synthetic dump triggered by hollow book; ladder bots active |


SYND — Synthetic Flick Loop

| Field | Value |
| --- | --- |
| Market | SYND |
| Pattern Type | Synthetic |
| Pattern Name | Flick Loop |
| Start Time | 09:00 |
| End Time | 09:20 |
| Duration | 20 min |
| Actor Behavior | Medium |
| Book Behavior | Thin |
| Memory Interaction | Shallow taps |
| Spike Interaction | Repeated flicks |
| Structure Before | Tight synthetic coil |
| Structure After | Coil reset |
| Notes | Flick cluster repeated every 5 minutes |

XPL — Natural Drift Corridor

| Field | Value |
| --- | --- |
| Market | XPL |
| Pattern Type | Natural |
| Pattern Name | Drift Corridor |
| Start Time | 10:00 |
| End Time | 11:00 |
| Duration | 60 min |
| Actor Behavior | Low |
| Book Behavior | Medium |
| Memory Interaction | None |
| Spike Interaction | None |
| Structure Before | Loose coil |
| Structure After | Slow recovery |
| Notes | Natural drift corridor; no synthetic involvement |


🔹 Schema Connections
Upstream:

Layer 7.1 — Synthetic Market Tracker

Layer 6.6 — Synthetic Spikes

Layer 6.7 — Synthetic Shared Timing

Layer 4.3 — Actor Registry

Downstream:

Layer 8 — Synthetic Engine Evolution (if you build it)

Pattern‑based trading logic (if you build it)

Layer 7.2 is the pattern‑recognition engine that powers synthetic detection, macro analysis, and engine evolution.