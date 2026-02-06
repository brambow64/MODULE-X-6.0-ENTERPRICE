Module X — Temporal Determinism Rules

Status: Canonical  
Layer: Temporal (Phase 4)

---

## Doel

Borgt dat alle temporele verwerking volledig deterministisch is.

---

## Determinisme Definitie

Temporeel determinisme betekent:

zelfde input volgorde
zelfde index structuur
zelfde output

yaml
Code kopiëren

---

## Tijdbronnen — Verboden

Niet toegestaan:

system time
wall clock
timestamps
runtime clocks
datetime.now
time.time

yaml
Code kopiëren

---

## Toegestane Tijdsbasis

Alleen toegestaan:

index positie
sample volgorde
deterministische teller

yaml
Code kopiëren

---

## Multi-Run Regel

Herhaalde runs moeten:

identieke temporele metrics geven
identieke fractal waarden geven
identieke hashes geven

yaml
Code kopiëren

---

## Sampling Discipline

Toegestaan:

vaste sampling
deterministische stride
vaste segmentlengte

yaml
Code kopiëren

Niet toegestaan:

random sampling
adaptive sampling
probabilistische selectie

yaml
Code kopiëren

---

## Cache Regel

Temporele caches mogen:

performance verbeteren

yaml
Code kopiëren

maar mogen nooit:

uitkomst beïnvloeden

yaml
Code kopiëren

---

## Constitutionele Garantie

Tijd in Module X is index — geen klok.
