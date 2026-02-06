# Module X — Temporal Determinism Rules

Status: Binding

## Tijdbron

Alle tijd = index-gebaseerd.

Verboden:

- wall clock
- timestamps
- systeemtijd
- externe tijd

---

## Window Selectie

Toegestaan:

- vaste vensters
- sliding windows

Niet toegestaan:

- random windows
- data-afhankelijke window selectie

---

## Schaalniveaus

Schalen moeten:

- vooraf gedefinieerd
- reproduceerbaar
- volgorde-vast zijn

---

## Sorteer Discipline

Alle schaalresultaten:

- vaste volgorde
- vaste index mapping

---

## Hash Stabiliteit

Temporal metrics moeten:

zelfde input → zelfde metrics → zelfde hash
