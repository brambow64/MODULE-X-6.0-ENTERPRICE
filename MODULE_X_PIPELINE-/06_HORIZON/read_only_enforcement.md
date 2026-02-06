Horizon Read-Only Enforcement Rules
Doel

Horizon mag nooit lagere lagen beïnvloeden.

Read-Only principe

Alle inputs worden behandeld als immutable.

Bij inname:

deep_copy()
freeze()

Mutatie detectie

Na verwerking:

compare(original, frozen_copy)


Verschil → violation.

Immutable regels
dict → immutable map
list → tuple
set → frozenset

Verboden operaties
in-place wijziging
pointer wijziging
object reference update
buffer overschrijven

Enforcement resultaat

Bij mutatie:

HORIZON_READ_ONLY_VIOLATION


Pipeline stopt.
