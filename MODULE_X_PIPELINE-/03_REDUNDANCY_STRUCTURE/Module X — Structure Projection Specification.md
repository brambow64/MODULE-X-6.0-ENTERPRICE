Module X — Structure Projection Specification

Status: Canonical  
Layer: Structure Projection (Phase 3)

---

## Doel

Projecteer ruwe output naar structurele vorm zonder informatieverlies.

---

## Projectie Definitie

Projectie =

vormmapping
geometrische ordening
structurele layout

makefile
Code kopiëren

Niet:

compressie
samenvatting
reductie

yaml
Code kopiëren

---

## Toegestane Projecties

grid mapping
vector mapping
matrix vorm
tensor structuur

yaml
Code kopiëren

---

## Verboden Projecties

dimension truncation
window cropping
sample dropping

yaml
Code kopiëren

---

## Dimensie Regel

Indien perfecte vorm niet mogelijk:

padding toegestaan
truncatie verboden

yaml
Code kopiëren

---

## Structurele Metrics

Toegestaan:

rank
determinant
singular values
symmetriemetriek

yaml
Code kopiëren

Niet toegestaan:

betekenislabels
klasse labels
interpretatievelden

yaml
Code kopiëren

---

## Output Regel

Projectie output moet:

volledig
reproduceerbaar
hashbaar

yaml
Code kopiëren

zijn.

---

## Constitutionele Garantie

Projectie verandert vorm — nooit inhoud.
