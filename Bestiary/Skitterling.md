```ds-statblock
name: Skitterling
ancestry:
- Animal
- Goblin
roles:
- Hexer
- Minion
level: 1
ev: 3
stamina: 5
immunities: []
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1T
stability: 0
free_strike: 2
might: -5
intuition: 0
agility: 2
reason: -4
presence: -2
traits: []
abilities:
- name: Claws
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object per minion
  t1: 2 poison damage
  t2: 3 poison damage
  t3: 4 poison damage
  effects:
  - name: Effect
    effect: The target has a bane on their next attack.

```
