```ds-statblock
name: Shade
ancestry:
- Incorporeal
- Undead
roles:
- Ambusher
- Minion
level: 1
ev: 3
stamina: 5
immunities:
- Corruption 2
- Poison 2
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1M
stability: 1
free_strike: 2
might: -5
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Corruptive Phasing
  effect: The shade can move through other creatures and objects at normal speed.
    The first time in a round that the shade passes through a creature, that creature
    takes 2 corruption damage.
abilities:
- name: Life Drain
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 corruption damage
    t2: 3 corruption damage
    t3: '4 corruption damage; the target moves up to their speed away from all shades '

```
