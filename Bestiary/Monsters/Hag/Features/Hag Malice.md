---
file_basename: Hag Malice
file_dpath: Monsters/Hag/Features
item_id: hag-malice-malice-features
item_index: '41'
item_name: Hag Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:hag-malice-malice-features
scdc:
- 1.1.1:2.2:41
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Hag Malice
flavor: >-
  At the start of a hag's turn, you can spend Malice to activate one of the
  following features.


  ❇️ **Casting Curses and Bodies (3 Malice)**


  The hag utters terrible words that push each enemy within 2 squares of them up
  to 3 squares.
features:
  - type: feature
    feature_type: ability
    name: Hag Wyrd
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 10 x 1 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 fire damage; R < 1 frightened (save ends)
        tier2: 8 fire damage; R < 2 frightened (save ends)
        tier3: 11 fire damage; R < 3 frightened (save ends)
      - name: Effect
        effect: After making the power roll, the hag can choose to replace the damage
          type and condition with lightning damage and dazed, or cold damage and
          slowed.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The hag takes an additional main action on their turn. They can use this
          feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: House Call
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: The hag's hut springs to life. It enters the encounter map within 10
          squares of the hag if it isn't already there and takes its turn. The
          hut is size 4, has 75 Stamina and damage immunity 3, and has speed 8
          from its powerful set of animal legs. This feature can't be used if
          the hut is reduced to 0 Stamina. In addition to its move action, the
          house can take only the following main action.
  - type: feature
    feature_type: ability
    name: Kick
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 2 cube within 2
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 6 damage; push 3; M < 1 prone
        tier2: 10 damage; push 4; M < 2 prone
        tier3: 13 damage; push 5; M < 3 prone
~~~