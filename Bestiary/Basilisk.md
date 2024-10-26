```ds-statblock
name: Basilisk
ancestry: []
roles: []
level: ''
ev: 32
stamina: 70
immunities:
- Poison 5
weaknesses: []
speed: '8'
size: '2'
stability: 2
free_strike: 5
might: 2
intuition: -1
agility: 0
reason: -3
presence: -1
traits:
- name: LEVEL 1 BRUTE
  effect: '*Basilisk, Monster*'
- name: Calcifying Presence
  effect: The area within 3 squares of the basilisk is considered [[Difficult Terrain|difficult terrain]]
    for enemies.
abilities:
- name: Noxious Bite
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 2 creatures or objects
  t1: 5 poison damage
  t2: 8 poison damage
  t3: 11 poison damage
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
- name: Poison Fumes
  type: Action
  roll: 2d10 + 2
  cost: 5 Malice
  keywords:
  - Area
  - Magic
  distance: 3 cube within 1
  target: All creatures in the cube
  t1: 4 poison damage; M1 [[Weakened|weakened]] (save ends)
  t2: 6 poison damage; M2 [[Weakened|weakened]] and [[Slowed|slowed]] (save ends)
  t3: '9 poison damage; M3 [[Weakened|weakened]] and [[Slowed|slowed]] (save ends) '
- name: Lash Out
  type: Triggered Action
  keywords:
  - —
  trigger: The basilisk takes Weapon damage.
  distance: 1 burst
  target: All enemies in the burst

```
