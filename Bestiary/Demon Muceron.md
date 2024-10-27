```ds-statblock
name: Demon Muceron
ancestry:
- Demon
- Planar EV 18
roles:
- BRUTE
level: 3
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 2
intuition: ''
agility: 2
reason: 0
presence: 1
traits:
- name: Lethe
  effect: While winded, the muceron has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the muceron can't be hidden from them.
abilities:
- name: Barbed Tongues
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: One creature
  t1: 5 damage; pull 2
  t2: 8 damage; pull 3
  t3: 11 damage; pull 4
  effects:
  - name: Effect
    effect: '[[Taunted]] (EoT). '
- name: Tongue Pull
  type: Maneuver
  cost: 2 Malice
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 5
  target: Three creatures
  effects:
  - name: Effect
    effect: 'The muceron pulls each target 5 squares. '

```
