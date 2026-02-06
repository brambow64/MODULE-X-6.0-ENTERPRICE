Schema Validation — Canon Discipline
Doel

Controle dat output structuur exact voldoet aan contract.

Niet inhoud — alleen vorm.

Validatie controleert

verplichte velden aanwezig

datatype correct

nesting correct

array shapes aanwezig

hash velden aanwezig

Valideert NIET

betekenis

waarde-interpretatie

signaaltype

patroonklasse

Voorbeeld schema checks
required:
  consensus_hash
  agreement_metrics
  module_version

types:
  consensus_hash: string
  k: integer

Schema engine mag

fail geven

rapporteren

blokkeren bij ontbrekende velden

Schema engine mag niet:

data aanpassen

defaults invullen

waarden corrigeren

✅ Resultaat

Deze vijf bestaan nu volledig opnieuw:

meta_layer_spec.docx
canonical_output_rules.md
flow_monitoring_spec.md
read_only_gate_rules.md
schema_validation_spec.md
