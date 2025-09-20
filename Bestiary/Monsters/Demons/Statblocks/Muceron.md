---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '5'
file_basename: Muceron
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 0
item_id: muceron
item_index: '278'
item_name: Muceron
level: 3
might: 2
presence: 1
reason: 0
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:muceron
scdc:
- 1.1.1:2:278
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
type: statblock
name: Muceron
level: 3
roles:
  - Horde Brute
ancestry:
  - Abyssal
  - Demon
ev: "5"
stamina: "30"
weaknesses:
  - Holy 3
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 2
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Barbed Tongues
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; pull 2
        tier2: 7 damage; pull 3
        tier3: 8 damage; pull 4
      - name: Effect
        effect: If the target is pulled adjacent to the muceron, the muceron can either
          make a free strike or use the Grab maneuver against them.
  - type: feature
    feature_type: ability
    name: Tongue Pull
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Maneuver
    distance: Ranged 5
    target: Three creatures or objects
    effects:
      - name: Effect
        effect: The muceron pulls each target up to 5 squares.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the muceron is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the muceron can't be hidden from them.
~~~