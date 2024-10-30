```ds-statblock
name: Abyssal Hyena
ancestry:
- Animal
- Gnoll
roles:
- Brute
- Minion
level: 2
ev: 7
stamina: 15
immunities: []
weaknesses: []
speed: '8'
size: 1M
stability: 1
free_strike: 2
might: 2
intuition: 0
agility: 1
reason: -3
presence: -2
traits:
- name: Death Snap
  effect: When the abyssal hyena is reduced to 0 Stamina, they make a [[Free Strike|free strike]]
    before dying.
abilities:
- name: Snapjaw
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage; [[Grabbed|grabbed]]
  t3: '5 damage; [[Grabbed|grabbed]] '
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 4 damage; [[Grabbed|grabbed]]
    t3: '5 damage; [[Grabbed|grabbed]] '

```
