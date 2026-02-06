Module X — Horizon Hash Discipline

Status: Canonical  
Phase: 6 — Horizon Layer

---

## Doel

Definieert de hash-discipline voor Horizon-laag synthese.

Horizon mag alleen werken op reeds canoniek gehashte module-outputs.

---

## Horizon Hash Basis

Horizon hash mag alleen opgebouwd worden uit:

module_output_hashes
canonical_layer_hashes
schema_hashes
version_ids

yaml
Code kopiëren

Niet toegestaan:

ruwe data
interne buffers
tussenstaten

yaml
Code kopiëren

---

## Hash Samenstelling

Horizon hash =

HASH(
sorted(module_hash_list)

horizon_skill_id

skill_version
)

yaml
Code kopiëren

---

## Sorteerregel

Alle hash inputs:

alfabetisch gesorteerd
deterministische volgorde
geen runtime volgorde

yaml
Code kopiëren

---

## Verboden Bronnen

Niet toegestaan:

timestamps
runtime counters
machine id
environment data

yaml
Code kopiëren

---

## Multi-Run Regel

Zelfde module outputs → zelfde horizon hash.

Altijd.

---

## Constitutionele Garantie

Horizon hash bewijst structuur — niet betekenis.

Moet aanwezig zijn in elke horizon output.
