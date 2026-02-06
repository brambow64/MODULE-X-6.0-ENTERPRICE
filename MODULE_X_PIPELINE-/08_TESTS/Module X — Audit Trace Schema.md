Module X — Audit Trace Schema
Doel

Definieert structuur van audit trace records.

Audit Trace Structuur
audit_trace = [
  {
    step_index
    layer_id
    layer_hash
    parent_hash
    check_id
    check_result
  }
]

Toegestane Velden
ids
hashes
booleans
counts
schema versions

Niet Toegestaan
diagnose tekst
interpretatie
betekenis labels

Trace Hash

Elke audit trace krijgt:

audit_trace_hash

build_hash identiek
artifact_hash identiek
