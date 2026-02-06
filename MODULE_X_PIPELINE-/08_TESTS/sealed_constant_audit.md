# Sealed Constant Audit

Controle:
1. Geen literal α in codebase
2. Alleen toegang via alpha_adapter
3. Provider import self-check actief

Scan:
grep -r "137.035999" .
Moet nul hits geven buiten provider.
