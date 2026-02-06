# Reproducible Build Rules

Build moet reproduceerbaar zijn.

Regels:
- vaste dependency versies
- geen system clock
- geen random
- vaste json sortering
- SOURCE_DATE_EPOCH gebruiken

Build hash = hash van alle bronbestanden.
