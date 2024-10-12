~~~ds-statblock
name: Radenwight Bruxer
ancestry:
- Humanoid
- Radenwight
roles:
- Brute
level: 1
ev: 16
stamina: 40
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1M
stability: 2
free_strike: 5
might: 1
intuition: 0
agility: 1
reason: -1
presence: 0
traits: []
abilities:
- name: Lockjaw
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object
  effect: 'While the target is grabbed, they take 2 damage at the start of each of
    the bruxer’s turns. '
- name: Flurry of Bites
  type: Action
  roll: 2d10 + 1
  cost: 3 VP
  keywords:
  - Area
  - Weapon
  distance: 1 burst
  target: Each enemy
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: The bruxer makes a free strike against the target.

~~~