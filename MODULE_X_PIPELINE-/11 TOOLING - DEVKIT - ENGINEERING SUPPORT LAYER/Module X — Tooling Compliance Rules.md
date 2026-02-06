Module X — Tooling Compliance Rules
Doel

Zorgt dat tooling zelf compliant is.

Tooling Compliance Checks
deterministisch gedrag
read-only werking
geen semantiek
geen kernel write

Tooling Mag Niet
kern muteren
sealed provider vervangen
constants injecteren
runtime beïnvloeden

Tooling Audit

Elke tool moet leveren:

tool_hash
tool_version
compliance_flag

Tooling Gate

Niet-compliant tooling:

mag niet in pipeline
mag niet in audit
mag niet in release
