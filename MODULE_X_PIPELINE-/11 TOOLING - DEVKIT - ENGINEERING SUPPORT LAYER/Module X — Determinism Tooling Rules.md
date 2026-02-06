Module X — Determinism Tooling Rules
Doel

Tooling voor determinisme-verificatie over meerdere runs.

Determinism Tooling Werking

Tooling voert uit:

N herhalingen
identieke input
hash vergelijking

Determinisme Check

Voor elke run:

output_hash vergelijken
trace_hash vergelijken
schema gelijkheid controleren

Fail Criteria

Determinisme faalt bij:

hash mismatch
array grootte mismatch
trace verschil

Verboden
gemiddelde nemen
resultaten samenvoegen
correctie toepassen

Output
determinism_score
run_hashes[]
match_flag
