# Module X — k-Path Redundancy Rules

Status: Binding

## Minimum

k ≥ 3 verplicht.

k = 1 → geen redundantie  
k = 2 → geen consensus mogelijk

---

## k Groei

k mag groeien zonder architectuurwijziging.

Consensuslogica mag niet afhangen van exact k.

---

## Pad Onafhankelijkheid

Elke pad-run:

- nieuwe kernel instantie
- geen gedeelde mutable state
- geen gedeelde buffers

---

## Toegestane Variatie

Pads mogen verschillen in:

- floating rounding
- numerieke drift

Niet in:

- algoritme
- configuratie
- α bron

---

## Niet Toegestaan

- pad-specifieke heuristiek
- adaptive pad weighting
- pad learning

---

## Consensus is Niet Correctie

Consensus mag nooit:

- waarden aanpassen
- waarden vervangen
- waarden middelen

Alleen rapporteren.
