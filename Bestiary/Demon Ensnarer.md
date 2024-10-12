~~~ds-statblock
name: Demon Ensnarer
ancestry:
- Demon
- Planar
roles:
- Brute
- Minion
level: 1
ev: 6
stamina: 10
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 1
intuition: -1
agility: 0
reason: -1
presence: -1
traits:
- name: Soulsight
  effect: Each creature within 2 squares of the ensnarer can’t be hidden from them.
abilities:
- name: Barbed Tongues
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 3
  target: One creature or object per minion
  t1: 2 damage; pull 1
  t2: 4 damage; pull 2
  t3: '5 damage; pull 3; slowed (EoT) '
weakness: Holy 3

~~~