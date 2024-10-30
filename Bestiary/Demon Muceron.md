```ds-statblock
name: Demon Muceron
ancestry:
- Demon
- Planar
roles:
- BRUTE
level: 3
ev: 18
stamina: 45
immunities: []
weaknesses:
- Holy 3
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 2
intuition: 0
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
  - roll: 2d10 + 2
    t1: 5 damage; pull 2
    t2: 8 damage; pull 3
    t3: 11 damage; pull 4
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
