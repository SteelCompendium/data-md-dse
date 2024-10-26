```ds-statblock
name: Demon Remasch
ancestry: []
roles: []
level: ''
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 0
intuition: ''
agility: 2
reason: 0
presence: 2
traits:
- name: LEVEL 2 AMBUSHER
  effect: ''
- name: Demon, Planar EV 13
  effect: '**Stamina:** 25 **Weakness:** Holy 3 **Speed:** 5 ([[Teleport|teleport]]) **Size:**
    1S / Stability 0 **[[Free Strike]]:** 4'
- name: Lethe
  effect: While winded, the remasch has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the remasch can’t be hidden from them.
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
  t3: '10 damage; the remasch [[Teleport|teleports]] 5 squares 5 Malice: The remasch takes an adjacent
    creature with them when they [[Teleport|teleport]]. The creature appears in an unoccupied space
    adjacent to the remasch’s destination. '
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
