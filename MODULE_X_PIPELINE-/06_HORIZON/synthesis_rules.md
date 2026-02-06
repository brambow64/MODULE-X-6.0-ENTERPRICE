Horizon Synthesis Rules
Doel

Synthesis combineert module outputs zonder interpretatie.

Toegestane operaties

Structureel:

hash vergelijking
vector samenvoeging
metriek aggregatie
grid vergelijking
laag-coherentie meting

Verboden operaties

Semantisch:

betekenis geven
signaal duiden
classificeren
labelen
conclusies trekken

Geen correctie

Synthesis mag niet:

waarden aanpassen
fouten herstellen
ruis verwijderen
scores corrigeren

Geen learning

Horizon synthesis:

geen training
geen geheugen
geen model update

Determinisme eis

Zelfde input modules → zelfde synthesis output.

Output eisen

Horizon synthesis output bevat:

horizon_hash
source_hashes[]
coherence_metrics
structure_alignment


Geen semantische velden.
