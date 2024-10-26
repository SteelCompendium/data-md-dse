```ds-statblock
name: War Dog Commando
ancestry:
- Humanoid
- War Dog
roles:
- Ambusher
- Minion
level: 1
ev: 5
stamina: 8
immunities: []
weaknesses: []
speed: '5'
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
  effect: When the commando dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Daggers
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: One creature per minion
  t1: 2 damage
  t2: 4 damage
  t3: 5 damage
  effects:
  - name: Effect
    effect: 'The commando can use the [[Hide]] maneuver, even if observed. '

```
