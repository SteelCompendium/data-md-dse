---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '10'
file_basename: Wode Elf Gweiadur
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 5
intuition: 1
item_id: wode-elf-gweiadur
item_index: '228'
item_name: Wode Elf Gweiadur
level: 3
might: 0
presence: 0
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster:wode-elf-gweiadur
scdc:
- 1.1.1:2:228
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: Wode Elf Gweiadur
level: 3
roles:
  - Platoon Artillery
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "10"
stamina: "40"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the gweiadur that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Snare Bow
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage
        t3: 14 damage; A < 2 restrained (save ends)
      - effect: The gweiadur shifts up to 3 squares
      - effect: If this ability restrains the target, one enemy adjacent to the target
          is also restrained (save ends).
        cost: 3 Malice
  - name: You Activated My Trap!
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 damage; R < 0 the target is marked (save ends)
        t2: 6 damage; R < 1 slowed and the target is marked (save ends)
        t3: 9 damage; R < 2 slowed and the target is marked (save ends)
      - effect: Allies gain an edge on abilities against a target marked by any wode
          elf.
```