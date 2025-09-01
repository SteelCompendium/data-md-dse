---
file_basename: Demon Malice Level 7 Malice Features
file_dpath: Monsters/Demons/Features
include_parens_in_filename: 'true'
item_id: demon-malice-level-7-malice-features
item_index: '38'
item_name: Demon Malice (Level 7+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:demon-malice-level-7-malice-features
scdc:
- 1.1.1:2.2:38
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Demon Malice
type: + Malice Features
level: 7
flavor: At the start of any level 7 or higher demon's turn, you can spend Malice
  to activate one of the following features.
stats: []
features:
  - name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The demon activates a Malice feature available to demons of level 6 or
          lower.
  - name: Seeping Blight
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: One demon acting this turn expels blight-digested soul juice onto the
          ground around them in a 3 burst that lingers until the start of their
          next turn. Any enemy who enters the area or starts their turn there
          takes 6 corruption damage, and has a double bane on power rolls until
          the start of their next turn.
~~~