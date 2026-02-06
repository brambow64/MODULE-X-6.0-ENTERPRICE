Module X — Cross Module Contract (Horizon Layer)
Doel

De Horizon-laag mag meerdere module-outputs combineren zonder:

write-back

mutatie

interpretatie

herberekening van onderliggende lagen

De Horizon werkt uitsluitend op final_report outputs.

Toegestane input

Alleen:

module_x_<version>/final_report.json


Niet toegestaan:

intermediate buffers
kernel internals
state objects
live pipeline references

Leesdiscipline

Horizon is read-only consumer:

open → read → close


Geen:

update
overwrite
append
patch

Structuurvereisten per module-output

Elke module output moet bevatten:

canonical_hash
module_version
layer_metrics
constitutional_status


Ontbreekt één veld → contract violation.

Verboden cross-module acties
gewicht toekennen
ranking
prioriteit berekenen
semantische vergelijking


Alleen structurele vergelijking toegestaan.

Determinisme eis

Zelfde module outputs → zelfde horizon result → zelfde horizon hash.
