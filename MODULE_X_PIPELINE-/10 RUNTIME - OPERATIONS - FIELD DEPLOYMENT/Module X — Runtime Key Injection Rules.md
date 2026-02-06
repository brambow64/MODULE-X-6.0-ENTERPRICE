Module X — Runtime Key Injection Rules
Doel

Definieert hoe unlock keys (Key B) in runtime mogen worden aangeboden.

Toegestane Methoden
environment variable
secure memory injection
license loader
secure enclave

Verboden Methoden
hardcoded in code
config file plaintext
command line argument
log output

Key Lifetime

Key mag bestaan:

alleen runtime memory
niet op disk
niet in logs

Key Gebruik

Key wordt gebruikt voor:

sealed constant unlock
license derivation
provider activation

Key Audit

Runtime logt:

key_present = true/false
key_source_type


Niet de key zelf.
