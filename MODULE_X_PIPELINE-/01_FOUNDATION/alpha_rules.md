# Module X — Alpha Usage Rules

Status: Binding  
Scope: Alle lagen

---

## 1. Enige Toegang

α mag alleen verkregen worden via:

    get_alpha()

of

    resolve_alpha()

Geen andere routes toegestaan.

---

## 2. Verboden

Niet toegestaan:

- α als literal in code
- α in config bestanden
- α in environment behalve unlock key
- α in logs
- α in error messages
- α in test fixtures
- α in comments met volledige waarde

---

## 3. Representatie

Intern:

- Decimal

Berekening:

- float toegestaan
- alleen na gedocumenteerde downcast

Opslag:

- nooit float-only

---

## 4. Precisie Discipline

- Decimal context vooraf gezet
- geen automatische rounding
- geen exponent notatie in output
- vaste string formatting

---

## 5. Audit Regel

Elke downcast:

    Decimal → float

moet:

- expliciet
- gelogd (structureel)
- reproduceerbaar

---

## 6. Test Regel

Codebase moet slagen:

    grep "137." → GEEN hits

(behalve in sealed generator tool)

---

## 7. Pipeline Regel

Alle lagen ontvangen α via dependency — nooit hardcoded.

---

Einde regels.
