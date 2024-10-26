```ds-statblock
name: Demon Torlas
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
- name: LEVEL 1 CONTROLLER
  effect: ''
- name: Demon, Planar EV 9
  effect: '**Stamina:** 15 **Weakness:** Holy 3 **Speed:** 5 **Size:** 1S / Stability
    0 **[[Free Strike]]:** 2'
- name: Lethe
  effect: While winded, the torlas has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 of the torlas can’t be hidden from them.
abilities:
- name: Cronenstorm
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: Each creature in the cube
  t1: Slide 1
  t2: Slide 2
  t3: Slide 3
  effects:
  - name: Effect
    effect: 'The area turns into a morass of spongy flesh before the targets are force
      moved. Until the start of the torlas’s next turn, the area is [[Difficult Terrain|difficult terrain]],
      and each creature who moves within the area takes 1 damage for each square moved. '
- name: Grasping Tendons
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Three creatures
  effects:
  - name: Effect
    effect: 'The torlas pulls each target 3 squares. '

```
