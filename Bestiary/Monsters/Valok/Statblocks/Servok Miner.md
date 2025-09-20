---
agility: -2
ancestry:
- Construct
- Servok
- Soulless
- Valok
ev: '44'
file_basename: Servok Miner
file_dpath: Monsters/Valok/Statblocks
free_strike: 9
intuition: -1
item_id: servok-miner
item_index: '331'
item_name: Servok Miner
level: 9
might: 4
presence: -5
reason: -4
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:servok-miner
scdc:
- 1.1.1:2:331
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 6
stamina: '200'
type: monster
---

~~~ds-statblock
type: statblock
name: Servok Miner
level: 9
roles:
  - Elite Controller
ancestry:
  - Construct
  - Servok
  - Soulless
  - Valok
ev: "44"
stamina: "200"
speed: 5
movement: Burrow, climb
size: "2"
stability: 6
free_strike: 9
might: 4
agility: -2
reason: -4
intuition: -1
presence: -5
features:
  - type: feature
    feature_type: ability
    name: Drill Press
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 13 damage; M < 2 restrained (save ends) and prone
        tier2: 18 damage; M < 3 restrained (save ends) and prone
        tier3: 22 damage; prone; M < 4 restrained (save ends)
      - name: Effect
        effect: In suitably soft ground, a target restrained this way is etrenched in a
          1-square-deep hole.
  - type: feature
    feature_type: ability
    name: Unload Rocks
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    usage: Main action
    distance: 4 cube within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes an **Agility test**.
        tier1: 14 damage; slide 4; the miner's allies have concealment from the target
          (save ends)
        tier2: 11 damage; slide 2
        tier3: 7 damage
      - effect: The area is difficult terrain
  - type: feature
    feature_type: ability
    name: Break Ground
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 20 x 1 line within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: A 5-square-deep fissure opens along the ground in the area. Each ally in
          the area can shift into the nearest unoccupied space outside the
          fissure. Each target makes an **Agility test**.
        tier1: 14 damage; the target falls into the fissure, and is prone and can't
          stand (EoT)
        tier2: 11 damage; the target is prone and hanging onto the edge of the fissure
        tier3: 7 damage; the target can shift into the nearest unoccupied space outside
          the fissure
  - type: feature
    feature_type: ability
    name: Miner Inconvenience
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The miner is targeted by a strike.
    effects:
      - name: Effect
        effect: Until the end of the round, dust and dirt billow in a 2 burst around the
          miner's initial space. While the miner is in the area, they ignore the
          nondamaging effects of any strike made against them, including the
          triggering strike.
  - type: feature
    feature_type: trait
    name: Valiar Tunneler
    icon: ⭐️
    effects:
      - effect: The miner can burrow through stone and metal. When the miner burrows,
          they create a stable size 2 tunnel in their wake.
  - type: feature
    feature_type: trait
    name: Servok Siege Machine
    icon: ⭐️
    effects:
      - effect: The miner ignores difficult terrain, and their abilities deal an extra
          15 damage to objects.
  - type: feature
    feature_type: trait
    name: Crafted to Perfection
    icon: ⭐️
    effects:
      - effect: The miner's shape can't be changed by any external effect.
  - type: feature
    feature_type: trait
    name: Valiar Might
    icon: ⭐️
    effects:
      - effect: While the miner isn't bleeding, weakened, or winded, any power roll made
          against them is automatically a tier 1 outcome. A critical hit still
          grants its additional main action.
~~~