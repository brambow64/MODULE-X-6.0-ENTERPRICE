# Module X — Structure Projection Specification

Status: Canonical

## Doel
Numerieke data projecteren naar structurele vormen zonder informatieverlies.

## Regel
Projectie = herordening, geen reductie.

## Grid
Array → N×N waar mogelijk.
Geen stille truncatie.

## Metrics
Toegestaan:
- row/column sums
- rank
- singular values

Niet toegestaan:
- patroonlabels

## Determinisme
Zelfde input → zelfde projectie.
