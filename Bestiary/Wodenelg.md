```ds-statblock
name: Wodenelg
ancestry:
- Plant
- Wode Elf
roles:
- Mount
level: 1
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 2
intuition: 0
agility: 1
reason: -1
presence: -1
traits:
- name: Sure Footed
  effect: The wodenelg ignores all [[Difficult Terrain|difficult terrain]], including enemy squares, and
    doesn’t provoke opportunity attacks by moving.
- name: Mounted Stability
  effect: The wodenelg’s rider has **+3** to Stability.
- name: Shared Glamor
  effect: If the wodenelg’s rider has the Masking Glamor or Hunter’s Glamor trait,
    they also gain the trait’s benefits.
abilities:
- name: Gore
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 2 damage
  t2: 5 damage
  effects:
  - name: Effect
    effect: 'The wodenelg’s rider can make a [[Free Strike|free strike]] at any point during the [[Charge|charge]]. '
- name: Where I End the Woods Begin
  type: Maneuver
  cost: 3 Malice
  keywords:
  - —
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The wodenelg and their rider become invisible until the start of their
      next turn. '

```
