---
agility: 1
ancestry:
- Fey
- High Elf
- Humanoid
ev: '10'
file_basename: High Elf Wyrd
file_dpath: Monsters/Elves High/Statblocks
free_strike: 5
intuition: -1
item_id: high-elf-wyrd
item_index: '113'
item_name: High Elf Wyrd
level: 3
might: 0
presence: 2
reason: 2
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:high-elf-wyrd
scdc:
- 1.1.1:2:113
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: High Elf Wyrd
level: 3
roles:
  - Platoon Controller
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "10"
stamina: "40"
immunities:
  - Psychic 5
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 1
reason: 2
intuition: -1
presence: 2
traits:
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the wyrd can choose one effect on
          them that can be ended by a saving throw. That effect instead ends at
          the end of their turn.
abilities:
  - name: Twystrd
    cost: Signature Ability
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 1 cube within 5
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: Vertical push 3
        t2: Vertical push 5
        t3: Vertical push 6
      - effect: For each elemental mote adjacent to the wyrd, the size of the cube
          increases by 1.
        name: Effect
  - name: Summon Elemental
    cost: 2 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Special
    effects:
      - effect: The wyrd summons two elemental motes or two soot crows into unoccupied
          spaces within distance.
        name: Effect
  - name: Wyrd Warp
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 8 wall within 8
    target: Special
    effects:
      - effect: The wyrd shapes the land in the area as if it were loose clay, either
          raising the ground or pushing it down to create a trench. Any creature
          in the area moves with the terrain to its new higher elevation, or
          falls if the ground is lowered beneath them.
        name: Effect
```