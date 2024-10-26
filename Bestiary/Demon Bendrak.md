```ds-statblock
name: Demon Bendrak
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
agility: 1
reason: 0
presence: 2
traits:
- name: LEVEL 2 HEXER
  effect: ''
- name: Demon, Planar EV 11
  effect: '**Stamina:** 20 **Weakness:** Holy 3 **Speed:** 5 **Size:** 1S / Stability
    0 **[[Free Strike]]:** 3'
- name: Lethe
  effect: While winded, the bendrak has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the bendrak can’t be hidden from them.
abilities:
- name: Warp Perceptions
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature
  t1: 3 psychic damage; P1 [[Weakened|weakened]] (save ends)
  t2: 5 psychic damage; P2 [[Weakened|weakened]] (save ends)
  t3: 7 psychic damage; P3 [[Weakened|weakened]] (save ends)
  effects:
  - name: Effect
    effect: 'If the target makes an attack while [[Weakened|weakened]] this way, the bendrak can
      choose a second target for the attack within the distance of the attack, then
      evenly divides any damage from the attack between the two targets. '
- name: Vanish
  type: Maneuver
  cost: 1 Malice
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Self or one ally
  effects:
  - name: Effect
    effect: 'The target immediately becomes hidden, regardless of whether they have
      cover or concealment. '

```
