```ds-statblock
name: Ghoul
ancestry:
- Corporeal
- Undead
roles:
- Harrier
level: 1
ev: 8
stamina: 15
immunities:
- Corruption 3
- Poison 3
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 3
might: 0
intuition: 0
agility: 2
reason: -2
presence: -1
traits:
- name: Hunger
  effect: If the ghoul [[Charge|charges]], their speed increases by 2 until the end of their
    turn.
- name: Arise
  effect: The first time the ghoul is reduced to Stamina 0 by damage that isn't fire
    damage or holy damage and their body isn't destroyed, they regain half their Stamina
    and fall [[Prone|prone]].
abilities:
- name: Razor Claws
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 2 damage; M1 [[Bleeding|bleeding]] (save ends)
  t2: 4 damage; M2 [[Bleeding|bleeding]] (save ends)
  t3: '5 damage; M3 [[Bleeding|bleeding]] (save ends) '
- name: Leap
  type: Maneuver
  keywords:
  - '-'
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The ghoul leaps 3 squares. If they land on a size 1 enemy, that enemy
      is knocked [[Prone|prone]] and the ghoul makes a [[Free Strike|free strike]] against them. '

```
