---
file_basename: War Dog Malice Level 7 Malice Features
file_dpath: Monsters/War Dogs/Features
include_parens_in_filename: 'true'
item_id: war-dog-malice-level-7-malice-features
item_index: '61'
item_name: War Dog Malice (Level 7+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:war-dog-malice-level-7-malice-features
scdc:
- 1.1.1:2.2:61
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: War Dog Malice
type: + Malice Features
level: 7
flavor: At the start of any level 7 or higher war dog's turn, you can spend
  Malice to activate one of the following features.
stats: []
features:
  - name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The war dog activates a Malice feature available to war dogs of level 6
          or lower.
  - name: Alchemical Cloud
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: A bank of choking chemicals sweeps across the area of the encounter map.
          Each enemy in the encounter makes a Might test.
        t1: 8 poison damage; dazed (EoT)
        t2: 7 poison damage; weakened (EoT)
        t3: 4 poison damage
~~~