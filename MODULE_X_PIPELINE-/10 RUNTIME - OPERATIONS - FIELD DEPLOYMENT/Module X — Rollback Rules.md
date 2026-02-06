Module X — Rollback Rules
Doel

Definieert rollback gedrag bij falende deploy of runtime.

Rollback Trigger
runtime fail
compliance fail
audit fail
hash break

Rollback Scope

Rollback mag:

versie rollback
package rollback
config rollback


Rollback mag niet:

data herschrijven
output aanpassen
hash wijzigen

Rollback Vereisten

Rollback versie moet hebben:

release_hash
manifest_hash
compliance_pass

Rollback Log
rollback_id
from_version
to_version
rollback_hash
