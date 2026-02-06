# Module X — Cap Free Flow Rules

Status: Binding

## Kernregel

De kernel en onderliggende lagen mogen GEEN datalimieten opleggen.

Alles wat binnenkomt wordt volledig verwerkt.

---

## Verboden

Niet toegestaan:

- max_iterations
- max_samples
- buffer_limit
- truncate()
- slice caps
- clipping op lengte

---

## Toegestaan

Wel toegestaan:

- geheugenfout → fail
- monitoring metrics
- waarschuwingen
- externe orchestrator limits

---

## Monitoring vs Limiting

Toegestaan:

    size = len(data)

Niet toegestaan:

    if size > MAX: data = data[:MAX]

---

## Grid Projectie Uitzondering

Alleen toegestaan:

herstructurering zonder informatieverlies  
of expliciet gedocumenteerde vormaanpassing.

Geen stille truncatie.

---

## Audit Regel

Code moet slagen:

grep max_ → geen hits  
grep truncate → geen hits  
grep limit → alleen monitoring context

- geen max_* caps
- geen truncate calls
- limit alleen in monitoring-context
