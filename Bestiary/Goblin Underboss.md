~~~ds-statblock
name: Goblin Underboss
ancestry:
- Goblin
- Humanoid
roles:
- Support
level: 1
ev: 10
stamina: 20
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: -1
intuition: 0
agility: 1
reason: 0
presence: 1
traits:
- name: Crafty
  effect: The underboss doesn’t provoke opportunity attacks by moving.
abilities:
- name: Sword
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object
  t1: 2 damage
  t2: 5 damage
  t3: 6 damage
  effect: 'One ally of the underboss adjacent to the target can make a free strike
    against them. '
- name: Get Reckless!
  type: Maneuver
  keywords:
  - Ranged
  distance: Ranged 10
  target: Each ally
  effect: 'Until the start of the underboss’s next turn, each target gains an edge
    on attacks, and attacks against them gain an edge. '

~~~