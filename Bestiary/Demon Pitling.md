```ds-statblock
name: Demon Pitling
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
might: -2
intuition: -2
agility: 2
reason: -2
presence: -2
traits:
- name: LEVEL 1 ARTILLERY MINION
  effect: ''
- name: Demon, Planar EV 2
  effect: '**Stamina:** 4 **Weakness:** Holy 3 **Speed:** 5 ([[Fly|fly]]) **Size:** 1T / Stability
    0 **[[Free Strike]]:** 2'
- name: Horrid Stench
  effect: Any enemy who has three or more pitlings within 2 squares of them can’t
    regain Stamina.
- name: Soulsight
  effect: Each creature within 2 of the pitling can’t be hidden from them.
abilities:
- name: Spit
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: One creature or object per minion
  t1: 2 poison damage
  t2: 3 poison damage
  t3: '4 poison damage '

```
