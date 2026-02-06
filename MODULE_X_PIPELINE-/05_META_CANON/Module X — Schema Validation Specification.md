Module X — Schema Validation Specification

Status: Canonical  
Phase: 5 — Meta Canon Layer

---

## Doel

Borgt dat elke output exact voldoet aan het contractschema.

---

## Schema Verplichting

Elke laag output:

moet schema hebben
moet schema valideren
moet schema hash dragen

yaml
Code kopiëren

---

## Validatie Type

Alleen toegestaan:

structurele validatie
type validatie
veld aanwezigheid
shape validatie

yaml
Code kopiëren

Niet toegestaan:

semantische validatie
betekenis validatie
interpretatie

yaml
Code kopiëren

---

## Schema Eigenschappen

Schema moet vastleggen:

verplichte velden
veldtypes
array shapes
decimal format
hash velden

yaml
Code kopiëren

---

## Foutgedrag

Schema mismatch:

hard fail
geen auto-correctie
geen fallback

yaml
Code kopiëren

---

## Versie Discipline

Schema moet:

versie-id dragen
schema_hash bevatten
onveranderlijk zijn per release

yaml
Code kopiëren

---

## Constitutionele Garantie

Schema valideert vorm — niet betekenis.
