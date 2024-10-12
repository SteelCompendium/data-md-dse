~~~ds-statblock
name: Radenwight Ratcrobat
ancestry:
- Humanoid
- Radenwight
roles:
- Harrier
level: 1
ev: 13
stamina: 30
immunities: []
weaknesses: []
speed: 7 (climb)
size: 1S
stability: 0
free_strike: 5
might: -1
intuition: 0
agility: 1
reason: 0
presence: 1
traits:
- name: Gymratstics
  effect: The ratcrobat gains an edge on attacks against larger creatures.
abilities:
- name: En Garde!
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: Two creatures or objects
  t1: 2 damage
  t2: 5 damage
  t3: 6 damage
  effect: 'The ratcrobat can shift up to 2 squares after attacking the first target,
    then can shift 1 square after attacking the second target. '
- name: Over Here, Thanks
  type: Maneuver
  keywords:
  - Melee
  distance: Reach 1
  target: One enemy
  effect: 'Slide 1; the ratcrobat can then shift into the square the target left. '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: 'The ratcrobat makes a free strike against the target. '

~~~