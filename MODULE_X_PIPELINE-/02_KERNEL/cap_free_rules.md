# Module X — Cap Free Flow Rules (Ultra Volledig)

Status: Bindend

## Kernregel
Geen enkele kernel- of onderlaag mag datalimieten opleggen.

## Verboden
- max_iterations
- max_samples
- buffer_caps
- truncation
- slicing caps
- clipping op lengte

## Toegestaan
- Monitoring
- Metrics
- Waarschuwingen
- Fail bij resource-uitputting

## Monitoring ≠ Limiting
Wel:
    size = len(data)

Niet:
    if size > MAX: data = data[:MAX]

## Grid Uitzondering
Alleen vormaanpassing met expliciete documentatie — geen stille datareductie.

## Audit
Codebase grep-regels:
- geen max_* caps
- geen truncate calls
- limit alleen in monitoring-context
