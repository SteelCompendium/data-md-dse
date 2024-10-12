~~~ds-statblock
name: Radenwight Maestro
ancestry:
- Humanoid
- Radenwight
roles:
- Boss
level: 1
ev: 38
stamina: 80
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 1
free_strike: 5
might: -2
intuition: 0
agility: 2
reason: 0
presence: 2
traits:
- name: End Effect
  effect: At the end of their turn, the maestro can take 5 damage to end one EoE effect
    affecting them. This damage can't be reduced in any way.
abilities:
- name: Cacophony
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  distance: 5 burst
  target: Each enemy
  t1: 3 sonic damage; slide 1; the maestro can shift 1 square
  t2: 5 sonic damage; slide 3; the maestro can shift 3 squares
  t3: 7 sonic damage; slide 5; the maestro can shift 5 squares
  effect: 'Each of the maestro''s allies can use Ready Rodent as a free triggered
    action once before the end of the round. '
- name: Tempo Change
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: Two enemies
  t3: Slowed (MGT ends)
  t2: Slowed (EoT)
  t1: 'No effect  5 VP: Each ally of the maestro within distance has their speed increased
    by 2 until the end of their next turn. '
- name: Ranged Ready Rodent
  type: Triggered Action
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature
  trigger: An ally deals damage to the target.
  effect: 'The maestro makes a free strike against the target. '
- name: Overture
  type: Villain Action
  cost: 1 VP
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effect: 'Each target shifts up to their speed or takes the Defend action. '
- name: Solo Act
  type: Villain Action
  cost: 2 VP
  keywords:
  - Ranged
  distance: Ranged 15
  target: One creature
  effect: 'Until the end of their next turn, the target''s stamina can''t be reduced
    below 1, their speed is doubled, and their next power roll is automatically a
    tier 3 result. '
- name: Rondo of Rat
  type: Villain Action
  cost: 3 VP
  keywords:
  - Area
  distance: 10 burst
  target: Each dead ally
  effect: Each target stands, makes a free strike, then collapses again. Allies of
    the targets can use Ready Rodent as a free triggered action once in conjunction
    with these free strikes.

~~~