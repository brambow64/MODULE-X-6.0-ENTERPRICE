Module X — Compliance Rules
Doel

Compliance regels definiëren wat een Module X implementatie moet volgen om geldig te zijn.

Verplichte Regels
Alpha Discipline
alpha alleen via sealed provider
geen literals
geen config alpha
geen override

Determinisme
zelfde input → zelfde hash
geen random
geen tijdsbron
geen netwerkinput

Layer Discipline
geen lower layer mutatie
geen write-back
geen cross-laag shortcuts

Hash Discipline
sha256 verplicht
canonical json hashing
chain hashing verplicht

Schema Discipline
alle outputs schema-valide
geen vrije velden
geen extra semantiek velden

Compliance Status

Elke build krijgt:

compliance_status = PASS | FAIL

Compliance Rapport

Bevat:

rule_set_version
checks_total
checks_passed
violations
compliance_hash
