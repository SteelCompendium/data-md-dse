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
type: featureblock
featureblock_type: Malice Features
name: Giant Malice
flavor: At the start of any giant's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: ability
    name: Hurl Landscape
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: A giant unearths a structure, hazard, or chunk of the encounter map and
          launches it to fill the area. Each target makes an **Agility test**.
        tier1: 18 damage; prone and can't stand (save ends)
        tier2: 14 damage; prone
        tier3: 9 damage
  - type: feature
    feature_type: trait
    name: Bellow
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: Each giant in the encounter takes a deep breath and yells, pushing each
          creature within 3 squares of them up to 10 squares. A creature who can
          be pushed by more than one giant is pushed by one giant of your
          choice.
  - type: feature
    feature_type: trait
    name: Titanic Tear
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: A giant creates a fissure along the ground, either in a 15 x 2 line
          within 1 or a 10 x 3 line within 2, and that opens up to a depth of 6
          squares. Each giant in the area can shift into the nearest unoccupied
          space outside the fissure. Each non-giant in the area makes an
          **Agility test**.
        tier1: 10 damage; the target falls into the fissure, and is prone and can't
          stand (EoT)
        tier2: 10 damage; the target is prone and hanging onto the edge of the fissure
        tier3: The target can shift into the nearest unoccupied space outside the
          fissure.
~~~