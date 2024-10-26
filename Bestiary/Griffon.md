```ds-statblock
name: Griffon
ancestry:
- Animal
- Griffon
roles:
- Mount
level: 2
ev: 32
stamina: 70
immunities: []
weaknesses: []
speed: 9 ([[Fly|fly]])
size: '2'
stability: 2
free_strike: 5
might: 2
intuition: 0
agility: 2
reason: -1
presence: 2
traits:
- name: Beast of Prey
  effect: Creatures have a double bane on escaping the griffon’s [[Grab|grab]].
- name: Steady
  effect: Creatures have a bane on power rolls that could knock the griffon or their
    rider [[Prone|prone]].
abilities:
- name: Claw Swipes
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 1
  target: 2 creatures or objects
  t1: 5 damage; shift 1
  t3: 11 damage; shift 3
  effects:
  - name: Effect
    effect: 'If this ability is used while charging, the griffon grapples one of the
      targets. '
- name: Crack the Earth
  type: Maneuver
  keywords:
  - Area
  - Ranged
  distance: 3 cube within 8 (while flying and grappling a creature or object)
  target: All enemies
  t1: 2 damage; A1 push 2
  t3: '4 damage; A3 push 4 and [[Prone|prone]] '
  effects:
  - name: Effect
    effect: The griffon flies up to half their speed towards the ground and then sends
      the creature or object they’ve grappled hurtling towards the affected area.
- name: Wing Buffet
  type: Maneuver
  roll: MGT RR
  cost: 3 Malice
  keywords:
  - Area
  - Resistance
  distance: 4 × 2 line within 1
  target: All creatures and objects
  t1: Vertical push 4
  t3: 'Push 2 '
- name: Juke
  type: Triggered Action
  cost: 1 Malice
  keywords:
  - —
  trigger: The griffon takes damage
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The griffon halves the damage, doesn’t suffer any effect associated with
      it, and shifts 2 squares. '

```
