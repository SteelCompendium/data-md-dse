```ds-statblock
name: Demon Ensnarer
ancestry: []
roles: []
level: ''
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 2
intuition: -1
agility: 0
reason: -1
presence: -1
traits:
- name: LEVEL 1 BRUTE MINION
  effect: ''
- name: Demon, Planar EV 6
  effect: '**Stamina:** 10 **Weakness:** Holy 3 **Speed:** 5 **Size:** 1M / Stability
    0 **[[Free Strike]]:** 2'
- name: Soulsight
  effect: Each creature within 2 of the ensnarer can’t be hidden from them.
abilities:
- name: Barbed Tongues
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 3
  target: One creature or object per minion
  t1: 2 damage; pull 1
  t2: 4 damage; pull 2
  t3: 5 damage; pull 3
  effects:
  - name: Effect
    effect: 'If the target is pulled adjacent to the ensnarer, the ensnarer takes
      a [[Free Strike|free strike]] against them. '

```
