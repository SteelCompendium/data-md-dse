---
file_basename: Undead Malice Level 7 Malice Features
file_dpath: Monsters/Undead/Features
include_parens_in_filename: 'true'
item_id: undead-malice-level-7-malice-features
item_index: 08
item_name: Undead Malice (Level 7+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:undead-malice-level-7-malice-features
scdc:
- 1.1.1:2.2:08
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: + Malice Features
name: Undead Malice
level: 7
flavor: At the start of any level 7 or higher undead's turn, you can spend
  Malice to activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Prior Malice Features
    icon: ⭐️
    cost: 2-7+ Malice
    effects:
      - effect: The undead activates a Malice feature available to undead of level 6 or
          lower.
  - type: feature
    feature_type: trait
    name: Necrotic Rupture
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: Until the end of the round, whenever an undead is reduced to 0 Stamina,
          they deal 8 corruption damage to each enemy within 3 squares of them.
~~~