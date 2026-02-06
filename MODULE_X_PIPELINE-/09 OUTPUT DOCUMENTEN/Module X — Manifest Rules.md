Module X — Manifest Rules
Doel

Manifest beschrijft exact welke componenten deel uitmaken van een release.

Manifest Structuur
manifest = {
  release_id
  version
  component_list[]
  component_hashes{}
  schema_versions{}
  build_hash
}

Component Lijst

Elke component entry:

name
path
hash
size
type

Volledigheid Regel

Manifest moet:

alle bestanden bevatten
geen ontbrekende entries
geen dubbele entries

Canonical Vorm

Manifest wordt:

canonical json
gesorteerde keys
vaste formatting

Manifest Hash

Manifest krijgt:

manifest_hash

Manifest Wijziging

Elke wijziging → nieuwe hash → nieuwe release id.
