# Module X — Alpha Usage Rules

Status: Binding

## Enige Toegang
Alpha alleen via get_alpha() of resolve_alpha().

## Verboden
- Geen alpha literal in code
- Niet in config
- Niet in logs
- Niet in exceptions
- Niet in testdata

## Representatie
- Intern: Decimal
- Float alleen na expliciete downcast

## Precisie
- Vaste Decimal context
- Geen exponent notatie

## Audit
Decimal → float conversie moet expliciet en reproduceerbaar zijn.
