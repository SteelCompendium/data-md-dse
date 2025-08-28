---
file_basename: Hag Malice
file_dpath: Monsters/Hag/Features
item_id: hag-malice-malice-features
item_index: '35'
item_name: Hag Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:hag-malice-malice-features
scdc:
- 1.1.1:2.2:35
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Hag Malice
type: Malice Features
flavor: >-
  At the start of a hag's turn, you can spend Malice to activate one of the
  following features.


  ❇️ **Casting Curses and Bodies (3 Malice)**


  The hag utters terrible words that push each enemy within 2 squares of them up
  to 3 squares.
stats: []
features:
  - name: Hag Wyrd
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 10 x 1 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 fire damage; R < 1 frightened (save ends)
        t2: 8 fire damage; R < 2 frightened (save ends)
        t3: 11 fire damage; R < 3 frightened (save ends)
      - effect: After making the power roll, the hag can choose to replace the damage
          type and condition with lightning damage and dazed, or cold damage and
          slowed.
        name: Effect
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The hag takes an additional main action on their turn. They can use this
          feature even if they are dazed.
  - name: House Call
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: The hag's hut springs to life. It enters the encounter map within 10
          squares of the hag if it isn't already there and takes its turn. The
          hut is size 4, has 75 Stamina and damage immunity 3, and has speed 8
          from its powerful set of animal legs. This feature can't be used if
          the hut is reduced to 0 Stamina. In addition to its move action, the
          house can take only the following main action.
  - name: Kick
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 2 cube within 2
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 6 damage; push 3; M < 1 prone
        t2: 10 damage; push 4; M < 2 prone
        t3: 13 damage; push 5; M < 3 prone
~~~