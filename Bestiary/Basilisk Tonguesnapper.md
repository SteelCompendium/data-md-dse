```ds-statblock
name: [[Basilisk]] Tonguesnapper
ancestry: []
roles: []
level: ''
ev: 26
stamina: 50
immunities:
- Poison 5
weaknesses: []
speed: '8'
size: '2'
stability: 2
free_strike: 4
might: 1
intuition: -1
agility: 2
reason: -3
presence: -1
traits:
- name: LEVEL 1 HEXER
  effect: '*[[Basilisk]], Monster*'
- name: Petrifying Fumes
  effect: A creature that starts their turn adjacent to the tonguesnapper is M2 [[Slowed|slowed]]
    (save ends).
abilities:
- name: Prehensile Tongue
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 3
  target: 1 creature or object
  t1: 6 acid damage; pull 1
  t2: 8 acid damage; pull 2
  t3: 12 acid damage; pull 3
- name: Petrifying Eye Beams
  type: Maneuver
  cost: MGT RR
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 5 × 2 line within 1
  target: Special
  t1: [[Restrained]] (save ends)
  t2: [[Slowed]] (save ends)
  t3: [[Slowed]] (EoT)
- name: Wink
  type: Action
  roll: 2d10 + 2
  cost: 2 Malice
  keywords:
  - Attack
  - Melee
  - Magic
  - Ranged
  distance: Melee 1 or Ranged 10
  target: 1 creature
  t1: 6 corruption damage; R1 [[Dazed|dazed]] (save ends)
  t2: 8 corruption damage; R2 [[Dazed|dazed]] (save ends)
  t3: 12 corruption damage; R3 [[Dazed|dazed]] and [[Slowed|slowed]] (save ends)
- name: Neurotoxin Splash
  type: Triggered Action
  keywords:
  - —
  trigger: The tonguesnapper takes Weapon damage.
  distance: 2 burst
  target: All enemies in the burst

```
