```ds-statblock
name: High Elf Quiver
ancestry:
- Fey
- High Elf
- Humanoid
roles:
- Artillery
- Minion
level: 1
ev: 6
stamina: 8
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: 1
presence: 0
traits:
- name: Otherworldly Grace
  effect: At the start of their turn, the quiver can turn the duration of one save
    ends effect they suffer from into EoT.
abilities:
- name: Heavy Arrow
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 5 damage; target’s speed reduced by 1 (EoT)

```
