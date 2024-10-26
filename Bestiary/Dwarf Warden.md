```ds-statblock
name: [[Dwarf]] [[Warden]]
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Brute
level: 2
ev: 18
stamina: 53
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 3
free_strike: 5
might: 2
intuition: 1
agility: 0
reason: 0
presence: 0
traits:
- name: Escort the Prisoners
  effect: Whenever the [[Warden|warden]] moves, they can carry an adjacent [[Restrained|restrained]] enemy as
    if they were [[Grabbed|grabbed]].
abilities:
- name: Concussive Maul
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 5 damage; push 1; M1 [[Slowed|slowed]] (save ends)
  t2: 8 damage; push 3; M2 [[Slowed|slowed]] (save ends)
  effects:
  - name: '**Effect**'
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this attack. '
- name: Concussive Shockwave
  type: Maneuver
  roll: 2d10 + 2
  cost: 5 Malice
  keywords:
  - Area
  distance: 3 cube within 1
  target: All enemies in the cube
  t1: 2 damage; push 2; A1 [[Slowed|slowed]] (save ends)
  t2: 4 damage; push 4; A2 [[Slowed|slowed]] (save ends)
  effects:
  - name: '**Effect**'
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this ability. '

```
