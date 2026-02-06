Module X — Cap-Free Kernel Rules

Status: Canonical  
Layer: Kernel (Phase 2)  
Scope: Kernel execution only

---

## Doel

Definieert het absolute verbod op flow-beperkingen binnen de kernel van Module X.

De kernel is een open pijplijn zonder interne afkapping.

---

## Cap-Free Definitie

Cap-free betekent:

geen vaste limieten
geen verborgen afkapping
geen stilzwijgende truncatie

yaml
Code kopiëren

---

## Verboden Mechanismen

Niet toegestaan in kernelcode:

max_iterations
max_steps
buffer limits
hard-coded array sizes
windowing truncation
sliding cutoffs

yaml
Code kopiëren

---

## Data Flow Regel

Input → Output moet zijn:

1-op-1 qua lengte
structureel behouden
volledig doorgegeven

yaml
Code kopiëren

De kernel mag **geen data verwijderen**.

---

## Normalisatie Regel

Toegestaan:

structurele transformaties
rekenkundige projecties
deterministische normalisatie

yaml
Code kopiëren

Niet toegestaan:

clipping
saturatie
threshold discard
lossy compression

yaml
Code kopiëren

---

## Performance vs Discipline

Performance optimalisatie mag:

vectorisatie
FFT
caching

markdown
Code kopiëren

Maar **nooit**:

data inkorten
waarden afkappen
informatie weggooien

yaml
Code kopiëren

---

## Monitoring Regel

De kernel mag:

meten
rapporteren
loggen (structureel)

markdown
Code kopiëren

Maar **niet**:

ingrijpen
corrigeren
afbreken

yaml
Code kopiëren

---

## Failure Regel

Indien resources onvoldoende zijn:

kernel faalt hard
geen gedeeltelijke output
geen fallback pad

yaml
Code kopiëren

---

## Constitutionele Garantie

De kernel:

is open-ended
is schaalbaar
is cap-vrij
is voorspelbaar
