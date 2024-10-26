```ds-statblock
name: War Dog Pestilite
ancestry:
- Humanoid
- War Dog
roles:
- Controller
level: 3
ev: 13
stamina: 25
immunities:
- Poison 3
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Loyalty Collar
  effect: When the pestilite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Plaguecaster
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  - Ranged
  - Resistance
  distance: 3 cube within 10
  target: Each creature in the cube
  t1: 2 poison damage; I1 [[Frightened|frightened]] (save ends)
  t2: 5 poison damage; I2 [[Frightened|frightened]] (save ends)
  t3: 8 poison damage; I3 [[Frightened|frightened]] (save ends)
  effects:
  - name: Effect
    effect: 'The area is covered in a cloud of pestilence that lasts until the start
      of the pestilite’s next turn. Any creature who enters the area for the first
      time in a round or starts their turn there takes 2 poison damage. '
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
