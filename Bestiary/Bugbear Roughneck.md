```ds-statblock
name: Bugbear Roughneck
ancestry: []
roles: []
level: ''
ev: 36
stamina: 80
immunities: []
weaknesses: []
speed: '6'
size: 1M
stability: 0
free_strike: 5
might: 2
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: LEVEL 2 BRUTE
  effect: '*Bugbear, Goblin, Humanoid*'
- name: Catcher (Free Triggered Action)
  effect: 'Keywords: — Distance: Melee 1 Target: 1 size 1 creature or object Trigger:
    The target is force moved into a square adjacent to the roughneck. - Effect: The
    target is [[Grabbed|grabbed]] by the roughneck.'
abilities:
- name: Haymaker
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 2 creatures or objects
  t1: 5 damage
  t2: 9 damage; one target is [[Grabbed|grabbed]]; one target gets push 2
  t3: 12 damage; one target is [[Grabbed|grabbed]]; one target gets vertical push 3
- name: Leaping Fury
  type: Action
  cost: 2d10 + 3
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 5 damage; M1 [[Prone|prone]]
  t2: 9 damage; M2 [[Prone|prone]]
  t3: 12 damage; M3 [[Prone|prone]]
- name: Drag Through Hell
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Melee
  distance: Melee 1
  target: 1 creature or object [[Grabbed|grabbed]] by the roughneck
- name: Throw
  type: Maneuver
  keywords:
  - Attack
  - Melee
  distance: Melee 1
  target: 1 creature or object [[Grabbed|grabbed]] by the roughneck
- name: Flying Sawblade
  type: Triggered Action
  keywords:
  - —
  distance: Self
  target: Self
  trigger: The roughneck is vertically moved by another creature.
weapon_immunity: '3'

```
