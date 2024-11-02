```ds-statblock
name: High Elf Orbweaver
ancestry:
- Fey
- High Elf
- Humanoid
roles:
- Hexer
level: 3
ev: 16
stamina: 35
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 0
intuition: 2
agility: 0
reason: 2
presence: 2
traits:
- name: Otherworldly Grace
  effect: At the start of their turn, the orbweaver can turn the duration of one save
    ends effect they suffer from into EoT.
abilities:
- name: Awash
  type: Action
  cost: Signature
  keywords:
  - Area
  - Magic
  distance: 3 cube within 1
  target: All creatures in the cube
  effects:
  - roll: 2d10 + 2
    t1: 3 damage; M1 [[Slowed|slowed]] (EoT)
    t2: 4 damage; M2 [[Slowed|slowed]] (EoT)
    t3: '5 cold damage; M3 [[Prone|prone]] '
- name: Aetherweb
  type: Action
  keywords:
  - Magic
  - Ranged
  distance: Ranged 8
  target: 2 enemies or objects
  effects:
  - roll: 2d10 + 2
    t1: 3 damage; R1 [[Slowed|slowed]] (save ends)
    t2: 5 damage; R2 [[Slowed|slowed]] (save ends)
    t3: 6 damage; R3 [[Restrained|restrained]] (save ends)
  - name: Effect
    effect: 'Each enemy within 3 of a target suffers the same additional effects as
      the target unless they shift into an unoccupied square adjacent to them. '

```
