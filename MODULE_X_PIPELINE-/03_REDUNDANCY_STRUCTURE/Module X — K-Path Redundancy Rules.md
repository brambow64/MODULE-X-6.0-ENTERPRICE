Module X — K-Path Redundancy Rules

Status: Canonical  
Layer: Redundancy (Phase 3)

---

## Doel

Definieert redundante multi-pad uitvoering voor structurele verificatie.

---

## K-Pad Definitie

K-pad betekent:

minimaal 3 parallelle runs
onafhankelijke kernel instanties
zelfde input

yaml
Code kopiëren

---

## Minimale K Waarde

k ≥ 3 verplicht

yaml
Code kopiëren

Lagere waarden verboden.

---

## Pad Onafhankelijkheid

Elk pad moet:

eigen kernel instantie
geen gedeelde state
geen gedeelde cache

yaml
Code kopiëren

---

## Vergelijkingsbasis

Vergelijking gebeurt via:

output hash
structure vector
canonical output

yaml
Code kopiëren

---

## Consensus Regel

Consensus =

meerderheid hash gelijk

yaml
Code kopiëren

---

## Afwijkingsregel

Indien hashes verschillen:

anomaly markering
geen pad verwijdering
geen pad correctie

yaml
Code kopiëren

---

## Verboden

pad-gewicht
pad-voorkeur
pad-ranking

yaml
Code kopiëren

---

## Constitutionele Garantie

Redundantie dient verificatie — niet interpretatie.
