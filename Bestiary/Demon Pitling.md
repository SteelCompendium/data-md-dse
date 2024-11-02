```ds-statblock
name: Demon Pitling
ancestry:
- Demon
- Planar
roles:
- ARTILLERY
- MINION
level: 1
ev: 2
stamina: 4
immunities: []
weaknesses:
- Holy 3
speed: 5 ([[Fly|fly]])
size: 1T
stability: 0
free_strike: 2
might: -2
intuition: -2
agility: 2
reason: -2
presence: -2
traits:
- name: Horrid Stench
  effect: Any enemy who has three or more pitlings within 2 squares of them can't
    regain Stamina.
- name: Soulsight
  effect: Each creature within 2 of the pitling can't be hidden from them.
abilities:
- name: Spit
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 poison damage
    t2: 3 poison damage
    t3: '4 poison damage '

```
