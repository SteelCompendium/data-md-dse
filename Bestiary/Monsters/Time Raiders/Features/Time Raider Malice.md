---
file_basename: Time Raider Malice
file_dpath: Monsters/Time Raiders/Features
item_id: time-raider-malice-malice-features
item_index: '19'
item_name: Time Raider Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:time-raider-malice-malice-features
scdc:
- 1.1.1:2.2:19
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Time Raider Malice
type: Malice Features
flavor: At the start of any time raider's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Gravity Well
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Psionic
      - Ranged
      - Weapon
    type: Maneuver
    distance: 5 cube within 3
    target: Special
    effects:
      - effect: A time raider acting this turn activates a gravity well in the area. The
          gravity well sits at the center of the cube and lasts until the end of
          the encounter, or until a creature adjacent to the well uses a
          maneuver to deactivate it. The area is difficult terrain for enemies.
          Any enemy who ends their turn in the area is pulled up to 4 squares
          toward the well.
        name: Effect
  - name: Recall Module
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Until the end of the round, each time raider gains a +3 bonus to speed,
          and can teleport up to their speed as a move action.
  - name: Psi-Cage
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: All time raiders in the encounter collectively create a psionic field
          over the encounter map, which lasts until the first time raider with
          the highest Stamina maximum drops to 0 Stamina or chooses to end the
          field (no action required). While the field is up, each non-time
          raider on the map makes a **Reason test** against this psionic effect
          at the start of each round.
        t1: 10 psychic damage; slowed (EoT)
        t2: 7 psychic damage; slowed (EoT)
        t3: No effect.
~~~