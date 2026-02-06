# CANONICAL OUTPUT RULES

Alle output moet deterministisch serializeerbaar zijn.
- Keys alfabetisch gesorteerd
- Decimal als string (geen exponent notatie)
- json.dumps met sort_keys en vaste separators

Canonical hash = sha256(canonical_json_string)
