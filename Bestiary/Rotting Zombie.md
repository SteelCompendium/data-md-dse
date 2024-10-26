```ds-statblock
name: Rotting [[Zombie]]
ancestry:
- Corporeal
- Undead
roles:
- Brute
- Minion
level: 1
ev: 4
stamina: 8
immunities:
- Corruption 2
- Poison 2
weaknesses: []
speed: '6'
size: 1M
stability: 0
free_strike: 2
might: 2
intuition: -2
agility: -2
reason: -5
presence: -3
traits:
- name: Arise Together
  effect: If the rotting [[Zombie|zombie]]’s captain has the Arise trait, the [[Zombie|zombie]] also gains
    the Arise trait.
abilities:
- name: Rotting Fist
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object per minion
  t1: 2 damage
  t2: 3 damage; M1 [[Slowed|slowed]] (save ends)
  t3: '4 damage; M2 [[Prone|prone]] if size 1, [[Slowed|slowed]] (save ends) otherwise '

```
