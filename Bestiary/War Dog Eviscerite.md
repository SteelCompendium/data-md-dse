```ds-statblock
name: War Dog Eviscerite
ancestry:
- Humanoid
- War Dog
roles:
- Harrier
level: 1
ev: 10
stamina: 20
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 3
might: 1
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the eviscerite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Chainsaw Whip
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 3
  target: One creature or object
  t1: 3 damage
  t2: 5 damage; pull 1
  t3: 7 damage; pull 2
  effects:
  - name: Effect
    effect: 'The eviscerite can [[Grab|grab]] a target pulled adjacent to them by this ability. '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '

```
