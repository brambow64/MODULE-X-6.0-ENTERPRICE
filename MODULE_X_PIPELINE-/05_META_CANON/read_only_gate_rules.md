Read-Only Gate — Discipline Layer
Doel

Voorkomt dat hogere lagen lagere data muteren.

Werking

Bij binnenkomst:

deep_copy(input)
freeze(copy)


Na verwerking:

compare(original, copy)
if changed → violation

Freeze regels

Dict → immutable mapping
List → tuple
Set → frozenset

Verboden

in-place update

pointer mutatie

reference write-back

object side-effects

Detectie

Mutatie = pipeline breach
