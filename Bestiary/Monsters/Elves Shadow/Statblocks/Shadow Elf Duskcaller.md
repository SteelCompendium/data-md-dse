---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '14'
file_basename: Shadow Elf Duskcaller
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 2
item_id: shadow-elf-duskcaller
item_index: '215'
item_name: Shadow Elf Duskcaller
level: 5
might: 0
presence: 1
reason: 3
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:shadow-elf-duskcaller
scdc:
- 1.1.1:2:215
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster
---

```ds-statblock
name: Shadow Elf Duskcaller
level: 5
roles:
  - Platoon Controller
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "14"
stamina: "60"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 0
agility: 3
reason: 3
intuition: 2
presence: 1
traits:
  - name: Of the Umbra
    effects:
      - effect: The duskcaller ignores concealment created by darkness. While the
          duskcaller is in direct sunlight, they have damage weakness 3. While
          the duskcaller has concealment, they have damage immunity 3.
abilities:
  - name: Night Knife
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 13 damage
        t3: 16 damage
      - effect: If the duskcaller has concealment, they can target one additional
          creature or object.
        name: Effect
  - name: The Lay of Cor'thoroth
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 2 cube within 3
    target: Special
    effects:
      - effect: Until the start of the duskcaller's next turn, the area is filled with
          darkness.
        name: Effect
      - effect: The size of the cube increases by 3.
        cost: 2 Malice
```