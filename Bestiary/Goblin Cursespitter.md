~~~ds-statblock
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
intuition: 1
agility: 1
reason: 0
presence: 0
traits:
- name: Crafty
  effect: The cursespitter doesn’t provoke opportunity attacks by moving.
abilities:
- name: Eye of Surlach
  type: Action
  roll: INU RR
  cost: Signature
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  t3: 6 corruption damage; weakened (INU ends)
  t2: 5 corruption damage; weakened (EoT)
  t1: '2 corruption damage '
- name: Dizzying Hex
  type: Maneuver
  roll: INU RR
  cost: 1 VP
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  t3: Prone and can’t stand (INU ends)
  t2: Prone and can’t stand (EoT)
  t1: 'No effect '

~~~