Module X — Canonical Output Rules

Status: Canonical  
Phase: 5 — Meta Canon Layer

---

## Doel

Definieert de vaste outputdiscipline voor alle Module X lagen.

Output is:

- volledig
- structureel
- deterministisch
- semantiek-vrij
- reproduceerbaar

---

## Output Vorm

Alle outputs moeten:

JSON-serialiseerbaar
key-gesorteerd
deterministisch geformatteerd
zonder optionele velden

yaml
Code kopiëren

zijn.

---

## Verboden Output Gedrag

Niet toegestaan:

samenvattingen
aggregaties die data verwijderen
heuristische reductie
interpretatieve labels
tekstuele duiding

yaml
Code kopiëren

---

## Decimal Discipline

Decimal waarden moeten:

als string worden geschreven
vaste precisie behouden
geen exponent notatie gebruiken

yaml
Code kopiëren

---

## Array Discipline

Arrays moeten:

volledig blijven
niet getrimd worden
niet gesampled worden
niet gemiddeld worden

yaml
Code kopiëren

---

## Hash Verplichting

Elke canonieke output bevat:

canonical_hash
input_hash_reference
layer_hash

yaml
Code kopiëren

---

## Key Sorting

JSON keys:

alfabetisch gesorteerd
recursief gesorteerd

yaml
Code kopiëren

---

## Determinisme Regel

Zelfde input → exact zelfde JSON string → exact zelfde hash.

---

## Constitutionele Garantie

Output toont structuur — nooit betekenis.
