```ds-statblock
name: [[Dwarf]] Stonewhisperer
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Controller
level: 3
ev: 16
stamina: 45
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 2
free_strike: 5
might: 1
intuition: 2
agility: 0
reason: 2
presence: 0
traits:
- name: Stonewalker
  effect: The stonewhisperer can phase through 2 squares of stone as part of any movement
    they take. If they end their movement inside stone, they are shunted out into
    the square where they entered it.
abilities:
- name: Tile Slide
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  distance: 3 cube within 1
  target: All creatures and objects
  t1: 3 damage; slide 1; M1 [[Slowed|slowed]] (save ends)
  t2: 6 damage; slide 3; M2 [[Slowed|slowed]] (save ends)
  t3: 9 damage; slide 5; M3 [[Restrained|restrained]] (save ends)
  effects:
  - roll: 2d10 + 2
    t1: 3 damage; slide 1; M1 [[Slowed|slowed]] (save ends)
    t2: 6 damage; slide 3; M2 [[Slowed|slowed]] (save ends)
    t3: 9 damage; slide 5; M3 [[Restrained|restrained]] (save ends)
  - name: Effect
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be slid by this attack. '
- name: Stone Wave
  type: Maneuver
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Area
  - Ranged
  distance: 2 cube within 10
  target: All enemies in the cube
  t1: 2 damage; push 2; R1 [[Slowed|slowed]] (save ends)
  t2: 3 damage; push 3; R2 [[Slowed|slowed]] (save ends)
  t3: 4 damage; push 3; R3 [[Slowed|slowed]] (save ends)
  effects:
  - roll: 2d10 + 2
    t1: 2 damage; push 2; R1 [[Slowed|slowed]] (save ends)
    t2: 3 damage; push 3; R2 [[Slowed|slowed]] (save ends)
    t3: 4 damage; push 3; R3 [[Slowed|slowed]] (save ends)
  - name: Effect
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this attack. The affected
      area is [[Difficult Terrain|difficult terrain]] for enemies. '

```
