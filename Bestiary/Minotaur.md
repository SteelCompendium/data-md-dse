```ds-statblock
name: Minotaur
ancestry:
- Minotaur
- Monster
roles:
- Harrier
level: 3
ev: 36
stamina: 70
immunities: []
weaknesses: []
speed: '8'
size: '2'
stability: 2
free_strike: 5
might: 2
intuition: ''
agility: 2
reason: 0
presence: -1
traits:
- name: Minotaur Sense
  effect: The minotaur cannot get a result lower than tier 2 when making Tests to
    navigate, search, or seek.
abilities:
- name: Flail and Blade
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 2
  target: 2 creatures or objects
  t1: 5 damage; push 1
  t2: 9 damage; push 2
  effects:
  - name: Effect
    effect: 'The minotaur shifts 3 after attacking. '
- name: Primal Bay
  type: Action
  cost: 3 Malice
  keywords:
  - '-'
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The minotaur has **resistance** and **advantage** until the end of their
      next turn. On their next turn, they have access to an additional maneuver. '
- name: Goring Horns
  type: Maneuver
  roll: 2d10 + 2
  cost: 5 Malice
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 2
  target: 1 creature or object
  t1: 5 damage; I1 [[Dazed|dazed]] (save ends)
  t2: 9 damage; I2 [[Dazed|dazed]] (save ends)
  effects:
  - name: Effect
    effect: 'The potency of this ability increases by 1 if it''s used while charging. '
- name: Retaliatory Gore
  type: Triggered Action
  keywords:
  - '-'
  trigger: The minotaur takes damage from a creature within 8.
  distance: Self
  target: Triggering creature
  effects:
  - name: Effect
    effect: 'The minotaur [[Charge|charges]] the target using Flail and Blade or Goring Horns. '

```
