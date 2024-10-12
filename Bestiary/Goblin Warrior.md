~~~ds-statblock
name: Goblin Warrior
ancestry:
- Goblin
- Humanoid
roles:
- Harrier
level: 1
ev: 10
stamina: 20
immunities: []
weaknesses: []
speed: 6 (climb)
size: 1S
stability: 0
free_strike: 2
might: -2
intuition: 0
agility: 1
reason: 0
presence: -1
traits:
- name: Crafty
  effect: The warrior doesn’t provoke opportunity attacks by moving.
abilities:
- name: Spear
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Charge
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object
  t1: 2 damage
  t2: 5 damage
  t3: '6 damage '
- name: Bury the Point
  type: Action
  roll: 2d10 + 1
  cost: 2 VP
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  t1: 3 damage
  t2: 7 damage; bleeding (EoT)
  t3: '8 damage; bleeding (MGT ends) '

~~~