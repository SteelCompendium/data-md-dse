```ds-statblock
name: Servitor Battle Walker
ancestry:
- Construct
- [[Dwarf]]
roles:
- Mount
level: 1
ev: 28
stamina: 60
immunities: []
weaknesses: []
speed: 8 (climb)
size: '3'
stability: 2
free_strike: 3
might: 2
intuition: 0
agility: 0
reason: -2
presence: -2
traits:
- name: Cupola
  effect: Three of the battle walker's size 1 allies can occupy the same space while
    riding the battle walker. Riders have cover against attacks that target them.
- name: Mobile Prison Harness
  effect: [[Slowed]] or [[Restrained|restrained]] creatures adjacent to the battle walker become [[Restrained|restrained]]
    (save ends) and have a bane on their resistance rolls. Adjacent [[Restrained|restrained]] creatures
    are automatically moved with the battle walker, ignoring stability.
abilities:
- name: Grasping Claws
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
  t1: 4 damage; M1 [[Slowed|slowed]] (save ends)
  t2: 7 damage; M2 [[Slowed|slowed]] (save ends)
  t3: 10 damage; M3 [[Restrained|restrained]] (save ends)
  effects:
  - name: Effect
    effect: '[[Restrained]] targets and targets [[Restrained|restrained]] by this ability are pulled
      3. A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pulled by this attack. '
- name: Stunning Blast
  type: Maneuver
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Resistance
  distance: 3 burst
  target: All enemies in the burst
  t1: 2 lightning damage; A1 [[Slowed|slowed]] (save ends)
  t2: 3 lightning damage; A2 [[Slowed|slowed]] (save ends)
  t3: '5 lightning damage; A3 [[Slowed|slowed]] (save ends) '

```
