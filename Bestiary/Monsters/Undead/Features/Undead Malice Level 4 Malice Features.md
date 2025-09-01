---
file_basename: Undead Malice Level 4 Malice Features
file_dpath: Monsters/Undead/Features
include_parens_in_filename: 'true'
item_id: undead-malice-level-4-malice-features
item_index: '06'
item_name: Undead Malice (Level 4+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:undead-malice-level-4-malice-features
scdc:
- 1.1.1:2.2:06
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Undead Malice
type: + Malice Features
level: 4
flavor: At the start of any level 4 or higher undead's turn, you can spend
  Malice to activate one of the following features.
stats: []
features:
  - name: Prior Malice Features
    icon: ⭐️
    cost: 2-7+ Malice
    effects:
      - effect: The undead activates a Malice feature available to undead of level 3 or
          lower.
  - name: Blood Hunger
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: One undead acting this turn uses a signature ability against a creature
          who is bleeding. As a free triggered action, each undead within 5
          squares of the first undead moves up to their speed and can make a
          free strike against the same target.
~~~