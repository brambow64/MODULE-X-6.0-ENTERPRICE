Module X — Pipeline Trace Rules
Doel

Pipeline trace registreert laagdoorloop zonder interpretatie.

Trace Principe

Elke laag voegt toe:

layer_id
layer_hash
parent_hash
processing_step_index

Trace Is Lineair
trace = [L1, L2, L3, L4 …]


Geen vertakkingen.

Verboden Trace Data
betekenis
labels
classificatie
diagnose

Toegestane Trace Data
hashes
ids
schema versions
sizes
shapes
counts

Trace Opslag

Trace mag:

naast output
in metadata
in audit record


Niet:

input muteren
laag output wijzigen

Trace Hash

Trace krijgt eigen hash:

trace_hash


Gebaseerd op:

gehele trace lijst canonical
