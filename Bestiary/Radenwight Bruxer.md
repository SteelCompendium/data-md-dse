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
  t1: 5 damage
  t2: 9 damage; [[Grabbed|grabbed]]
  t3: 12 damage; [[Grabbed|grabbed]]
  effect: 'While the target is [[Grabbed|grabbed]], they take 2 damage at the start of each of
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
  t1: 4 damage
  t2: 8 damage
  t3: '10 damage; [[Bleeding|bleeding]] (EoT) '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: The bruxer makes a [[Free Strike|free strike]] against the target.

~~~