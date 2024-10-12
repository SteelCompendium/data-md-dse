~~~ds-statblock
name: Giant Hawk
ancestry:
- Animal
roles:
- Mount
level: 1
ev: 13
stamina: 20
immunities: []
weaknesses: []
speed: 7 (flying)
size: '2'
stability: 0
free_strike: 3
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
  target: One creature or object
  t1: 3 damage
  t2: 5 damage
  t3: 7 damage
  effect: 'The target is grabbed by the giant hawk. '
- name: Dive
  type: Maneuver

~~~