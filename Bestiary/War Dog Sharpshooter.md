```ds-statblock
name: War Dog Sharpshooter
ancestry:
- Humanoid
- War Dog
roles:
- Artillery
- Minion
level: 1
ev: 4
stamina: 8
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the sharpshooter dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Bolt Launcher
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 5
  target: One creature or object per minion
  t1: 2 damage
  t2: 3 damage
  t3: 4 damage
  effects:
  - name: Effect
    effect: 'This ability ignores cover and concealment. '

```
