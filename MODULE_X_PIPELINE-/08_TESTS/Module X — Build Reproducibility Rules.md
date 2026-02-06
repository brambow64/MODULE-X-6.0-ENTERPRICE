Module X — Build Reproducibility Rules
Doel

Elke build moet reproduceerbaar zijn.

Build Input Vastlegging

Build gebruikt alleen:

vastgelegde source files
vastgelegde dependency versies
vastgelegde config

Verboden
auto dependency upgrade
floating versions
dynamic code generation

Build Manifest Verplicht
build_id
source_hash
dependency_lock_hash
pipeline_version
sealed_provider_hash

Rebuild Test

Procedure:

rebuild from clean state


Controle:

build_hash identiek
artifact_hash identiek
