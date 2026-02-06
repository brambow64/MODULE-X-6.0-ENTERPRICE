Module X — Release Hash Specification
Doel

Definieert hoe release hashes worden berekend.

Release Hash Scope

Release hash omvat:

alle release bestanden
manifest
schema set
audit rapporten

Hash Methode
sha256
canonical ordering
byte exact

Hash Volgorde

Bestanden worden gehasht in:

gesorteerde pad volgorde

Hash Input Vorm

Voor elke file:

path + file_hash


Wordt samengevoegd tot:

release_hash_input


Daarover:

sha256

Release Hash Veld
release_hash


verplicht in:

release manifest
verification bundle
OEM package descriptor

Hash Stabiliteit

Zelfde release inhoud → zelfde release hash.
