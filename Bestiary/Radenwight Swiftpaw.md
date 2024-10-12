~~~ds-statblock
name: Radenwight Swiftpaw
ancestry:
- Humanoid
- Radenwight
roles:
- Harrier
- Minion
level: 1
ev: 6
stamina: 10
immunities: []
weaknesses: []
speed: 7 (climb)
size: 1S
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 1
presence: -1
traits: []
abilities:
- name: Rapier Flunge
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object per minion
  t1: 2 damage; slide 1; the swiftpaw can shift 1 square
  t2: 4 damage; slide 2; the swiftpaw can shift 2 squares
  t3: '5 damage; slide 3; the swiftpaw can shift 3 squares '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: The swiftpaw makes a free strike against the target.

~~~