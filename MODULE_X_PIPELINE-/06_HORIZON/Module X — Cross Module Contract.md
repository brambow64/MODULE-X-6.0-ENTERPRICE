 Module X — Cross Module Contract

Status: Canonical  
Phase: 6 — Horizon Layer

---

## Doel

Legt vast hoe Horizon meerdere module-versies mag lezen.

Alleen lezen — nooit schrijven.

---

## Toegestane Invoer

Horizon mag alleen lezen:

final_report.json
canonical_output.json
layer_hash_report.json

yaml
Code kopiëren

---

## Verboden Invoer

Niet toegestaan:

interne buffers
kernel states
debug dumps
temp bestanden

yaml
Code kopiëren

---

## Contractvorm

Elke module output moet bevatten:

module_version
canonical_hash
schema_version
layer_trace

yaml
Code kopiëren

---

## Contract Schending

Bij ontbrekend veld:

hard fail
geen fallback
geen herstel

yaml
Code kopiëren

---

## Versie Onafhankelijkheid

Horizon mag:

meerdere versies tegelijk lezen
vergelijking uitvoeren
synthese berekenen

yaml
Code kopiëren

---

## Verboden Gedrag

Horizon mag nooit:

modules herconfigureren
parameters aanpassen
kern beïnvloeden

yaml
Code kopiëren

---

## Constitutionele Garantie

Cross-module toegang is read-only.
