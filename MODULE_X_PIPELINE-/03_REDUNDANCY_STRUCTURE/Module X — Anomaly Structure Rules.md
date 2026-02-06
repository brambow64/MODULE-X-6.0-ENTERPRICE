Module X — Anomaly Structure Rules

Status: Canonical  
Layer: Redundancy / Structure (Phase 3)

---

## Doel

Definieert hoe structurele afwijkingen worden vastgesteld zonder semantische interpretatie.

Anomalie = structurele afwijking t.o.v. consensus, niet t.o.v. betekenis.

---

## Definitie Anomalie

Een anomalie is:

structurele afwijking
hash-afwijking
vorm-afwijking
consensus-breuk

makefile
Code kopiëren

Niet:

fout
probleem
diagnose
betekenis

yaml
Code kopiëren

---

## Detectiebasis

Detectie mag alleen gebaseerd zijn op:

hash verschil
vector verschil
structurele metriek
geometrische afwijking

yaml
Code kopiëren

Niet toegestaan:

semantische classificatie
domeinregels
contextinterpretatie

yaml
Code kopiëren

---

## Consensus Afwijking

Bij k-pad processing:

indien ≥1 pad afwijkt → anomaly flag

yaml
Code kopiëren

Geen herstel.
Geen correctie.
Alleen markering.

---

## Registratieregel

Anomalieën moeten:

zichtbaar blijven
niet gefilterd worden
niet overschreven worden

yaml
Code kopiëren

---

## Pipeline Regel

Anomalieën:

stromen door
worden niet verwijderd
worden niet opgelost

yaml
Code kopiëren

---

## Verboden

auto-repair
auto-correctie
semantische labeling
prioritering

yaml
Code kopiëren

---

## Constitutionele Garantie

Anomalieën blijven structureel, zichtbaar en onveranderd.
