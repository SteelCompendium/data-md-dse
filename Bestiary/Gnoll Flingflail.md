```ds-statblock
name: Gnoll Flingflail
ancestry:
- Fiend
- Gnoll
roles:
- Artillery
- Minion
level: 2
ev: 5
stamina: 8
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 1
free_strike: 2
might: 2
intuition: 0
agility: 0
reason: 1
presence: -2
traits:
- name: Death Frenzy
  effect: Whenever an ally within 5 is reduced to 0 Stamina, the flingflail archer
    moves up to their speed and makes a [[Free Strike|free strike]].
abilities:
- name: Chain Shotput
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 8
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage; push 1

```
