---
file_basename: Xorannoxs Malice
file_dpath: Monsters/Xorannox the Tyract/Features
item_id: xorannoxs-malice-malice-features
item_index: '44'
item_name: Xorannox's Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:xorannoxs-malice-malice-features
scdc:
- 1.1.1:2.2:44
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Xorannox's Malice
flavor: At the start of Xorannox's turn, you can spend Malice to activate one of
  the following features.
features:
  - type: feature
    feature_type: trait
    name: Gas Belch
    icon: ❇️
    cost: 3 Malice
    effects:
      - effect: Xorannox lets out a noxious belch. Each enemy within 2 squares of him
          who has M < 3 is weakened (save ends).
  - type: feature
    feature_type: trait
    name: Slime Trail
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Until the end of Xorannox's next turn, whenever he or any of his eyes
          leave their space, they secrete a viscous slime onto the ground in
          that area. Any enemy who enters an affected square has lightning
          weakness 5 and fire weakness 5 until the end of the encounter.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: Xorannox takes an additional main action on his turn. He can use this
          feature even if he is dazed.
  - type: feature
    feature_type: trait
    name: Mind Over Matter
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Xorannox fills the encounter map with a powerful telekinetic field. The
          Director chooses a cardinal direction (north, south, east, or west).
          Whenever a creature in the encounter willingly moves or is force
          moved, they are pulled 2 squares in the chosen direction, ignoring
          stability. Each time this feature is used, its previous effect ends.
~~~