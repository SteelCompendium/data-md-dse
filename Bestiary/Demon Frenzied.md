~~~ds-statblock
name: Demon Frenzied
ancestry:
- Demon
- Planar
roles:
- Harrier
- Minion
level: 1
ev: 4
stamina: 8
immunities: []
weaknesses: []
speed: '6'
size: 1M
stability: 0
free_strike: 1
might: 0
intuition: -1
agility: 1
reason: -1
presence: -1
traits:
- name: Soulsight
  effect: Each creature within 2 squares of the frenzied can’t be hidden from them.
abilities:
- name: Rip and Tear
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Charge
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object per minion
  t1: 2 damage
  t2: 3 damage
  t3: '4 damage '
weakness: Holy 3

~~~