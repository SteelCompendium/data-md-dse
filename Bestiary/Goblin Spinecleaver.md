```ds-statblock
name: Goblin Spinecleaver
ancestry:
- Goblin
- Humanoid
roles:
- Brute
- Minion
level: 1
ev: 6
stamina: 10
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: 2
intuition: 0
agility: 0
reason: 0
presence: -1
traits:
- name: Crafty
  effect: The spinecleaver doesn't provoke opportunity attacks by moving.
abilities:
- name: Axe
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object per minion
  t1: 2 damage; push 1
  t2: 4 damage; push 3
  t3: '5 damage; push 4 '
  effects:
  - roll: 2d10 + 2
    t1: 2 damage; push 1
    t2: 4 damage; push 3
    t3: '5 damage; push 4 '

```
