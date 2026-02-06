# READ ONLY GATE RULES

Doel: voorkom mutatie van data tussen lagen.

Regels:
- deepcopy vóór doorgifte
- freeze structuren (dict→frozendict, list→tuple)
- na verwerking vergelijking uitvoeren
- verschil = MutationViolation
