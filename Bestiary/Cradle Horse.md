```ds-statblock
name: Cradle Horse
ancestry:
- Construct
- High Elf
roles:
- Mount
level: 1
ev: 13
stamina: 30
immunities: []
weaknesses: []
speed: '10'
size: '2'
stability: 2
free_strike: 3
might: 2
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Shared Otherworldly Grace
  effect: If the cradle horse's rider has the Otherworldly Grace trait, it also gains
    the Otherworldly Grace trait.
abilities:
- name: Radiant [[Charge]]
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
  t1: 3 damage; M1 [[Prone|prone]]
  t2: 5 fire damage; M2 [[Prone|prone]]
- name: Stomp
  type: Action
  cost: 2d10 + 2
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: 1 burst
  target: All enemies in the burst
  t1: 2 damage
  t2: 4 damage
  effects:
  - name: Effect
    effect: 'This attack has edge against [[Prone|prone]] targets. '
- name: Buck
  type: Maneuver
  cost: 2 Malice
  keywords:
  - '-'
  distance: Self
  target: The horse's rider
  effects:
  - name: Effect
    effect: 'Vertical slide 3; The rider can use a ranged ability at any point during
      the movement and then fall without taking damage. '

```
