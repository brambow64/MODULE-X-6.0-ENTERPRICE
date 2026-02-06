Module X — Hash Chain Rules
Doel

Alle versies en lagen moeten gekoppeld zijn via hash chain discipline.

Hash Chain Principe

Elke laag output bevat:

self_hash
parent_hash
chain_hash

Definitie
self_hash = hash(current_layer_output)
chain_hash = hash(parent_hash + self_hash)

Verboden
hash overschrijven
hash herberekenen met andere regels
hash skippen

Parent Hash Bron

Parent hash komt uit:

direct vorige laag


Niet:

opnieuw berekend
samengevoegd
gemiddeld

Version Hash

Elke version map heeft:

version_root_hash


Gebaseerd op:

alle layer chain_hash waarden

Hash Algoritme
SHA-256


Altijd hetzelfde.

Hash Canonicalisatie

Hash wordt altijd berekend over:

canonical json string


Niet over:

memory object
dict object
runtime object
