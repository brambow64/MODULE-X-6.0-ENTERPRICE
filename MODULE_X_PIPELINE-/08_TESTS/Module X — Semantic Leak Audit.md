Module X — Semantic Leak Audit
Doel

Detecteert ongewenste semantische inhoud in outputs, logs en schema velden.

Module X is structureel — niet interpretatief.

Audit Domeinen

Controleert:

json outputs
audit reports
logs
metadata velden
horizon outputs

Verboden Woorden (indicatie set)
meaning
interpretation
significance
diagnosis
label
classification
insight
understanding
conclusion

Verboden Structuren
"label": ...
"type": "signal_type"
"class": ...
"meaning": ...

Toegestane Structuurwoorden
metric
hash
index
value
vector
grid
layer
trace

Controle Methode

Audit voert:

string scan
field name scan
schema field compare

Audit Output
semantic_leak_detected = true | false
violating_fields[]
violating_strings[]

Audit Fail Gedrag

Bij semantic leak:

compliance = FAIL
release = BLOCK
audit = FAIL
