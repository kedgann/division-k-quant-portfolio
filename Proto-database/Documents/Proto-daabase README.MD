Division‑K Proto‑Database
A relational SQL database for structural market‑engine research.

The Division‑K Proto‑Database is a fully structured relational system designed to store, analyze, and query synthetic‑engine behavior, actor fingerprints, spike clusters, timing sync, candle‑tracking, liquidation events, and pattern ontologies. It supports the 20‑Layer Structural Trading Schema and serves as the foundation for future Division‑K trading tools, dashboards, and research automation.

NOTE: The Proto‑Database is currently in active development, with several layers fully implemented and others in progress. It is designed for continuous expansion as Division‑K research evolves.

Purpose
This database provides a unified architecture for:

Reverse‑engineering synthetic market engines.
Classifying actor behavior and fingerprints.

Tracking spike clusters and ignition patterns.

Detecting shared timing across markets.

Modeling liquidation cycles and structural collapses.

Recording multi‑timeframe candle behavior.

Building pattern ontologies and structural triggers.

Supporting high‑frequency structural trading research.

It is designed for scalability, clarity, and integration with the Division‑K Master Schema.

| Schema Layer | SQL Table | Description |
| --- | --- | --- |
| Layer 1 | ``markets`` | Market identity, tags, engine personality |
| Layer 2 | ``daily_logs`` | Daily structural snapshots |
| Layer 3 | ``trades`` | High‑frequency structural trades |
| Layer 4 | ``engine_map`` | Engine mechanics & actor pressure |
| Layer 4.2 | ``movement_family`` | Movement‑family behavior rules |
| Layer 4.3 | ``actor_registry`` | Actor fingerprints & spacing rules |
| Layer 5 | ``memory_taps`` | Memory‑band interactions |
| Layer 6 | ``price_spikes`` | Natural & synthetic spike events |
| Layer 6.1–6.4 | ``candle_*`` | Multi‑timeframe candle tracking |
| Layer 6.5 | ``liquidation_events`` | Liquidation clusters & reactions |
| Layer 6.6 | ``synthetic_spikes`` | Synthetic spike behavior |
| Layer 6.7 | ``synthetic_shared_timing`` | Multi‑market timing sync |
| Layer 6.9 | ``flat_spike_markets`` | Flat‑spike market behavior |
| Layer 7 | ``patterns`` | Pattern ontology & structural triggers |