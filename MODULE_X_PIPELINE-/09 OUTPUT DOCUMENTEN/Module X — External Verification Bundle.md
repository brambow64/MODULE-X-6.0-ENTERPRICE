Module X — External Verification Bundle
Doel

Definieert bundel waarmee externe partijen Module X builds kunnen verifiëren.

Bundle Inhoud
final_report.json
canonical_output.json
release_manifest.json
hash_list.txt
schema_set/
audit_report.json

Bundle Eigenschappen

Bundle moet:

read-only zijn
self-contained zijn
geen runtime dependencies hebben

Externe Verificatie Taken

Externe partij moet kunnen:

hash controleren
schema valideren
determinisme check uitvoeren
chain hash controleren

Niet In Bundle

Niet toegestaan:

source secrets
unlock keys
sealed key B
interne logs

Bundle Hash

Bundle krijgt:

verification_bundle_hash
