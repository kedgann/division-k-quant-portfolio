🔹 Flat Spike Types

| **Flat Type** | **Definition** |
| --- | --- |
| **True Flat** | No spikes of any kind |
| **Synthetic Suppressed** | Synthetic engine intentionally muted |
| **Natural Drift** | Natural engine stuck in drift corridor |
| **Compression Flat** | Tight compression preventing spikes |
| **Actor‑Absent Flat** | No actor presence → no spikes |
| **Book‑Thick Flat** | Thick book prevents spike formation |
| **Pre‑Ignition Flat** | Engine silent before ignition cycle |

| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which market is flat |
| **Date** | When the flat window occurred |
| **Flat Type** | True / Suppressed / Drift / Compression / Actor‑Absent / Thick‑Book / Pre‑Ignition |
| **Spike Count** | Number of spikes in the window |
| **Synthetic Spike Count** | Number of synthetic spikes |
| **Actor Presence** | Low / none |
| **Book Behavior** | Thick / medium / thin |
| **Drift Corridor** | Whether drift corridor is active |
| **Compression Level** | Tight / medium / loose |
| **Memory Interaction** | None / shallow taps |
| **Notes** | Freeform structural notes |


Example Flat Spike Records


| Field | Value |
| --- | --- |
| Market | JTO |
| Date | 2026‑06‑20 |
| Flat Type | Synthetic Suppressed |
| Spike Count | 0 |
| Synthetic Spike Count | 0 |
| Actor Presence | Low |
| Book Behavior | Thick |
| Drift Corridor | Active |
| Compression Level | Tight |
| Memory Interaction | None |
| Notes | Synthetic engine intentionally muted; pre‑ignition window forming |

SYND — True Flat

| Field | Value |
| --- | --- |
| Market | SYND |
| Date | 2026‑06‑20 |
| Flat Type | True Flat |
| Spike Count | 0 |
| Synthetic Spike Count | 0 |
| Actor Presence | None |
| Book Behavior | Thick |
| Drift Corridor | Active |
| Compression Level | Medium |
| Memory Interaction | None |
| Notes | No synthetic or natural spikes; engine fully silent |

ALLO — Compression Flat

| Field | Value |
| --- | --- |
| Market | ALLO |
| Date | 2026‑06‑21 |
| Flat Type | Compression Flat |
| Spike Count | 0 |
| Synthetic Spike Count | 0 |
| Actor Presence | Low |
| Book Behavior | Thick |
| Drift Corridor | Active |
| Compression Level | Tight |
| Memory Interaction | Shallow taps |
| Notes | Tight compression prevented synthetic bursts |

XPL — Natural Drift Flat

| Field | Value |
| --- | --- |
| Market | XPL |
| Date | 2026‑06‑22 |
| Flat Type | Natural Drift |
| Spike Count | 0 |
| Synthetic Spike Count | 0 |
| Actor Presence | Low |
| Book Behavior | Medium |
| Drift Corridor | Active |
| Compression Level | Loose |
| Memory Interaction | None |
| Notes | Natural drift corridor; no synthetic involvement |