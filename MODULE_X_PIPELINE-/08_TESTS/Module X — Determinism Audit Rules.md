Module X — Determinism Audit Rules
Doel

Controle op volledige reproduceerbaarheid.

Test Procedure

Zelfde run:

run pipeline N keer


Controle:

alle final_hash gelijk
alle layer_hash gelijk

Minimale N
N ≥ 5


Aanbevolen:

N ≥ 50

Determinisme Schending

Schending wanneer:

hash mismatch
output shape mismatch
schema mismatch

Verboden Bronnen
time()
datetime
uuid
random
os entropy
thread order afhankelijkheid
random
os entropy
thread order afhankelijkheid
