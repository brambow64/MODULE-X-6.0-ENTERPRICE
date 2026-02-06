Canonical Output Rules — Module X
Doel

Alle outputs boven META-laag moeten canoniek reproduceerbaar zijn.

Zelfde input → exact zelfde JSON string → exact zelfde hash.

Canonical JSON Regels
Keys

alfabetisch gesorteerd

case-stabiel

geen dynamische key-namen

Numerieke waarden

Decimal → string

geen exponent notatie

vaste precisie

geen afronding shortcuts

JSON serialisatie
json.dumps(
  obj,
  sort_keys=True,
  separators=(",",":")
)

Verboden

pretty print

whitespace formatting

runtime timestamp velden

locale formatting

Canonical hash input

Hash wordt berekend over:

canonical_json_string


Niet over object. Niet over dict. Alleen over canonical string.
