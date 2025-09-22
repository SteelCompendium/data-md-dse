---
agility: 2
ancestry:
- Beast
- Griffon
ev: '16'
file_basename: Griffon
file_dpath: Monsters/Griffons/Statblocks
free_strike: 5
intuition: 1
item_id: griffon
item_index: '87'
item_name: Griffon
level: 2
might: 2
presence: 2
reason: -1
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:griffon
scdc:
- 1.1.1:2:87
size: '2'
source: mcdm.monsters.v1
speed: 9
stability: 2
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Griffon
level: 2
roles:
  - Elite Mount
ancestry:
  - Beast
  - Griffon
ev: "16"
stamina: "80"
speed: 9
movement: Fly
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 2
reason: -1
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Claw Swipes
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; the griffon can shift 1 square
        tier2: 10 damage; the griffon shifts up to 2 squares
        tier3: 13 damage; the griffon shifts up to 3 squares
      - name: Effect
        effect: If this ability is used as part of the Charge main action, the griffon
          can grab one of the targets.
  - type: feature
    feature_type: ability
    name: Crack the Earth
    icon: 🔳
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 3 cube within 8
    target: Each enemy in the area
    effects:
      - name: Special
        effect: The griffon must be flying and must have a creature or object grabbed.
      - name: Effect
        effect: The griffon flies up to half their speed toward the ground, then sends
          the creature or object they've grabbed hurtling down. The creature or
          object hits the ground to turn the area into an impact crater, and
          takes falling damage that can't be reduced in any way.
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage; A < 1 push 3
        tier3: 9 damage; A < 2 push 4; prone
  - type: feature
    feature_type: ability
    name: Wing Buffet
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 4 x 2 line within 1
    target: Each creature or object in the area
    effects:
      - name: Special
        effect: A target object must be size 2 or smaller.
      - roll: Power Roll + 2
        tier1: Push 3; A < 0 the forced movement is vertical
        tier2: Push 4; A < 1 the forced movement is vertical
        tier3: Push 5; A < 2 the forced movement is vertical
  - type: feature
    feature_type: ability
    name: Zephyr Feint
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The griffon takes damage.
    effects:
      - name: Effect
        effect: The griffon halves the damage, ignores any nondamaging effects
          associated with it, and shifts up to 2 squares.
  - type: feature
    feature_type: trait
    name: Beast of Prey
    icon: ⭐️
    effects:
      - effect: While grabbed by the griffon, a creature has a double bane on the Escape
          Grab maneuver.
  - type: feature
    feature_type: trait
    name: Steady
    icon: ⭐️
    effects:
      - effect: Any power roll that could knock the griffon or their rider prone takes a
          bane.
~~~