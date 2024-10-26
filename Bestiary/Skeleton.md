```ds-statblock
name: Skeleton
ancestry:
- Corporeal
- Undead
roles:
- Artillery
level: 1
ev: 8
stamina: 12
immunities:
- Corruption 3
- Poison 3
weaknesses: []
speed: '5'
size: 1M
stability: -2
free_strike: 4
might: 0
intuition: 0
agility: 1
reason: 1
presence: -1
traits:
- name: Arise
  effect: The first time the skeleton is reduced to Stamina 0 by damage that isn’t
    fire damage or holy damage and their body isn’t destroyed, they regain half their
    Stamina and fall [[Prone|prone]].
abilities:
- name: Bone Shards
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 10
  target: One creature or object
  t1: 2 damage
  t2: 5 damage
  t3: 6 damage
  effects:
  - name: Effect
    effect: 'Until the start of the skeleton’s next turn, the target takes 2 damage
      the first time they move on their turn. '
- name: Bone Spur
  type: Maneuver
  roll: 2d10 + 2
  cost: 2 Malice
  keywords:
  - Area
  - Weapon
  distance: 1 burst
  target: Each enemy in the burst
  t1: 1 damage; M1 [[Bleeding|bleeding]] (save ends)
  t2: 2 damage; M2 [[Bleeding|bleeding]] (save ends)
  t3: 3 damage; M3 [[Bleeding|bleeding]] (save ends)
  effects:
  - name: Effect
    effect: 'Each target has a bane on their next attack until the start of the skeleton’s
      next turn. '

```
