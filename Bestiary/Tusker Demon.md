```ds-statblock
name: Tusker Demon
ancestry:
- Demon
- Gnoll
- Planar
roles:
- Brute
level: 2
ev: 15
stamina: 35
immunities:
- weapon 3
weaknesses: []
speed: '7'
size: '3'
stability: 3
free_strike: 4
might: 2
intuition: 0
agility: -1
reason: -3
presence: -1
traits:
- name: Trample
  effect: The tusker demon can move through enemies and objects at normal speed. When
    the tusker enters a creature's space for the first time on their turn, the creature
    takes 2d6 damage. The tusker demon can end their turn in a [[Prone|prone]] size 1 creature's
    space, preventing the creature from getting up.
- name: Lethe
  effect: While winded, the tusker demon has edge on attacks, and attacks have edge
    against them.
abilities:
- name: Gore
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 2
  target: 1 creature or object
  t1: 4 damage; push 1
  t2: 7 damage; push 2
  t3: 10 damage; push 3; [[Prone|prone]]
  effects:
  - roll: 2d10 + 2
    t1: 4 damage; push 1
    t2: 7 damage; push 2
    t3: 10 damage; push 3; [[Prone|prone]]
  - name: Effect
    effect: 'This attack has edge while charging. '
- name: Vengeful Tusker
  type: Triggered Action
  keywords:
  - '-'
  trigger: An enemy within 7 deals damage to the tusker.
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The tusker demon [[Charge|charges]] the target using Gore. '

```
