```ds-statblock
name: War Dog Phosphorite
ancestry:
- Humanoid
- War Dog
roles:
- Hexer
level: 2
ev: 10
stamina: 20
immunities:
- Acid 3
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the phosphorite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Caustic Detonator
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature or object
  t1: 3 acid damage; M1 [[Bleeding|bleeding]] (save ends)
  t2: 5 acid damage; M2 [[Bleeding|bleeding]] (save ends)
  t3: 7 acid damage; M3 [[Bleeding|bleeding]] (save ends)
  effects:
  - roll: 2d10 + 2
    t1: 3 acid damage; M1 [[Bleeding|bleeding]] (save ends)
    t2: 5 acid damage; M2 [[Bleeding|bleeding]] (save ends)
    t3: 7 acid damage; M3 [[Bleeding|bleeding]] (save ends)
  - name: Effect
    effect: 'A detonator attaches to the target. At the end of each round, roll a
      die. On an odd result, the detonator explodes, triggering the power roll. '
  - name: Special
    effect: 'An adjacent creature can attempt an easy Agility test to remove the detonator
      as a maneuver. A failure does nothing, a success disarms and destroys the detonator,
      and a success with a reward allows the disarming creature to throw the detonator
      onto another target within 5 squares. '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target''s loyalty collar detonates, killing them instantly. '

```
