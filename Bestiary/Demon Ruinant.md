```ds-statblock
name: Demon Ruinant
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
might: 0
intuition: ''
agility: 2
reason: 0
presence: 1
traits:
- name: LEVEL 1 HARRIER
  effect: ''
- name: Demon, Planar EV 10
  effect: '**Stamina:** 20 **Weakness:** Holy 3 **Speed:** 6 **Size:** 1M / Stability
    0 **[[Free Strike]]:** 2'
- name: Lethe
  effect: While winded, the ruinant has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the ruinant can’t be hidden from them.
abilities:
- name: Bloodletting Claws
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: Two creatures or objects
  t1: 2 damage
  t2: 5 damage; M1 [[Bleeding|bleeding]] (save ends)
  t3: '6 damage; M2 [[Bleeding|bleeding]] (save ends) '
- name: Salt Wounds
  type: Maneuver
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Three creatures without full Stamina
  t1: 2 corruption damage
  t2: 5 corruption damage
  t3: '6 corruption damage '

```
