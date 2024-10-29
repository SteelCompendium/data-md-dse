```ds-statblock
name: Ogre Juggernaut
ancestry:
- Giant
- Ogre
roles:
- Harrier
level: 2
ev: 32
stamina: 70
immunities: []
weaknesses: []
speed: '6'
size: '2'
stability: 2
free_strike: 5
might: 2
intuition: 0
agility: 1
reason: -1
presence: -1
traits:
- name: Destructive Path
  effect: The juggernaut automatically destroys unattended, mundane size 1 objects
    in their path during their movement. They can break through any mundane wall made
    of wood, stone, or a similarly sturdy material in this way, so long as the wall
    is no more than 1 square thick.
- name: Defiant Anger
  effect: The juggernaut has Weapon immunity 2 while they are winded.
abilities:
- name: Pitchfork Catapult
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 2
  target: 2 creatures or objects
  t1: 5 damage; A1 vertical slide 2
  t2: 8 damage; A2 vertical push 3
  t3: 11 damage; A3 vertical slide 5
  effects:
  - name: 1 Malice
    effect: 'Each target is M2 [[Bleeding|bleeding]] (save ends). '
- name: Earth Breaking [[Jump]]
  type: Action
  cost: 2d10 + 2
  keywords:
  - Area
  - Melee
  - Weapon
  distance: 3 burst
  target: All creatures in the burst
  t1: 3 damage; M1 [[Prone|prone]]
  t2: 4 damage; push 2; M2 [[Prone|prone]]
  t3: '5 damage; push 4; M3 [[Prone|prone]] '
  effects:
  - name: Effect
    effect: 'The juggernaut leaps up to 6 squares before making the attack. '
- name: Horrible Bellow
  type: Maneuver
  roll: INU RR
  cost: 2 Malice
  keywords:
  - Area
  - Resistance
  distance: 3 burst
  target: All enemies in the burst
  t1: [[Frightened]] (save ends)
  t2: [[Frightened]] (EoT)
  t3: No effect
  effects:
  - name: Effect
    effect: 'Ogres have **advantage** on attacks against creatures [[Frightened|frightened]] by this
      ability. '
- name: Hrraaaaaagh!
  type: Triggered Action
  keywords:
  - '-'
  trigger: The juggernaut takes damage.
  distance: Melee 1
  target: 1 creature or object
  effects:
  - name: Effect
    effect: 'The juggernaut moves up to their speed and makes a [[Free Strike|free strike]]. '

```
