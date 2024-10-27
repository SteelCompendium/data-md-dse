```ds-statblock
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
might: 2
intuition: 1
agility: 2
reason: -3
presence: -2
traits:
- name: Mounted Platform
  effect: Any creature riding the hawk can make a [[Free Strike|free strike]] during or after the
    hawk's movement.
abilities:
- name: Talons
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 3 damage; M2 [[Grabbed|grabbed]]
  t2: 5 damage; M3 [[Grabbed|grabbed]]
  t3: '7 damage; [[Grabbed|grabbed]] '
- name: Dive
  type: Maneuver

```
