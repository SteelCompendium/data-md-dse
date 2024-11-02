```ds-statblock
name: Shieldscale Drangolin
ancestry:
- Animal
- Kobold
roles:
- Brute
level: 1
ev: 16
stamina: 40
immunities: []
weaknesses: []
speed: 7 ([[Burrow|burrow]])
size: '3'
stability: 0
free_strike: 4
might: 2
intuition: 0
agility: 1
reason: -3
presence: -2
traits:
- name: Ash Shot
  effect: An enemy adjacent to the drangolin has resistance and can't be hidden.
abilities:
- name: Fiery Claws
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  effects:
  - roll: 2d10 + 2
    t1: 4 fire damage
    t2: 7 fire damage
    t3: '10 fire damage '
- name: Drangolin Plume
  type: Action
  cost: 5 Malice
  keywords:
  - '-'
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The drangolin shifts their speed and makes a Fiery Claws attack against
      each creature who comes within 1 during the move. The drangolin makes one power
      roll against all targets. '
- name: Erupt
  type: Action
  cost: 3 Malice
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: 2 Burst (while burrowing)
  target: All creatures
  effects:
  - roll: 2d10 + 2
    t1: 4 damage; push 1; 1 [[Prone|prone]]
    t2: 7 damage; push 3; 2 [[Prone|prone]]
    t3: 10 damage; push 5; 3 [[Prone|prone]]
  - name: Effect
    effect: 'This attack has an edge against targets directly above the drangolin. '

```
