---
file_basename: Human Malice
file_dpath: Monsters/Humans/Features
item_id: human-malice-malice-features
item_index: '21'
item_name: Human Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:human-malice-malice-features
scdc:
- 1.1.1:2.2:21
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Human Malice
flavor: At the start of any human's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: ability
    name: Alchemical Device
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 3 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 corruption damage; A < 0 slowed (save ends)
        tier2: 6 corruption damage; A < 1 slowed (save ends)
        tier3: 9 corruption damage; A < 2 restrained (save ends)
      - name: Special
        effect: This ability can't be used by a minion.
  - type: feature
    feature_type: trait
    name: Exploit Opening
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each human acting this turn gains an edge on abilities until the end of
          their turn, or has a double edge on any ability that targets an enemy
          affected by a condition.
  - type: feature
    feature_type: trait
    name: Staying Power
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Each non-minion human in the encounter regains Stamina equal to 5 times
          their level.
~~~