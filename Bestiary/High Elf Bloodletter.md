```ds-statblock
name: High Elf Bloodletter
ancestry:
- Fey
- High Elf
- Humanoid
roles:
- Ambusher
level: 1
ev: 7
stamina: 10
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits:
- name: Otherworldly Grace
  effect: At the start of their turn, the scribe can turn the duration of one save
    ends effect they suffer from into EoT.
abilities:
- name: Razor’s Edge
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 4 damage; R1 [[Bleeding|bleeding]] (save ends)
  t2: 7 damage; R2 [[Bleeding|bleeding]] (save ends)
  effects:
  - name: Effect
    effect: 'A creature [[Bleeding|bleeding]] from this ability takes edge from attacks. '
- name: Blood Haze
  type: Maneuver
  cost: 2 Malice
  keywords:
  - Area
  - Magic
  distance: 3 burst
  target: Special
  effects:
  - name: Effect
    effect: 'The bloodletter creates a cloud of blood vapor in the area until the
      end of the next round. The cloud blocks line of effect for enemies, and an enemy
      has Magic weakness 3 occupying an affected square. The bloodletter then shifts
      up to their speed, hiding if they end their movement under concealment. '

```
