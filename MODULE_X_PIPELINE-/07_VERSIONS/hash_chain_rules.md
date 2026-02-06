# HASH CHAIN REGELS — PIPELINE

Definitie:
Elke laag levert een hash.
De pipeline hash is de concatenatie‑hash van alle layer hashes.

Formule:

H_total = SHA256(H1 + H2 + H3 + ... + Hn)

Eigenschappen:
- Elke laag beïnvloedt eindhash
- Geen verborgen mutatie mogelijk
- Volledig auditbaar

Verboden:
- Random salt
- Timestamp input
- Volgorde variatie