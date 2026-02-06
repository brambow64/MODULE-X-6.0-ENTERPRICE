Module X — Fractal Metrics Specification

Status: Canonical  
Layer: Temporal / Fractal (Phase 4)

---

## Doel

Definieert toegestane fractale en temporele structuurmetingen binnen Module X.

Metingen zijn structureel — nooit semantisch.

---

## Fractale Metrics — Toegestaan

Alleen structurele metrics:

lacunarity
hurst exponent
scale variance
self-similarity ratio
multi-scale density

yaml
Code kopiëren

---

## Niet Toegestaan

betekenis interpretatie
domein classificatie
trend labeling
context duiding

yaml
Code kopiëren

---

## Tijdsdefinitie

Tijd binnen Module X is:

index-gebaseerd
volgorde-gebaseerd
structureel

yaml
Code kopiëren

Niet toegestaan:

wall clock
systeem tijd
real-world timestamps

yaml
Code kopiëren

---

## Multi-Scale Analyse

Multi-scale analyse moet:

deterministisch zijn
zelfde input → zelfde schaalresultaat
geen random sampling

yaml
Code kopiëren

---

## Windowing Regels

Toegestaan:

vaste vensters
deterministische segmentatie
index slicing

makefile
Code kopiëren

Verboden:

adaptieve vensters
data-afhankelijke venstergrootte
heuristische splitsing

yaml
Code kopiëren

---

## Output Discipline

Fractale metrics moeten:

numeriek
reproduceerbaar
hashbaar
volledig

yaml
Code kopiëren

zijn.

---

## Constitutionele Garantie

Fractale analyse onthult structuur — nooit betekenis.
