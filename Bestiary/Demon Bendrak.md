~~~ds-statblock
name: Demon Bendrak
ancestry:
- Demon
- Planar
roles:
- Hexer
level: 2
ev: 11
stamina: 20
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
  effect: While winded, the bendrak has an edge on attacks, and attacks have an edge
    against them.
- name: Soulsight
  effect: Each creature within 2 squares of the bendrak can’t be hidden from them.
abilities:
- name: Warp Perceptions
  type: Action
  roll: PRS RR
  cost: Signature
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  effect: 'If the target makes an attack while weakened this way, the bendrak can
    choose a second target for the attack within the distance of the attack, then
    evenly divides any damage from the attack between the two targets. '
- name: Vanish
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Self or one ally
  effect: 'The target immediately becomes hidden, regardless of whether they have
    cover or concealment. '
weakness: Holy 3

~~~