~~~ds-statblock
name: Demon Torlas
ancestry:
- Demon
- Planar
roles:
- Controller
level: 1
ev: 9
stamina: 15
immunities: []
weaknesses: []
speed: '5'
size: 1S
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 1
traits:
- name: Lethe
  effect: While winded, the torlas has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 squares of the torlas can’t be hidden from them.
abilities:
- name: Cronenstorm
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: Each creature
  t1: Slide 1
  t2: Slide 2
  t3: Slide 3
  effect: 'The area turns into a morass of spongy flesh before the targets are force
    moved. Until the start of the torlas’s next turn, the area is difficult terrain,
    and each creature who moves within the area takes 1 damage for each square moved. '
- name: Grasping Tendons
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Three creatures
  effect: 'The torlas pulls the target up to 2 squares. '
weakness: Holy 3

~~~