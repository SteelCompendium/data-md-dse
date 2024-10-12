~~~ds-statblock
name: Siege Hawk
ancestry:
- Animal
roles:
- Mount
level: 1
ev: 28
stamina: 60
immunities: []
weaknesses: []
speed: 7 (flying)
size: '3'
stability: 0
free_strike: 4
might: 1
intuition: 0
agility: 1
reason: -3
presence: -2
traits:
- name: Mounted Platform
  effect: Any creature riding the hawk can make a free strike during or after the
    hawk’s movement.
abilities:
- name: Talons
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: Two creatures or objects
  t1: 4 damage
  t2: 7 damage
  t3: 10 damage
  effect: 'The target is grabbed by the siege hawk. The siege hawk can have two targets
    grabbed at a time. '
- name: Bombs Away!
  type: Action
  roll: AGL RR
  cost: 7 VP
  keywords:
  - Area
  - Magic
  - Ranged
  - Resistance
  distance: 5 cube within 10
  target: Each creature and object
  t3: 7 fire damage; restrained (EoT)
  t2: 6 fire damage; slowed (EoT)
  t1: 3 fire damage
  special: 'The siege hawk must be flying to use this ability. '
- name: Dive
  type: Maneuver

~~~