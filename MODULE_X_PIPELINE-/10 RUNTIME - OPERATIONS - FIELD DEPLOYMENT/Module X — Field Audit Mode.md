Module X — Field Audit Mode
Doel

Runtime audit modus voor veld-uitvoering.

Activatie

Field audit mode wordt geactiveerd via:

runtime flag
deployment config
audit profile

Gedrag

Bij field audit mode:

extra hash logging
laag trace logging
schema checks per laag

Geen Extra Semantiek

Audit mode voegt toe:

hashes
counts
flags


Niet:

diagnoses
interpretaties
labels

Audit Mode Output
field_audit_trace[]
field_audit_hash
