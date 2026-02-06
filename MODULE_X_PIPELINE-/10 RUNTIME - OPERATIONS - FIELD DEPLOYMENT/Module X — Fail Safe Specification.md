Module X — Fail Safe Specification
Doel

Definieert gedrag bij runtime fouten.

Fail Safe Principe

Bij structurele fout:

stop pipeline
geen gedeeltelijke output
geen stille correctie

Fail Safe Triggers
hash mismatch
schema fail
sealed provider fail
determinism fail
read-only violation

Fail Safe Gedrag
abort execution
emit fail_code
emit fail_hash

Verboden Fail Safe Gedrag
auto herstel
data aanpassen
fallback berekening
alternatieve interpretatie

Fail Safe Output
runtime_status = FAIL
fail_stage
fail_hash
