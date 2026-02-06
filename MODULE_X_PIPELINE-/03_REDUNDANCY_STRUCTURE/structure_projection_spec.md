# Module X — Structure Projection Specification

Status: Canonical

## Doel

Numerieke outputs projecteren naar structurele vormen
zonder informatieverlies en zonder semantiek.

---

## Basisregel

Projectie = herordening  
Niet = reductie

---

## Grid Projectie

Array → N×N grid waar mogelijk.

Als geen perfect vierkant:

toegestaan:
- expliciete reshape strategie
- remainder apart rapporteren

niet toegestaan:
- stille truncatie

---

## Structure Metrics

Toegestaan:

- row sums
- column sums
- rank
- singular values
- determinant (waar mogelijk)

Niet toegestaan:

- patroonlabels
- classificatie

---

## Determinisme

Projectie moet:

zelfde input → zelfde grid

geen random padding

---

## Output

Moet bevatten:

grid_dimensions  
checksums  
structure_metrics  
anomaly_coordinates (structureel)

