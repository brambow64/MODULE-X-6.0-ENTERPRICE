Horizon Hash Discipline
Doel

Horizon-resultaten moeten canoniek gehasht worden.

Hash is:

deterministisch

reproduceerbaar

canonical-string gebaseerd

Hash input

Hash wordt berekend over:

canonical_horizon_json


Niet over:

dict object
memory object
runtime structure

Canonicalisatie vóór hash

Verplicht:

keys gesorteerd

decimal als string

vaste precisie

geen timestamps

geen runtime id’s

Verboden in hash input
tijd
random id
uuid
hostname
process id

Hash algoritme
SHA-256


Geen varianten per run.

Hash veld
horizon_hash


Moet aanwezig zijn in elke horizon output.
