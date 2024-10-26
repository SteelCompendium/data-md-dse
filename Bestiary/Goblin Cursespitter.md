```ds-statblock
name: Goblin Cursespitter
ancestry:
- Goblin
- Humanoid
roles:
- Hexer
level: 1
ev: 9
stamina: 15
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: -2
intuition: 2
agility: 1
reason: 0
presence: 0
traits:
- name: Crafty
  effect: The cursespitter doesn’t provoke opportunity attacks by moving.
abilities:
- name: Eye of Surlach
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  t1: 2 corruption damage; I1 [[Weakened|weakened]] (save ends)
  t2: 5 corruption damage; I2 [[Weakened|weakened]] (save ends)
  t3: '6 corruption damage; I3 [[Weakened|weakened]] (save ends) '
- name: Dizzying Hex
  type: Maneuver
  roll: INU RR
  cost: 1 Malice
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  t1: [[Prone]] and can’t stand (save ends)
  t2: [[Prone]] and can’t stand (EoT)
  t3: 'No effect '

```
