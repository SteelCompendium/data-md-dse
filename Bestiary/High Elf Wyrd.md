```ds-statblock
name: High Elf Wyrd
ancestry:
- Fey
- High Elf
- Humanoid
roles:
- Controller
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
intuition: -1
agility: 1
reason: 2
presence: 2
traits:
- name: Otherworldly Grace
  effect: At the start of their turn, the wyrd can turn the duration of one save ends
    effect they suffer from into EoT.
abilities:
- name: Twystrd
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: 1 cube within 5
  target: All enemies in the cube
  effects:
  - roll: 2d10 + 2
    t1: vertical push 2
    t2: vertical push 3
    t3: vertical push 5
  - name: Effect
    effect: 'The area of the cube increases by 1 for each [[Elemental Mote|elemental mote]] adjacent
      to the wyrd. '
- name: Wyrd Warp
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 8 wall within 8
  target: Special
  effects:
  - name: Effect
    effect: 'The wyrd shapes the land as if it were loose clay. Each wall segment
      is a full cube. A segment can also be used to push a square of the terrain further
      into the ground. An enemy within an affected square moves with the elevation
      of the terrain. '

```
