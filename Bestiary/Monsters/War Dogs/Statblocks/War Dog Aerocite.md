---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Aerocite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 3
item_id: war-dog-aerocite
item_index: '368'
item_name: War Dog Aerocite
level: 8
might: 0
presence: 1
reason: 1
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:war-dog-aerocite
scdc:
- 1.1.1:2:368
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '50'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Aerocite
level: 8
roles:
  - Horde Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "50"
speed: 8
movement: Fly
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 4
reason: 1
intuition: 3
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Dive Bomb
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage
        tier2: 10 damage; vertical slide 2
        tier3: 12 damage; vertical slide 3
      - cost: 1 Malice
        effect: An enemy force moved by this ability is grabbed instead.
  - type: feature
    feature_type: ability
    name: Caustic Paste Bomb
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 3 cube within 5
    target: Each creature or object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 2 acid damage; M < 2 slowed (save ends)
        tier2: 4 acid damage; M < 3 slowed (save ends)
        tier3: 6 acid damage; M < 4 slowed (save ends)
      - name: Effect
        effect: The area is difficult terrain.
  - type: feature
    feature_type: trait
    name: Jetwing Agility
    icon: ⭐️
    effects:
      - effect: If the aerocite moves 5 or more squares on their turn, strikes made
          against them take a bane until the start of their next turn.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the aerocite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
~~~