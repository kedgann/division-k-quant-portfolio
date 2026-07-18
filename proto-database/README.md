Layer 1 — Markets (DB Version)			
field	type	description	
market_id	string	e.g., JTO‑USD	
status	enum	active / paused / dead / experimental	
tags	array<string>	high‑cap, synthetic, vacuum‑prone	
notes	text	engine personality	
			
Layer 2 — Daily Log (DB Version)			
field	type	description	
date	date	snapshot date	
market_id	FK → Layer 1	market identity	
end_day_high	float	numeric high	
end_day_low	float	numeric low	
peak_volume_time	time	HH:MM	
volume_sequence	array<int>	compressed volume	
natural_spike_count	int	count	
synthetic_spike_count	int	count	
largest_spike_size	float	pts	
largest_synthetic_spike_size	float	pts	
actor_pressure	enum	low / medium / high	
engine_stability	enum	stable / unstable / chaotic	
			
Layer 3 — Trades (DB Version)			
field	type	description	
trade_id	string	unique	
date_time	datetime	trade timestamp	
market_id	FK	market	
quantity	float	size	
entry_price	float	numeric	
exit_price	float	numeric	
pnl	float	profit/loss	
direction	enum	buy / sell	
reason_entry	text	structural read	
reason_exit	text	exit logic	
emotional_state	enum	calm / tilted / fatigued	
structural_notes	text	engine behavior	
time_in_trade	int	seconds	
spike_events	array<string>	natural / synthetic	
actor_behavior	enum	low / medium / high	
book_behavior	enum	thick / thin / hollow	
dump_signature	text	optional	
recovery_signature	text	optional	
notes	text	freeform	
			
Layer 4 — Engine Map (DB Version)			
field	type	description	
market_id	FK	engine identity	
engine_type	enum	synthetic / natural / hybrid	
typical_spike_interval	int	seconds	
typical_spike_size	float	pts	
memory_tap_frequency	enum	low / medium / high	
memory_tap_depth	enum	shallow / medium / deep	
coil_behavior	enum	tight / loose / erratic	
actor_presence	enum	low / medium / high	
book_behavior	enum	thick / thin / hollow	
dump_signature	text	shape	
recovery_signature	text	shape	
notes	text	engine personality	
			
Layer 4.2 — Movement‑Family Behavior (DB Version)			
field	type	description	
market_id	FK	market	
family_lifespan_min	int	minutes	
branch_count	int	always 2	
sequence_count	int	always 3	
sequence_approach_min	int	minutes	
sequence_test_min	int	minutes	
sequence_resolution_min	int	minutes	
geometry_break_conditions	text	structural failures	
family_switch_conditions	text	triggers	
anchor_rules	text	anchor relevance	
inversion_markers	text	turbulence patterns	
ceiling_migration_markers	text	top‑boundary signals	
decay_repair_markers	text	controlled descent	
drift_floor_conditions	text	formation rules	
drift_floor_failure	text	failure rules	
purge_conditions	text	sweep triggers	
actor_presence_req	enum	low / medium / high	
book_state_req	enum	thick / thin / hollow	
			
Layer 4.3 — Actor Registry (DB Version)			
field	type	description	
actor_id	string	Burst / Cascade / Drift / etc.	
purpose	text	compact definition	
lane_primary	string	e.g., C‑D‑Ceiling	
lane_secondary	string	optional	
spacing_min	int	numeric	
spacing_max	int	numeric	
spacing_direction	enum	+ / – / neutral	
spacing_type	enum	expansion / collapse / compression	
conditions	text	core requirements	
families	array<string>	movement families	
			
Layer 5 — Memory Taps (DB Version)			
field	type	description	
market_id	FK	market	
date_time	datetime	tap timestamp	
frequency	enum	low / medium / high	
depth	enum	shallow / medium / deep	
tap_type	enum	natural / synthetic / actor / vacuum	
outcome	enum	hold / break / hesitation	
structure_before	enum	shelf / valley / coil / vacuum	
structure_after	enum	reinforced / weakened / broken	
actor_reaction	enum	increase / decrease / neutral	
engine_reaction	enum	stabilize / destabilize / accelerate	
notes	text	freeform	
			
Layer 6 — Price Spikes (DB Version)			
field	type	description	
market_id	FK	market	
date_time	datetime	spike timestamp	
direction	enum	up / down	
cause	enum	actor / vacuum / synthetic / natural	
structure_before	enum	coil / drift / hollow	
structure_after	enum	reinforced / broken	
notes	text	freeform	
			
Layers 6.1–6.4 — Candle Trackers (DB Version)			
field	type		
market_id	FK		
date_time	datetime		
open	float		
high	float		
low	float		
close	float		
notes	text		
			
Layer 6.5 — Liquidation Events (DB Version)			
field	type		
market_id	FK		
date_time	datetime		
liquidation_side	enum		
liquidation_size	float		
cluster_density	enum		
liquidation_type	enum		
cascade_depth	int		
engine_reaction	enum		
actor_reaction	enum		
book_reaction	enum		
spike_interaction	enum		
synthetic_interaction	enum		
recovery_time_sec	int		
follow_through_strength	enum		
pre_structure	enum		
post_structure	enum		
notes	text		
			
Layer 6.6 — Synthetic Spike Behavior (DB Version)			
field	type		
market_id	FK		
date_time	datetime		
spike_size	float		
spike_pattern	enum		
engine_reaction	enum		
actor_reaction	enum		
notes	text		
			
Layer 6.8 — Synthetic Shared Timing-Layer 6.8			
field	type	description	
id	PK	Unique row ID	
market_id	FK	Links to your Market table (Layer 1)	
date	date	Spike event date	
time	time	Spike event time	
start_price	float	Price at start of spike	
price_spike_count	int	Number of spikes in the event window	
largest_spike_size	float	Largest spike magnitude	
peak_price	float	Highest price reached	
price_dumps	text	Notes on dump events during/after spike	
pre_ignition_notes	text	Notes on possible pre‑ignition behavior	
actor_notes	text	Actor behavior observed	
movement_sync	boolean	YES/NO — whether movement synced with other markets	
notes	text	Additional notes	
			
			
Layer 6.9  — Flat spike markets tracker			
Field	Type	Purpose	
market_id	FK	Links to Layer 1 Markets	
date	date	Spike date	
time	time	Spike time	
start_price	float	Price before spike	
peak_price	float	Highest price reached	
movement_type	text	Burst / Cascade / Actor‑Driven / Synthetic	
total_run_length	int	Duration of spike	
notes	text	General notes	
events_before	text	Pre‑spike events	
extra_notes	text	Additional observations	
			
Layer 7 — Pattern Recognition (DB Version)			
field	type		
market_id	FK		
pattern_name	string		
conditions	text		
behavior	text		
outcome	text		
notes	text		
screenshot_ref	string		
