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

```ds-statblock
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
traits:
  - name: Beast of Prey
    effects:
      - effect: While grabbed by the griffon, a creature has a double bane on the Escape
          Grab maneuver.
  - name: Steady
    effects:
      - effect: Any power roll that could knock the griffon or their rider prone takes a
          bane.
abilities:
  - name: Claw Swipes
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; the griffon can shift 1 square
        t2: 10 damage; the griffon shifts up to 2 squares
        t3: 13 damage; the griffon shifts up to 3 squares
      - effect: If this ability is used as part of the Charge main action, the griffon
          can grab one of the targets
  - name: Crack the Earth
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 3 cube within 8
    target: Each enemy in the area
    effects:
      - effect: The griffon must be flying and must have a creature or object grabbed.
        name: Special
      - effect: The griffon flies up to half their speed toward the ground, then sends
          the creature or object they've grabbed hurtling down. The creature or
          object hits the ground to turn the area into an impact crater, and
          takes falling damage that can't be reduced in any way.
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage; A < 1 push 3
        t3: 9 damage; A < 2 push 4; prone
  - name: Wing Buffet
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 4 x 2 line within 1
    target: Each creature or object in the area
    effects:
      - effect: A target object must be size 2 or smaller.
        name: Special
      - roll: Power Roll + 2
        t1: Push 3; A < 0 the forced movement is vertical
        t2: Push 4; A < 1 the forced movement is vertical
        t3: Push 5; A < 2 the forced movement is vertical
  - name: Zephyr Feint
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The griffon takes damage
    effects:
      - effect: The griffon halves the damage, ignores any nondamaging effects
          associated with it, and shifts up to 2 squares
```