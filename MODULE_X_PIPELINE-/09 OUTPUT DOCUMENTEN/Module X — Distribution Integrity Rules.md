Module X — Distribution Integrity Rules
Doel

Waarborgt integriteit van distributie-artefacten.

Distributie Targets
release packages
OEM bundles
runtime bundles
audit bundles
verification bundles

Verplichte Bestanden

Elke distributie bevat:

manifest.json
release_hash.txt
component_hashes.json
schema_versions.json

Hash Vereiste

Alle distributie bestanden:

sha256 gehasht

Integriteitscontrole Bij Installatie

Installatieproces moet:

alle hashes verifiëren
manifest vergelijken
bestandentelling controleren

Distributie Fail

Fail wanneer:

bestand ontbreekt
extra bestand aanwezig
hash mismatch
manifest mismatch

Transport Onafhankelijk

Integriteit moet gelijk blijven bij:

zip
tar
installer
OEM package
