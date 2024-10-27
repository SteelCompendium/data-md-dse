```ds-statblock
name: [[Minotaur]] Sunderer
ancestry:
- [[Minotaur]]
- Monster
roles:
- Brute
level: 3
ev: 40
stamina: 90
immunities: []
weaknesses: []
speed: '6'
size: '2'
stability: 2
free_strike: 6
might: 2
intuition: ''
agility: 1
reason: 0
presence: -1
traits:
- name: [[Minotaur]] Sense
  effect: The sunderer cannot get a result lower than tier 2 when making Tests to
    navigate, search, or seek.
abilities:
- name: Spiked Maul
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
  t1: 6 damage; pull 1
  t2: 10 damage; pull 2
  effects:
  - name: Effect
    effect: 'A target is [[Grabbed|grabbed]] if they are pulled adjacent to the sunderer. '
- name: Fearsome Bay
  type: Action
  roll: INU RR
  cost: 5 Malice
  keywords:
  - Area
  - Resistance
  distance: 3 burst
  target: All enemies in the burst
  t1: [[Frightened]] of the [[Minotaur|minotaur]] (save ends)
  t2: [[Frightened]] of the [[Minotaur|minotaur]] (EoT)
  effects:
  - name: Effect
    effect: 'The [[Minotaur|minotaur]] has **resistance** and **advantage** until the end of their
      next turn. '
- name: Disemboweling Horns
  type: Maneuver
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 2
  target: 1 [[Grabbed|grabbed]] creature
  t1: 6 damage; push 1; M1 [[Bleeding|bleeding]] (save ends)
  t2: 10 damage; push 3; M2 [[Bleeding|bleeding]] (save ends)
  effects:
  - name: Effect
    effect: 'The target takes 6 damage at the start of each of their turns while [[Bleeding|bleeding]]
      from this ability. '
- name: Retaliatory Gore
  type: Triggered Action
  keywords:
  - '-'
  trigger: The sunderer takes damage from a creature within 6.
  distance: Self
  target: Triggering creature
  effects:
  - name: Effect
    effect: 'The sunderer [[Charge|charges]] the target using Spiked Maul. '

```
