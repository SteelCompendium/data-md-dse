```ds-statblock
name: Specter
ancestry:
- Incorporeal
- Undead
roles:
- Hexer
level: 1
ev: 7
stamina: 12
immunities:
- Corruption 3
- Poison 3
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1M
stability: 1
free_strike: 2
might: -5
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Corruptive Phasing
  effect: The specter can move through other creatures and objects at normal speed.
    The first time in a round that the specter passes through a creature, that creature
    takes 2 corruption damage.
abilities:
- name: Decaying Touch
  type: Action
  cost: Signature
  keywords:
  - Magic
  - Melee
  distance: Melee 1
  target: One creature
  effects:
  - roll: 2d10 + 2
    t1: 2 corruption damage; P1 [[Weakened|weakened]] (save ends)
    t2: 4 corruption damage; P2 [[Weakened|weakened]] (save ends)
    t3: 5 corruption damage; P3 [[Weakened|weakened]] (save ends)
  - name: 2 Malice
    effect: 'The potency of this ability increases by 1. A living creature killed
      by this ability becomes a specter who appears in the target''s space under the
      Director''s control. '
- name: Hidden Movement
  type: Maneuver
  keywords:
  - '-'
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The specter turns invisible, moves up to their speed, and becomes visible
      again. '

```
