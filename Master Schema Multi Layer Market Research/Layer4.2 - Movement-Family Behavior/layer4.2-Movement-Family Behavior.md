
Full movement‑family schema

Band ranges

Lanes A → D

Ceiling & drift floor definitions

Live market tracker examples (JTO, KITE‑USD)

Corridor logic

Sequence timing

Geometry rules



| **Column** | **Purpose** |
| --- | --- |
| **Market** | Which market this family applies to |
| **Active Family Lifespan (min)** | How long the current family remains valid before geometry breaks |
| **Branch Count** | Always 2: continuation or failure |
| **Sequence Count** | Always 3: Approach → Test → Resolution |
| **Sequence Timing** | Duration of each phase |
| **Geometry‑Break Conditions** | Structural failures that invalidate the family |
| **Family‑Switch Conditions** | Triggers that move the engine into the next family |
| **Anchor Relevance Rules** | Which highs/lows matter to the current family |
| **Inversion Turbulence Markers** | Deep taps, chaotic spacing, instability signals |
| **Ceiling Migration Markers** | Signals that the top boundary is shifting upward |
| **Decay Repair Markers** | Controlled descent patterns after ceiling migration |
| **Drift Floor Formation Conditions** | Requirements for a true drift floor |
| **Drift Floor Failure Conditions** | Signals drift floor cannot form |
| **Purge‑Style Sweep Conditions** | When the engine clears stacked lows/highs |
| **Actor‑Presence Requirements** | Minimum actor involvement needed |
| **Book‑State Requirements** | Required book thickness/hollowness |


Example Movement‑Family Profiles
These examples show recruiters you understand engine geometry, not just price.

UNI — Stable Long‑Cycle Family (95 minutes)

| Field | Value |
| --- | --- |
| Active Family Lifespan | 75 min |
| Branch Count | Continuation / Failure |
| Sequence Count | Approach → Test → Resolution |
| Sequence Timing | 18m / 9m / 48m |
| Geometry‑Break Conditions | Burst inheritance failure, spacing collapse, symmetry fracture |
| Family‑Switch Conditions | Ceiling‑test rejection, drift‑floor failure, anchor invalidation |
| Anchor Rules | Only anchors formed after inversion are relevant |
| Inversion Markers | Deep uneven taps (7774–7789), chaotic spacing |
| Ceiling Migration | 794.5 → 796.4 → 798.3 → 800.4 → 803.1 |
| Decay Repair | Shallow controlled descent (791.3 → 786.6) |
| Drift Floor Formation | Requires symmetry + muted decay + 2 taps (not present) |
| Drift Floor Failure | Inversion active, burst inheritance present |
| Purge Conditions | Clears stacked lows (7774 cluster) |
| Actor Requirements | Medium presence needed for ceiling migration |
| Book Requirements | Hollow → thin during turbulence; medium during repair |


XPL — Short, Unstable Family (55 minutes)

| Field | Value |
| --- | --- |
| Lifespan | 55 min |
| Branch Count | Burst‑Continuation / Burst‑Failure |
| Sequence Timing | 15m / 7m / 33m |
| Geometry‑Break | Burst inheritance break, amplitude collapse |
| Family‑Switch | Burst‑failure → inversion → ceiling re‑approach |
| Anchor Rules | Only current‑family anchors matter |
| Inversion Markers | Strong turbulence, chaotic spacing |
| Ceiling Migration | Frequent, aggressive |
| Decay Repair | Fast, aggressive |
| Drift Floor Formation | Almost impossible |
| Drift Floor Failure | Burst amplitude present + actor absence |
| Purge Conditions | Common (clears stacked lows) |
| Actor Requirements | Low‑medium (bot‑driven) |
| Book Requirements | Hollow → thin → hollow |

Band & Lane Structure


JTO — Motion‑Space Stack (Example)


| **Layer / Segment** | **Range** | **Function / Behavior** | **Burst Likelihood** |
| --- | --- | --- | --- |
| Ceiling | 0.7908–0.7924 | Hard rejection zone | High |
| Lane D | 0.7850–0.7900 | Upper‑range bursts → ceiling tests | High |
| Lane C | 0.7800–0.7850 | High‑velocity cascades | Very High |
| Lane B | 0.7760–0.7800 | Mid‑range continuation | Medium |
| Lane A | 0.7720–0.7760 | Drift → expansion | Medium–High |
| Drift Floor | 0.7720–0.7733 | Passive equilibrium | Low |
