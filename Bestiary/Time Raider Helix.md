~~~ds-statblock
name: [[Time Raider]] Helix
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Controller
level: 3
ev: 17
stamina: 40
immunities:
- Psychic 4
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1M
stability: 0
free_strike: 5
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Foresight
  effect: The helix doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Blaster Volley
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 4 corruption damage; push 2
  t2: 7 corruption damage; push 4
  t3: '10 corruption damage; push 6; [[Prone|prone]] '
  effects:
  - name: '**Keywords**'
    effect: Attack, Ranged, Psionic, Weapon
  - name: '**Distance**'
    effect: Ranged 10
  - name: '**Target**'
    effect: 'Three creatures '
- name: Kinetic Lane
  type: Maneuver
  effects:
  - name: '**Keywords**'
    effect: Area, Psionic, Ranged
  - name: '**Distance**'
    effect: 4 × 2 line within 10
  - name: '**Target**'
    effect: Special
  - name: '**Effect**'
    effect: Until the start of the helix’s next turn, the area becomes a psionically
      charged treadmill that pushes creatures and objects at high speed in one direction
      of the helix’s choice. Any creature that moves into the area or starts their
      turn there is immediately slid 3 squares toward the square at the end of the
      area in the appropriate direction, starting with creatures closest to the helix.
      Any non-[[Time Raider|time raider]] standing in the area when it first appears takes 3 damage
      before they are moved.
  - name: '**5 VP**'
    effect: 'The helix creates a second kinetic lane. '

~~~