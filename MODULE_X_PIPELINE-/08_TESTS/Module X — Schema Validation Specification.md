Module X — Schema Validation Specification
Doel

Schema validation controleert of alle Module X outputs exact voldoen aan de vastgelegde structurele contracten.

Schema validation controleert:

veld aanwezigheid
veld type
veld volgorde (indien canoniek vereist)
numerieke vorm
hash velden
array structuur


Schema validation controleert niet:

betekenis
kwaliteit
interpretatie
domeinwaarde

Validatie Momenten

Schema validatie is verplicht bij:

layer output
module output
final_report
audit report
horizon output
release artifact

Schema Bron

Elke output verwijst naar:

schema_id
schema_version
schema_hash


Schema zelf moet gehasht en versioned zijn.

Canonical JSON Regel

Validatie gebeurt op:

canonicalized json


Niet op:

runtime dict
object memory layout
unsorted json

Verplichte Controles
Structuur
alle verplichte velden aanwezig
geen onbekende velden
geen dubbele keys

Types
hash → string
metrics → number
arrays → list
flags → boolean

Numeriek
geen NaN
geen Inf
geen exponent notatie indien verboden

Validatie Resultaat

Output:

schema_valid = true | false
schema_errors[]
schema_checked_version

Validatie Fail

Schema fail stopt:

release
audit pass
compliance pass
