```ds-statblock
name: Demon Remasch
ancestry:
- Demon
- Planar
roles:
- AMBUSHER
level: 2
ev: 13
stamina: 25
immunities: []
weaknesses:
- Holy 3
speed: 5 ([[Teleport|teleport]])
size: 1S
stability: 0
free_strike: 4
might: 0
intuition: 0
agility: 2
reason: 0
presence: 2
traits:
- name: Lethe
  effect: While winded, the remasch has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the remasch can't be hidden from them.
abilities:
- name: Abyssal Strike
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 4 damage; the remasch [[Teleport|teleports]] 2 squares
  t2: 7 damage; the remasch [[Teleport|teleports]] 3 squares
  t3: 10 damage; the remasch [[Teleport|teleports]] 5 squares
  effects:
  - name: 5 Malice
    effect: 'The remasch takes an adjacent creature with them when they [[Teleport|teleport]].
      The creature appears in an unoccupied space adjacent to the remasch''s destination. '
- name: Grasping Shadow
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Magic
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The remasch [[Teleport|teleports]] 2 squares and uses Abyssal Strike. '

```
