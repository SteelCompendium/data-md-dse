---
file_basename: Giant Malice
file_dpath: Monsters/Giants/Features
item_id: giant-malice-malice-features
item_index: '24'
item_name: Giant Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:giant-malice-malice-features
scdc:
- 1.1.1:2.2:24
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Giant Malice
type: Malice Features
flavor: At the start of any giant's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Hurl Landscape
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: A giant unearths a structure, hazard, or chunk of the encounter map and
          launches it to fill the area. Each target makes an **Agility test**.
        t1: 18 damage; prone and can't stand (save ends)
        t2: 14 damage; prone
        t3: 9 damage
  - name: Bellow
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: Each giant in the encounter takes a deep breath and yells, pushing each
          creature within 3 squares of them up to 10 squares. A creature who can
          be pushed by more than one giant is pushed by one giant of your
          choice.
  - name: Titanic Tear
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: A giant creates a fissure along the ground, either in a 15 x 2 line
          within 1 or a 10 x 3 line within 2, and that opens up to a depth of 6
          squares. Each giant in the area can shift into the nearest unoccupied
          space outside the fissure. Each non-giant in the area makes an
          **Agility test**.
        t1: 10 damage; the target falls into the fissure, and is prone and can't stand
          (EoT)
        t2: 10 damage; the target is prone and hanging onto the edge of the fissure
        t3: The target can shift into the nearest unoccupied space outside the fissure.
~~~