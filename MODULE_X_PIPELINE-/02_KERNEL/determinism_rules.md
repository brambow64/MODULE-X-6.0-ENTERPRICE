# Module X — Determinism Rules

Status: Canonical

## Definitie

Determinisme betekent:

zelfde input → zelfde output → zelfde hash

Altijd.

---

## Verboden Bronnen van Variatie

Niet toegestaan:

- random
- np.random zonder vaste seed afgeleid van input
- time.time
- datetime.now
- process id
- thread timing
- unordered dict iteration

---

## Toegestane Seeds

Seed mag alleen afhangen van:

- input data
- α
- configuratie

Niet van runtime omgeving.

---

## Determinism Gate

Elke kernel moet testbaar zijn via:

2× run → hash vergelijken

Bij mismatch:

DeterminismViolation

---

## Hash Regel

Hash moet gebaseerd zijn op:

- ruwe numerieke output
- byte representatie
- gesorteerde structuur

Niet op:

- geformatteerde tekst
- logs
- metadata strings

---

## Float Discipline

Float afronding is toegestaan  
mits dtype vast staat.

precision = config gestuurd  
geen automatische promotie.

---

## Test Regel

Minimaal:

100 runs → zelfde hash

vereist voor acceptatie.
