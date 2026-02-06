Flow Monitoring — Meta Layer
Doel

Flow monitoring meet doorvoer zonder beperking.

Monitoren ≠ limiteren

Toegestaan

Meten:

input grootte

output grootte

doorlooptijd per laag

cumulatieve doorvoer

buffer grootte

Verboden
if size > limit: truncate ❌
if load high: drop data ❌
if slow: sample ❌

Backpressure

Backpressure mag:

gemeten worden

gelogd worden

gerapporteerd worden

Backpressure mag niet:

data blokkeren

data verwijderen

data verkorten

Output velden
flow_metrics:
  processed_count
  batch_size
  layer_time
  total_throughput
