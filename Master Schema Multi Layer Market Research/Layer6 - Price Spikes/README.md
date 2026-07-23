Layer 6 is the core spike‑system layer.
It tracks every meaningful spike event across all markets and ties it directly to:

🔹 Usage
Use Layer 6 to:

Identify synthetic vs natural spikes

Track memory band interactions

Understand actor involvement during spikes

Diagnose engine stability

Predict post‑spike behavior

Build case studies for synthetic control

Map dump → recovery signatures

Feed candle‑level spike trackers (6.1–6.4)

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
