~~~ds-statblock
name: Goblin Sniper
ancestry:
- Goblin
- Humanoid
roles:
- Artillery
- Minion
level: 1
ev: 4
stamina: 5
immunities: []
weaknesses: []
speed: 5 (climb)
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
  effect: The sniper doesn’t provoke opportunity attacks by moving.
abilities:
- name: Bow
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: One creature or object per minion
  effect: 'If the sniper doesn’t use a maneuver or a move action this turn, the ability
    deals an extra 2 damage. '

~~~