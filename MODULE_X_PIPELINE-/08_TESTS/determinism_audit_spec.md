# Determinism Audit Spec

Regel: Zelfde input → zelfde output hash.

Procedure:
- Run pipeline 100×
- Verzamel canonical_hash
- Set grootte moet = 1 zijn

Verboden:
- random
- time
- uuid
- unordered serialization

Verplicht:
- canonical json
- vaste decimal precisie
- sort_keys=True
