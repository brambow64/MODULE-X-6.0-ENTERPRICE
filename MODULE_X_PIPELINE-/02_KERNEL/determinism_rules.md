# Module X — Determinism Rules (Ultra Volledig)

Status: Canonical

## Definitie
Zelfde input → zelfde output → zelfde hash.

## Verboden Variatiebronnen
- random
- tijd
- process-id
- thread timing
- netwerk
- niet-gesorteerde structuren

## Seeds
Alleen afgeleid van input + configuratie + α.

## Determinism Gate
Minimaal 2 runs → hash vergelijking → mismatch = fout.

## Hash Basis
- Ruwe numerieke bytes
- Gesorteerde structuur
Niet:
- Tekst formatting
- Logs

## Float Discipline
Vaste dtype. Geen automatische promotie.

## Acceptatietest
Minimaal 100 runs → identieke hash verplicht.
