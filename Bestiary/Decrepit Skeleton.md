```ds-statblock
name: Decrepit [[Skeleton]]
ancestry:
- Corporeal
- Undead
roles:
- Artillery
- Minion
level: 1
ev: 2
stamina: 4
immunities:
- Corruption 2
- Poison 2
weaknesses: []
speed: '5'
size: 1M
stability: -2
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: -2
presence: -2
traits:
- name: Bonetrops
  effect: When the decrepit [[Skeleton|skeleton]] is reduced to Stamina 0, its space becomes difficult
    terrain. The first time any enemy enters this space, they take 1 damage.
abilities:
- name: Bone Bow
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
    t2: 3 damage
    t3: 4 damage
  - name: Effect
    effect: 'The decrepit [[Skeleton|skeleton]] chooses one other target within distance to take
      1 damage. '

```
