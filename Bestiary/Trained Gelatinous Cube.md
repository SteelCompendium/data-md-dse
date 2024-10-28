```ds-statblock
name: Trained Gelatinous Cube
ancestry:
- Animal
- Kobold
roles:
- Hexer
level: 1
ev: 16
stamina: 20
immunities:
- Acid 3
- Weapon 3
weaknesses: []
speed: '5'
size: '2'
stability: 2
free_strike: 4
might: 2
intuition: 0
agility: -1
reason: -3
presence: -2
traits:
- name: You Didn't Pay Attention! (Free Triggered Action)
  effect: 'Keywords: - Trigger: A creature moves or is force moved into the cube.
    Distance: Self Target: Self Effect: The cube uses Engulf with a double edge.'
- name: Translucent Cube
  effect: The cube completely occupies its space, blocking line of effect on enemy
    attacks and abilities. The cube is hidden until revealed.
abilities:
- name: Engulf
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 3 acid damage; 1 [[Dazed|dazed]] (save ends)
  t2: 5 acid damage; 2 [[Dazed|dazed]] (save ends)
  t3: 7 acid damage; 3 [[Restrained|restrained]] (save ends)
  effects:
  - name: Effect
    effect: A size 2 or smaller creature [[Restrained|restrained]] by this attack is pulled into
      one of the cube's squares and moves with the cube. The creature takes 3 acid
      damage at the start of each of their turns while [[Restrained|restrained]]. When [[Restrained|restrained]]
      ends, the creature moves to the nearest unoccupied square adjacent to the cube.
  - name: 3 Malice
    effect: 'The cube attacks 1 additional target. '

```
