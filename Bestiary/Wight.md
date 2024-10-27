```ds-statblock
name: Wight
ancestry:
- Corporeal
- Undead
roles:
- Hexer
level: 1
ev: 7
stamina: 12
immunities:
- Corruption 3
- Poison 3
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 2
intuition: 0
agility: 1
reason: 0
presence: 1
traits:
- name: Arise
  effect: The first time the wight is reduced to Stamina 0 by damage that isn't fire
    damage or holy damage and their body isn't destroyed, they regain half their Stamina
    and fall [[Prone|prone]].
abilities:
- name: Lifestealer Longsword
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 2 corruption damage
  t2: 4 corruption damage; M1 [[Slowed|slowed]] (save ends)
  t3: 5 corruption damage; M2 [[Slowed|slowed]] and [[Weakened|weakened]] (save ends)
  effects:
  - name: Effect
    effect: 'The target appears to rapidly age each time they take damage from this
      attack. The target regains their former appearance when the wight is destroyed. '
- name: Raise
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Magic
  - Ranged
  distance: Ranged 3
  target: One dead ally
  effects:
  - name: Effect
    effect: 'The target revives with half their Stamina. The wight can''t use this
      maneuver again until they attack a creature with their lifestealer longsword. '

```
