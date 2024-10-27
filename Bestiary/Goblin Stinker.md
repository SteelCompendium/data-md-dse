```ds-statblock
name: Goblin Stinker
ancestry:
- Goblin
- Humanoid
roles:
- Controller
level: 1
ev: 9
stamina: 15
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: -2
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Crafty
  effect: The stinker doesn't provoke opportunity attacks by moving.
abilities:
- name: Toxic Winds
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: Each enemy
  t1: 1 poison damage; slide 1
  t2: 2 poison damage; slide 2
  t3: 3 poison damage; slide 3
  effects:
  - name: 1 Malice
    effect: 'Increase the slide for one target by 2 squares. '
- name: Swamp Gas
  type: Maneuver
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: Special
  effects:
  - name: Effect
    effect: 'The area is filled with a green haze until the start of the stinker''s
      next turn or until the stinker is reduced to Stamina 0. The area is difficult
      terrain for non-goblin creatures, and each such creature who moves within the
      area takes 2 poison damage for each square moved. The haze can''t be dispersed
      by wind. '

```
