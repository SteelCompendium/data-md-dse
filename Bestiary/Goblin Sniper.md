```ds-statblock
name: Goblin [[Sniper]]
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
agility: 2
reason: 0
presence: -1
traits:
- name: Crafty
  effect: The [[Sniper|sniper]] doesn't provoke opportunity attacks by moving.
abilities:
- name: Bow
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
    t1: 2 damage
    t2: 4 damage
    t3: 5 damage
  - name: Effect
    effect: 'If the [[Sniper|sniper]] doesn''t use a maneuver or a move action this turn, the
      ability has edge. '

```
