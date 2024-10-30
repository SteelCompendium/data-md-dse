```ds-statblock
name: Elemental Mote
ancestry:
- Elemental
- High Elf
roles:
- Hexer
- Minion
level: 1
ev: 5
stamina: 8
immunities: []
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1T
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 0
reason: 0
presence: 2
traits:
- name: Cradle Heart
  effect: On their turn, the mote can choose to die to revive a dead [[Cradle Crow|cradle crow]],
    [[Cradle Horse|cradle horse]], or [[Cradle Credenza|cradle credenza]] within 1, returning with 8 Stamina.
abilities:
- name: Dweomer Plume
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  distance: Melee 2
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage; the target gains Magic weakness 1 (EoT)
  t3: '5 damage; the target gains Magic weakness 3 (EoT) '
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 4 damage; the target gains Magic weakness 1 (EoT)
    t3: '5 damage; the target gains Magic weakness 3 (EoT) '

```
