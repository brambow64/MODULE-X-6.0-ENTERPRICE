Module X — Core Protection Rules
Doel

Definieert de beschermingsregels voor de Module X kern.

De kern omvat:

sealed constant provider
kernel lagen
determinism gates
hash discipline
constitutional contracts

Kern Toegang

Kern mag alleen benaderd worden via:

publieke interfaces
sealed adapters
contract APIs


Niet toegestaan:

direct file access
reflection
introspection op private velden
monkey patching
runtime override

Kern Mutatie Verbod

Verboden:

core file wijziging
constant wijziging
provider wijziging
kernel formule wijziging

Integriteitscontrole

Elke core component moet hebben:

component_hash
version_id
build_origin

Core Tamper Detectie

Tamper wordt aangenomen bij:

hash mismatch
sealed blob mismatch
provider self-check fail


Resultaat:

core_invalid = true
pipeline stop

OEM Regel

OEM integraties:

mogen kern niet aanpassen
alleen wrapper lagen toegestaan
