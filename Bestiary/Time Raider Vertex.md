~~~ds-statblock
name: [[Time Raider]] Vertex
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Support
level: 3
ev: 19
stamina: 50
immunities:
- Psychic 5
weaknesses: []
speed: 5 ([[Fly|fly]])
size: '2'
stability: 3
free_strike: 5
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Foresight
  effect: The vertex doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Psionic Slam
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 3 damage; 2 psychic damage
  t2: 5 damage; 3 psychic damage
  t3: 7 damage; 4 psychic damage
  effects:
  - name: '**Keywords**'
    effect: Attack, Melee, Psionic
  - name: '**Distance**'
    effect: Reach 2
  - name: '**Target**'
    effect: 'One creature '
  - name: '**Effect**'
    effect: 'Any ability used against the target gains an edge until the start of
      the vertex’s next turn. '
- name: Split Space
  type: Action
  effects:
  - name: '**Keywords**'
    effect: Area, Psionic, Ranged
  - name: '**Distance**'
    effect: 2 cube within 10
  - name: '**Target**'
    effect: Special
  - name: '**Effect**'
    effect: 'A portal fills the area, leading to a location the vertex has seen (in
      person or otherwise) on any plane of existence. Each creature who touches the
      portal is instantly teleported to the nearest unoccupied square at the chosen
      location. The portal lasts until the vertex dies, uses this ability again, dismisses
      the portal (no action required), or is transported by the portal. '
- name: Invigorated March
  type: Maneuver
  effects:
  - name: '**Keywords**'
    effect: Area, Psionic
  - name: '**Distance**'
    effect: 4 burst
  - name: '**Target**'
    effect: Each ally
  - name: '**Effect**'
    effect: 'Each target can shift half their speed. '

~~~